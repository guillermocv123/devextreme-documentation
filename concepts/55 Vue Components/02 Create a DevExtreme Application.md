If you are starting a project from scratch, use the <a href="https://github.com/DevExpress/devextreme-vue-template#devextreme-vue-template" target="_blank">DevExtreme Vue Template</a>. It is a simple application with a navigation menu and several sample views in a responsive layout.

You can generate the application with the [DevExtreme CLI](/concepts/Common/DevExtreme%20CLI/00%20DevExtreme%20CLI.md '/Documentation/Guide/Common/DevExtreme_CLI/'):

    npx -p devextreme-cli devextreme new vue-app app-name
    cd app-name
    npm run serve

The application already contains the [DataGrid](https://js.devexpress.com/Demos/WidgetsGallery/Demo/DataGrid/Overview/Vue/Light) and [Form](https://js.devexpress.com/Demos/WidgetsGallery/Demo/Form/Overview/Vue/Light) components. You can find their configurations in the `src/views/display-data.vue` and `src/views/profile.vue` files correspondingly.

The following resources provide more information about DevExtreme Vue components:

- [Component Configuration Syntax](/concepts/55%20Vue%20Components/20%20Component%20Configuration%20Syntax '/Documentation/Guide/Vue_Components/Component_Configuration_Syntax/')
- [Demos](https://js.devexpress.com/Demos/WidgetsGallery/Demo/DataGrid/Overview/Vue/Light)
- [API Reference](/api-reference/10%20UI%20Widgets/dxAccordion '/Documentation/ApiReference/UI_Widgets/')
