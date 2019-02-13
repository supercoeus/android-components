[android-components](../../index.md) / [mozilla.components.support.base.feature](../index.md) / [LifecycleAwareFeature](./index.md)

# LifecycleAwareFeature

`interface LifecycleAwareFeature : LifecycleObserver` [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/support/base/src/main/java/mozilla/components/support/base/feature/LifecycleAwareFeature.kt#L16)

An interface for all entry points to feature components to implement in order to make them lifecycle aware.

### Functions

| Name | Summary |
|---|---|
| [start](start.md) | `abstract fun start(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [stop](stop.md) | `abstract fun stop(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |

### Inheritors

| Name | Summary |
|---|---|
| [ContextMenuFeature](../../mozilla.components.feature.contextmenu/-context-menu-feature/index.md) | `class ContextMenuFeature : `[`LifecycleAwareFeature`](./index.md)<br>Feature for displaying a context menu after long-pressing web content. |
| [CoordinateScrollingFeature](../../mozilla.components.feature.session/-coordinate-scrolling-feature/index.md) | `class CoordinateScrollingFeature : `[`SelectionAwareSessionObserver`](../../mozilla.components.browser.session/-selection-aware-session-observer/index.md)`, `[`LifecycleAwareFeature`](./index.md)<br>Feature implementation for connecting an [EngineView](../../mozilla.components.concept.engine/-engine-view/index.md) with any View that you want to coordinate scrolling behavior with. |
| [CustomTabsToolbarFeature](../../mozilla.components.feature.customtabs/-custom-tabs-toolbar-feature/index.md) | `class CustomTabsToolbarFeature : `[`LifecycleAwareFeature`](./index.md)`, `[`BackHandler`](../-back-handler/index.md)<br>Initializes and resets the Toolbar for a Custom Tab based on the CustomTabConfig. |
| [DownloadsFeature](../../mozilla.components.feature.downloads/-downloads-feature/index.md) | `class DownloadsFeature : `[`SelectionAwareSessionObserver`](../../mozilla.components.browser.session/-selection-aware-session-observer/index.md)`, `[`LifecycleAwareFeature`](./index.md)<br>Feature implementation to provide download functionality for the selected session. The feature will subscribe to the selected session and listen for downloads. |
| [FindInPageFeature](../../mozilla.components.feature.findinpage/-find-in-page-feature/index.md) | `class FindInPageFeature : `[`LifecycleAwareFeature`](./index.md)`, `[`BackHandler`](../-back-handler/index.md)<br>Feature implementation that will keep a [FindInPageView](../../mozilla.components.feature.findinpage.view/-find-in-page-view/index.md) in sync with a bound [Session](../../mozilla.components.browser.session/-session/index.md). |
| [FullScreenFeature](../../mozilla.components.feature.session/-full-screen-feature/index.md) | `open class FullScreenFeature : `[`SelectionAwareSessionObserver`](../../mozilla.components.browser.session/-selection-aware-session-observer/index.md)`, `[`LifecycleAwareFeature`](./index.md)`, `[`BackHandler`](../-back-handler/index.md)<br>Feature implementation for handling fullscreen mode (exiting and back button presses). |
| [PromptFeature](../../mozilla.components.feature.prompts/-prompt-feature/index.md) | `class PromptFeature : `[`LifecycleAwareFeature`](./index.md)<br>Feature for displaying native dialogs for html elements like: input type date, file, time, color, option, menu, authentication, confirmation and alerts. |
| [SessionFeature](../../mozilla.components.feature.session/-session-feature/index.md) | `class SessionFeature : `[`LifecycleAwareFeature`](./index.md)`, `[`BackHandler`](../-back-handler/index.md)<br>Feature implementation for connecting the engine module with the session module. |
| [SitePermissionsFeature](../../mozilla.components.feature.sitepermissions/-site-permissions-feature/index.md) | `class SitePermissionsFeature : `[`LifecycleAwareFeature`](./index.md)<br>This feature will subscribe to the currently selected [Session](../../mozilla.components.browser.session/-session/index.md) and display a suitable dialogs based on [Session.Observer.onAppPermissionRequested](../../mozilla.components.browser.session/-session/-observer/on-app-permission-requested.md) or [Session.Observer.onContentPermissionRequested](../../mozilla.components.browser.session/-session/-observer/on-content-permission-requested.md)  events. Once the dialog is closed the [PermissionRequest](../../mozilla.components.concept.engine.permission/-permission-request/index.md) will be consumed. |
| [TabsFeature](../../mozilla.components.feature.tabs.tabstray/-tabs-feature/index.md) | `class TabsFeature : `[`LifecycleAwareFeature`](./index.md)<br>Feature implementation for connecting a tabs tray implementation with the session module. |
| [ToolbarFeature](../../mozilla.components.feature.toolbar/-toolbar-feature/index.md) | `class ToolbarFeature : `[`LifecycleAwareFeature`](./index.md)`, `[`BackHandler`](../-back-handler/index.md)<br>Feature implementation for connecting a toolbar implementation with the session module. |
| [WindowFeature](../../mozilla.components.feature.session/-window-feature/index.md) | `class WindowFeature : `[`LifecycleAwareFeature`](./index.md)<br>Feature implementation for handling window requests. |