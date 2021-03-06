A funnel item is a visual representation of a data object.

![Funnel Items](/images/funnel/visual_elements/funnel-items.png)

Funnel items get their colors from the [palette](/api-reference/20%20Data%20Visualization%20Widgets/dxFunnel/1%20Configuration/palette.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxFunnel/Configuration/#palette') by default. If you want to use colors from the data source, specify the [colorField](/api-reference/20%20Data%20Visualization%20Widgets/dxFunnel/1%20Configuration/colorField.md '/Documentation/ApiReference/Data_Visualization_Widgets/dxFunnel/Configuration/#colorField') option.

---
##### jQuery

    <!--JavaScript-->
    $(function() {
        $("#funnelContainer").dxFunnel({
            dataSource: [
                { fruit: "Apples", count: 10, color: "green" },
                { fruit: "Oranges", count: 12, color: "orange" },
                { fruit: "Lemons", count: 15, color: "yellow" }
            ],
            argumentField: "fruit",
            valueField: "count",
            colorField: "color"
        });
    });

##### Angular

    <!--HTML-->
    <dx-funnel
        [dataSource]="fruits"
        argumentField="fruit"
        valueField="count"
        colorField="color">
    </dx-funnel>

    <!--TypeScript-->
    import { DxFunnelModule } from "devextreme-angular";
    // ...
    export class AppComponent {
        fruits = [
            { fruit: "Apples", count: 10, color: "green" },
            { fruit: "Oranges", count: 12, color: "orange" },
            { fruit: "Lemons", count: 15, color: "yellow" }
        ];
    }
    @NgModule({
        imports: [
            // ...
            DxFunnelModule
        ],
        // ...
    })

---

To configure other aspects of the funnel items' appearance, use the [item](/api-reference/20%20Data%20Visualization%20Widgets/dxFunnel/1%20Configuration/item '/Documentation/ApiReference/Data_Visualization_Widgets/dxFunnel/Configuration/item/') object.

---
##### jQuery

    <!--JavaScript-->
    $(function() {
        $("#funnelContainer").dxFunnel({
            // ...
            item: {
                border: {
                    visible: true
                }
            }
        });
    });

##### Angular

    <!--HTML-->
    <dx-funnel ... >
        <dxo-border
            [visible]="true">
        </dxo-border>
    </dx-funnel>

    <!--TypeScript-->
    import { DxFunnelModule } from "devextreme-angular";
    // ...
    export class AppComponent {
        // ...
    }
    @NgModule({
        imports: [
            // ...
            DxFunnelModule
        ],
        // ...
    })

---

Refer to other topics in this section for details on the main funnel item features.

#####See Also#####
- [Funnel Item Hover](/concepts/05%20Widgets/Funnel/14%20Funnel%20Items/10%20Hover '/Documentation/Guide/Widgets/Funnel/Funnel_Items/Hover/')
- [Funnel Item Selection](/concepts/05%20Widgets/Funnel/14%20Funnel%20Items/20%20Selection '/Documentation/Guide/Widgets/Funnel/Funnel_Items/Selection/')
- [Funnel Demos](https://js.devexpress.com/Demos/WidgetsGallery/Demo/Charts/FunnelChart)
