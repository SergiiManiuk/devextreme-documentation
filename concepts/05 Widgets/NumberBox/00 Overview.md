The **NumberBox** is a widget that displays a numeric value and allows a user to modify it by typing in a value, and incrementing or decrementing it using the keyboard or mouse.

<a href="https://js.devexpress.com/Demos/WidgetsGallery/#demo/editors-number_box-overview" class="button orange small fix-width-155" style="margin-right: 20px;" target="_blank">View Demo</a>

The following code adds the **NumberBox** to your page. The simplest configuration of the widget requires only a [value](/api-reference/10%20UI%20Widgets/dxNumberBox/1%20Configuration/value.md '/Documentation/ApiReference/UI_Widgets/dxNumberBox/Configuration/#value') to be specified. In addition, you can specify the [placeholder](/api-reference/10%20UI%20Widgets/dxTextEditor/1%20Configuration/placeholder.md '/Documentation/ApiReference/UI_Widgets/dxNumberBox/Configuration/#placeholder') to be displayed when the number box is empty.

    <!--HTML-->
    <div id="numberBoxContainer"></div>

<!---->    

    <!--JavaScript-->
    $(function() {
        $("#numberBoxContainer").dxNumberBox({
            value: 20,
            placeholder: 'Enter your age'
        });
    });

In most cases, it is useful to specify the range of possible values. For this purpose, set the [min](/api-reference/10%20UI%20Widgets/dxNumberBox/1%20Configuration/min.md '/Documentation/ApiReference/UI_Widgets/dxNumberBox/Configuration/#min') and [max](/api-reference/10%20UI%20Widgets/dxNumberBox/1%20Configuration/max.md '/Documentation/ApiReference/UI_Widgets/dxNumberBox/Configuration/#max') options.

    <!--JavaScript-->
    $(function() {
        $("#numberBoxContainer").dxNumberBox({
            value: 20,
            min: 16,
            max: 100
        });
    });

If the entered value falls out of the range, the widget sets the value to the lower (if the value is less than the lower bound) or upper bound (if the value is greater than the upper bound).

#####See Also#####
- [Widget Basics - jQuery](/concepts/00%20Getting%20Started/10%20Widget%20Basics%20-%20jQuery '/Documentation/Guide/Getting_Started/Widget_Basics_-_jQuery/')
- [Widget Basics - AngularJS](/concepts/00%20Getting%20Started/20%20Widget%20Basics%20-%20AngularJS '/Documentation/Guide/Getting_Started/Widget_Basics_-_AngularJS/')
- [Widget Basics - Knockout](/concepts/00%20Getting%20Started/25%20Widget%20Basics%20-%20Knockout '/Documentation/Guide/Getting_Started/Widget_Basics_-_Knockout/')
- [NumberBox - Handle the Value Change Event](/concepts/05%20Widgets/NumberBox/10%20Handle%20the%20Value%20Change%20Event.md '/Documentation/Guide/Widgets/NumberBox/Handle_the_Value_Change_Event')
- [NumberBox - Control the Behavior](/concepts/05%20Widgets/NumberBox/15%20Control%20the%20Behavior.md '/Documentation/Guide/Widgets/NumberBox/Control_the_Behavior')
- [NumberBox - Keyboard Support](/concepts/05%20Widgets/NumberBox/20%20Keyboard%20Support.md '/Documentation/Guide/Widgets/NumberBox/Keyboard_Support')
- [NumberBox API Reference](/api-reference/10%20UI%20Widgets/dxNumberBox '/Documentation/ApiReference/UI_Widgets/dxNumberBox/')

[tags]number box, numberBox, editor, overview