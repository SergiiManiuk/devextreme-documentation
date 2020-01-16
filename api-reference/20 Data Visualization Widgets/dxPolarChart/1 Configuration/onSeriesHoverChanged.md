---
EventForAction: ..\4 Events\seriesHoverChanged.md
type: function(e)
---
---
##### notUsedInTheme

##### shortDescription
A handler for the [seriesHoverChanged](/api-reference/20%20Data%20Visualization%20Widgets/dxPolarChart/4%20Events/seriesHoverChanged.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxPolarChart/Events/#seriesHoverChanged') event.

##### param(e): Object
Information about the event.

##### field(e.component): Object
The <a href="/Documentation/16_2/ApiReference/Data_Visualization_Widgets/dxPolarChart/Methods/#instance">widget instance</a>.

##### field(e.element): Object
The widget's container.

##### field(e.target): Series
The series whose hover state has been changed.

---
When implementing a handling function, use the object passed to it as its parameter. Among the fields of this object, you can find the series whose hover state has been changed. To identify whether this series was hovered over or hovered out, call its [isHovered()](/api-reference/20%20Data%20Visualization%20Widgets/BaseChart/7%20Chart%20Elements/Series/3%20Methods/isHovered().md '/Documentation/ApiReference/Data_Visualization_Widgets/dxPolarChart/Chart_Elements/Series/Methods/#isHovered') method. To discover series fields and methods, refer to the [Series](/api-reference/20%20Data%20Visualization%20Widgets/dxPolarChart/7%20Chart%20Elements/Series '/Documentation/ApiReference/Data_Visualization_Widgets/dxPolarChart/Chart_Elements/Series/') class description.

To learn more about how to handle hover operations, refer to the [Hover Handling](/concepts/05%20Widgets/zz%20Common/10%20Data%20Visualization%20Widgets/90%20Charts%20-%20End-User%20Interaction/3%20Hover%20Handling '/Documentation/Guide/Widgets/Common/Data_Visualization_Widgets/Charts_-_End-User_Interaction/Hover_Handling') topic.