# kap-cam

> A [Kap](https://github.com/wulkano/kap) plugin that adds a Loom-like Webcam overlay to recordings.

## Installation

This requires using the terminal currently. The package is yet to be included by `npms.io`. It uses e.g. the number of stars of a repository to determine whether to include a package.

1. Open your terminal and enter the following command to download and make available the plugin to kap:

```
cd ~/Library/Application\ Support/Kap/plugins/
npm remove kap-camera
git clone https://github.com/thunfischbrot/kap-cam
npm link ./kap-cam
sed -i '' 's/"dependencies": {/"dependencies": {\n    "kap-cam": "latest",/' package.json
npm link
```

2. Open Kap `Preferences`
3. Select the `Plugins` pane, and switch to `Discover` tab.
4. In the list of plugins, find `cam` and toggle it on.

## Usage

To enable or disable the overlay:

1. Right click the Kap menu icon or click the `…` icon in the cropper.
2. In the `Plugins` menu, check or uncheck `Show Camera`

Note that the Camera window does not appear until you start a recording.

## Notes

This is based off of [@karaggeorge's](https://github.com/karaggeorge) [kap-camera](https://github.com/karaggeorge/kap-camera/) plugin, which was forked by [@clearlysid](https://github.com/clearlysid/kap-cam), which was forked by [@maticrivo](https://github.com/maticrivo/kap-cam). The repos seem to be inactive, with some features broken, so I decided to fork and maintain my own. Feel free to raise issues, leave feedback or contribute in any way you see fit.

## Demo

![demo](https://user-images.githubusercontent.com/30227512/193472451-810ad0e7-a90f-4b06-b819-28347f1cb771.gif)
