The **ResponsiveBox** widget allows you to create an application or a website with a layout adapted to different screen sizes.

![DevExtreme HTML5 JavaScript ResponsiveBox](/images/UiWidgets/responsive-box.png)

<a href="https://js.devexpress.com/Demos/WidgetsGallery/#demo/forms_and_multi-purpose-responsive_box-overview/tablet-landscape" class="button orange small fix-width-155" style="margin-right:5px;" target="_blank">View Demo</a>
<a href="https://www.youtube.com/watch?v=uoSs9cJc5gc&index=18&t=110s&list=PL8h4jt35t1wjGvgflbHEH_e3b23AA30-z" class="button orange small fix-width-155" target="_blank">Watch Video</a>

The following code creates a simple **ResponsiveBox**. The widget defines an ordinary page layout: a header, a footer, content area, left- and right-side bars. On small and extra small screens, the bars are hidden to give more space to the content. Note that the height of all elements that are ancestors to the **ResponsiveBox** (such as `<body>` and `<html>`) is explicitly set to *"100%"*. This makes the **ResponsiveBox** occupy full screen height.

    <!--HTML--><html style="height:100%">
        <!-- ... -->
    </html>
    
    <body style="height:100%">
        <div id="responsiveBoxContainer">
            <div class="header" data-options="dxItem: {
                location: [{
                    screen: 'md lg',
                    row: 0, col: 0,
                    colspan: 3
                }, {
                    screen: 'xs sm',
                    row: 0, col: 0
                }]
            }"> <p>Header</p> </div>

            <div class="content" data-options="dxItem: {
                location: [{
                    screen: 'md lg',
                    row: 1, col: 1
                }, {
                    screen: 'xs sm',
                    row: 1, col: 0
                }]
            }"> <p>Content</p> </div>

            <div class="left-side-bar" data-options="dxItem: {
                location: {
                    screen: 'md lg',
                    row: 1, col: 0
                }
            }"> <p>Left Bar</p> </div>

            <div class="right-side-bar" data-options="dxItem: {
                location: {
                    screen: 'md lg',
                    row: 1, col: 2
                }
            }"> <p>Right Bar</p> </div>

            <div class="footer" data-options="dxItem: {
                location: [{
                    screen: 'md lg',
                    row: 2, col: 0,
                    colspan: 3
                }, {
                    screen: 'xs sm',
                    row: 2, col: 0
                }]
            }"> <p>Footer</p> </div>
        </div>
    </body>

<!---->

    <!--JavaScript-->$(function() {
        $("#responsiveBoxContainer").dxResponsiveBox({
            rows: [
                { ratio: 1 },
                { ratio: 2 },
                { ratio: 0.7 }
            ],
            cols: [
                { ratio: 0.5, screen: "md lg" },
                { ratio: 2 },
                { ratio: 0.5, screen: "md lg" }
            ]
        });
    });

<!---->

    <!--CSS-->#responsiveBoxContainer p {
        font-size: 16px;
        padding-top: 10px;
        text-align: center;
    }

    .header { background: #f39e6c }
    .content { background: #f5e5a6 }
    .left-side-bar { background: #94d7c7 }
    .right-side-bar { background: #77c7e7 }
    .footer { background: #7b9bcf }
    
The **ResponsiveBox** elements in the code above are declared using the [dxItem](/api-reference/10%20UI%20Widgets/Markup%20Components/dxItem '/Documentation/ApiReference/UI_Widgets/Markup_Components/#dxItem') markup component. An object passed to this component can have the following fields.

- [location](/api-reference/10%20UI%20Widgets/dxResponsiveBox/5%20Default%20Item%20Template/location '/Documentation/ApiReference/UI_Widgets/dxResponsiveBox/Default_Item_Template/location/')
- [template](/api-reference/10%20UI%20Widgets/CollectionWidget/5%20Default%20Item%20Template/template.md '/Documentation/ApiReference/UI_Widgets/dxBox/Default_Item_Template/#template')
- [visible](/api-reference/10%20UI%20Widgets/CollectionWidget/5%20Default%20Item%20Template/visible.md '/Documentation/ApiReference/UI_Widgets/dxResponsiveBox/Default_Item_Template/#visible')

All **ResponsiveBox** elements are arranged against a layout grid defined by the [rows](/api-reference/10%20UI%20Widgets/dxResponsiveBox/1%20Configuration/rows '/Documentation/ApiReference/UI_Widgets/dxResponsiveBox/Configuration/rows/') and [cols](/api-reference/10%20UI%20Widgets/dxResponsiveBox/1%20Configuration/cols '/Documentation/ApiReference/UI_Widgets/dxResponsiveBox/Configuration/cols/') arrays. For further information, see the [Create the Layout Grid](/concepts/05%20Widgets/ResponsiveBox/10%20Create%20the%20Layout%20Grid.md '/Documentation/Guide/Widgets/ResponsiveBox/Create_the_Layout_Grid/') topic.

#####See Also#####
- [Widget Basics - jQuery](/concepts/00%20Getting%20Started/10%20Widget%20Basics%20-%20jQuery '/Documentation/Guide/Getting_Started/Widget_Basics_-_jQuery/')
- [Widget Basics - AngularJS](/concepts/00%20Getting%20Started/20%20Widget%20Basics%20-%20AngularJS '/Documentation/Guide/Getting_Started/Widget_Basics_-_AngularJS/')
- [Widget Basics - Knockout](/concepts/00%20Getting%20Started/25%20Widget%20Basics%20-%20Knockout '/Documentation/Guide/Getting_Started/Widget_Basics_-_Knockout/')
- [ResponsiveBox - Size Qualifiers](/concepts/05%20Widgets/ResponsiveBox/05%20Size%20Qualifiers.md '/Documentation/Guide/Widgets/ResponsiveBox/Size_Qualifiers/')
- [ResponsiveBox - Create the Layout Grid](/concepts/05%20Widgets/ResponsiveBox/10%20Create%20the%20Layout%20Grid.md '/Documentation/Guide/Widgets/ResponsiveBox/Create_the_Layout_Grid/')
- [ResponsiveBox - Arrange Layout Elements](/concepts/05%20Widgets/ResponsiveBox/15%20Arrange%20Layout%20Elements.md '/Documentation/Guide/Widgets/ResponsiveBox/Arrange_Layout_Elements/')
- [ResponsiveBox API Reference](/api-reference/10%20UI%20Widgets/dxResponsiveBox '/Documentation/ApiReference/UI_Widgets/dxResponsiveBox/')

[tags]responsive box, responsiveBox, layout widget, overview, dxItem, full screen widget