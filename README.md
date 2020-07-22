# <img src="https://github.com/sieteunoseis/betterbat-public-releases/blob/master/images/logo.png" width="60px" align="center" alt="Better BAT icon"> Better BAT

Better BAT was created to improve the bulk administration experience when using Cisco's Unified Communications Manager.

<h3 align="center">
  <a href="https://github.com/sieteunoseis/betterbat-public-releases/releases/latest">
  Download Better BAT for macOS or Windows
  </a>
</h3>

<p align="center">
<img src="https://github.com/sieteunoseis/betterbat-public-releases/blob/master/images/better-bat-social-preview.png" width="640px" alt="Better BAT screenshot">
</p>

# Features

### Live Feedback

![Screenshot: Better BAT running](https://github.com/sieteunoseis/betterbat-public-releases/blob/master/images/live-feedback.png)

Better BAT shows misconfigurations with your import file before you make any changes. This saves engineers from issues stemming from bad data collections, typo's or features not supported all phone models.

* #### Legend
  - ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) `#f03c15`
  - ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) `#c5f015`
  - ![#1589F0](https://via.placeholder.com/15/1589F0/000000?text=+) `#1589F0`

### Auto-Fix

![Screenshot: Better BAT auto-fix](https://github.com/sieteunoseis/betterbat-public-releases/blob/master/images/auto-fix.png)

Better BAT has a built in auto-fix feature to help engineers fix missing or misconfigurations. Currently Auto-Fix will help solve the following:

* Phone Button Template
  * Auto-Fix will analyze the number of lines and speed dials configured on each device. It will then try to select the best phone template that matches the configuration. (Note: Auto-Fix will only select phone templates that match the exact phone model)
* Device Pool
  * Via the Settings > Options > Auto-Fix Keyword, Auto-Fix will try to select a Device Pool that contains the keyword. This is useful if you use site codes or any other naming convention. (Note: Auto-Fix will only change/update fields that are marked as incorrect)
* Location
  * Via the Settings > Options > Auto-Fix Keyword, Auto-Fix will try to select a Location that contains the keyword. This is useful if you use site codes or any other naming convention. (Note: Auto-Fix will only change/update fields that are marked as incorrect)
* Max Call/Busy Trigger
  * Auto-Fix will look up the default settings per device type and fill in the missing values
* Device Security Profile
  * Auto-Fix will select the default Device Security Profile for the particular device type. Example: for a Cisco 8845, Auto-Fix would select "Cisco 8845 - Standard SIP Non-Secure Profile". (Note: This feature is for phones configured as SIP in the Device Protocol)
* MLPP Support (MLPP Indication & MLPP Preemption)
  * Auto-Fix will look up the default settings per device type and set to off if the model does not support the feature.
* Extension Mobility Support
  * Auto-Fix will look up the default settings per device type and set to off if the model does not support the feature.
* DND Support
  * Auto-Fix will look up the default settings per device type and set to off if the model does not support the feature.
* SIP Profile
  * Auto-Fix will select "Standard SIP Profile" if this is missing from the import file. "Standard SIP Profile" is a non-deletable profile in Communication Manager.
* Common Phone Profile
  * Auto-Fix will select "Standard Common Phone Profile" if this is missing from the import file. "Standard Common Phone Profile" is a deletable profile in Communication Manager, please verify that it still there before using Better BAT.
* Line Display and Alerting Names
  * Auto-Fix will copy data from Display (Caller ID) to ASCII Display (Caller ID) if missing.
  * Auto-Fix will copy data from Alerting Name to ASCII Alerting Name if missing.
* Call Forward to Voicemail Settings
* CSS (Calling Search Space)

### Handsontable

![Screenshot: Fiddle's Types](https://user-images.githubusercontent.com/1426799/43874324-10e46eae-9b40-11e8-962b-8c793d73c259.png)

Fiddle includes Microsoft's excellent Monaco Editor, the same editor powering
Visual Studio Code. It also installs the type definitions for the currently
selected version of Electron automatically, ensuring that you always have
all Electron APIs only a few keystrokes away.

### Compile and Package

![Screenshot: Fiddle's Tasks Menu](https://user-images.githubusercontent.com/1426799/52155857-c0bb4300-2639-11e9-8776-e05dc528439c.png)

Fiddle can automatically turn your experiment into binaries you can share with
your friends, coworkers, or grandparents. It does so thanks to
[electron-forge][electron-forge], allowing you to package your fiddle as an
app for Windows, macOS, or Linux.

### Start with Fiddle, Continue Wherever

![Screenshot: Visual Studio Code with Fiddle Export](https://user-images.githubusercontent.com/1426799/43874411-9cfd5946-9b40-11e8-8797-dd4138e31933.png)

Fiddle is not an IDE – it is however an excellent starting point. Once your
fiddle has grown up, export it as a project with or without
[electron-forge][electron-forge]. Then, use your favorite editor and take on
the world!

## Contributing

Electron Fiddle is a community-driven project that welcomes all sorts of contributions. Please check out our [Contributing Guide](https://github.com/electron/fiddle/blob/master/CONTRIBUTING.md) for more details.

## License

[MIT, please see the LICENSE file for full details](https://github.com/electron/fiddle/blob/master/LICENSE.md).

When using the Electron or other GitHub logos, be sure to follow the [GitHub
logo guidelines](https://github.com/logos).

[BrowserView]: https://electronjs.org/docs/api/browser-view
[desktopCapturer]: https://electronjs.org/docs/api/desktop-capturer
[electron-forge]:  https://electronforge.io/
