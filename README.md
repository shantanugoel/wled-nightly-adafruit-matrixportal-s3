# WLED MatrixPortal Nightly Builds

Automated nightly builds of [WLED](https://github.com/wled/WLED) for the **Adafruit MatrixPortal ESP32-S3** board.

## Downloads

Check the [Releases](../../releases) page for the latest nightly firmware.

## What This Repo Does

- Runs a nightly GitHub Action at 2 AM UTC
- Clones the latest upstream WLED
- Builds firmware specifically for the MatrixPortal ESP32-S3 with HUB75 matrix support
- Publishes the `.bin` file as a release

## Manual Trigger

You can manually trigger a build from the [Actions](../../actions) tab.

## Configuration

The build uses upstream WLED's `platformio_override.sample.ini` which includes the MatrixPortal configuration with:
- HUB75 Matrix Panel support
- Audio reactive usermod
- PSRAM enabled
- Optimized settings for the MatrixPortal board
