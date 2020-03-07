# myOwnDialog

Modal box - jQuery - Simple and very effective modal box. [Demo](https://siva7170.github.io/myOwnDialog/modal.html)

## Getting Started

This plugin is work with jQuery. So, you need below requirements to work with this datepicker

### Prerequisites

* Latest jQuery

* `modalbox_v1.0.min.css`

* `modalbox_v1.0.min.js`

### Initialization

Place "modalbox_v1.0.min.css" and latest jQuery above the end head tag and place "modalbox_v1.0.min.js" above the end body tag.

```html
<html>
  <head>
    <link rel="stylesheet" href="css/modalbox_v1.0.min.css" type="text/css"/>
    <script src="script/jquery.min-3.1.1.js" type="text/javascript"></script> <!-- Please update with latest jQuery -->
  </head>
  <body>
    <!-- Your page content -->
    <script src="script/modalbox_v1.0.min.js" type="text/javascript"></script>
  </body>
</html>
```

## Usage

Below code is sample for how to use it. Please see methods and its functionalities below sections.

```html
<html>
<head>
    <link rel="stylesheet" href="css/modalbox_v1.0.min.css" type="text/css"/>
    <script src="script/jquery.min-3.1.1.js" type="text/javascript"></script> <!-- Please update with latest jQuery -->
</head>
<body>
    <div id="myDialog">
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
        Abcdefghijklmnopqrstuvwxyz Abcdefghijklmnopqrstuvwxyz
    </div>
    <button id="dialogop"> Click me[Movale,Not resizable]</button>
    <script src="script/modalbox_v1.0.min.js" type="text/javascript"></script>
    <script>
        // Apply Modalbox to "#myDialog"
        $("#myDialog").myOwnDialog(
            {
                autoClose: false,
                width: "400",
                pos_y: "50",
                height: "300",
                bg_color: 'white',
                title: "This is movable but not resizable",
                body_margin: "10",
                body_overflow_x: "hidden",
                body_overflow_y: "scroll",
                movable: true,
                resizable: false,
                touchOutsideForClose: false
            });
        // Apply Modalbox trigger for "#myDialog" from "#dialogop" button
        $("#dialogop").click(function () {
            $("#myDialog").myOwnDialog("open");
        });
    </script>
</body>
</html>
```
## Plugin parameters

### autoClose

- Type: `Boolean`|`String`
- Default: `false`

You can set time delay in milliseconds (Ex: for 5 seconds, autoClose:"5000") to close Modal box. If you don't want auto close, simply set autoClose:false

### width

- Type: `String`
- Default: `"300"`

You can set width of modalbox in pixel. Ex:. width:"500"

### height

- Type: `String`
- Default: `"200"`

You can set height of modalbox in pixel. Ex:. height:"300"

### pos_x

- Type: `String`
- Default: pos_x is automatically detected middle of screen in horizontal direction

Modal box is started with pos_x distance from left of browser window Ex:. pos_x:"150"

### pos_y

- Type: `String`
- Default: pos_y is automatically detected middle of screen in veritical direction

Modal box is started with pos_y distance from top of browser window Ex:. pos_y:"50"

### bg_color

- Type: `String`
- Default: `"white"`

You can change background color of modal box. Ex:. bg_color:"white" Or bg_color:"#ff8800"

### title

- Type: `String`
- Default: title will be shown as empty

You can set title of modal box. Ex:. title:"This is modal box"

### body_margin

- Type: `String`
- Default: `"5"`

This parameter is used for making margin(in pixel) on body of modal box and modal box window. Ex:. body_margin:"20"

### body_overflow_x

- Type: `String`
- Default: `"hidden"`

This parameter is used for apply overflow on horizontal direction of body of modal box. This parameter is same as overflow-x property. Ex:. body_overflow_x:"hidden"

### body_overflow_y

- Type: `String`
- Default: `"hidden"`

This parameter is used for apply overflow on veritical direction of body of modal box. This parameter is same as overflow-y property. Ex:. body_overflow_y:"hidden"

### movable

- Type: `Boolean`
- Default: `true`

By this parameter, you can set modal box behaviour. If this option set to true, you can able to move modal box in any where in browser window. If this option set to false, modal box is fixed on that position. Ex:. movable:false

### resizable

- Type: `Boolean`
- Default: `true`

You can resize modal box from all directions.(top,top-right,right,bottom-right,bottom,bottom-left,left,top-left) Ex:. resizable:false

### touchOutsideForClose (Not yet completed)
