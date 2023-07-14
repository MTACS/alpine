# Alpine

**Proper tvOS alerts for iOS**

![alpine-banner](https://github.com/MTACS/alpine/assets/13209789/fdcc60b6-b035-4bf2-a670-7123445c9921)
## Available soon on [Havoc](https://havoc.app)

Alpine uses classes and styling taken directly from tvOS to bring a clean and modern look to alerts system wide. [Cephei](https://chariz.com/get/cephei) is required for use in all apps on all jailbreaks (rootful & rootless) on iOS 14.0 - 16.x.

### Features

- Use fullscreen or alert only background blur
- Set type of background blur styling (iOS/tvOS)
- Choose interface style (dark/light/system) for all alert elements
- Tap anywhere outside alert view to dismiss
- Hide cancel button globally (automatically enables tap to dismiss)

### Example of tvOS classes used

```objective-c
%hook UIInterfaceActionVisualStyle
- (id)initWithConcreteVisualStyle:(id)arg0 {
	UIInterfaceActionConcreteVisualStyle_AppleTV *style = [%c(UIInterfaceActionConcreteVisualStyle_AppleTV) new];
	return %orig(style);
}
%end
```
### Screenshots

![screenshots](https://github.com/MTACS/alpine/assets/13209789/b8cd0a1f-0779-47b1-99c4-e0f9df4e76a6)

#
[Submit bug report](https://github.com/MTACS/alpine/issues/new?assignees=MTACS&labels=Bug&projects=&template=bug_report.md&title=)

[Request Feature](https://github.com/MTACS/alpine/issues/new?assignees=MTACS&labels=Enhancement&projects=&template=feature_request.md&title=)
