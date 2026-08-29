# Slideshow View

The Slideshow view displays a full-screen, responsive photo slideshow ideal for smart displays and digital photo frames. It integrates seamlessly with View Assist gesture navigation and background synchronization.

## Features

- **Full Viewport Scaling**: Clean responsive layout tailored for View Assist satellite displays.
- **Gesture Controls**: Navigate forward, backward, or pause playback using swipe/touch gestures or voice.
- **Background Synchronization**: Synchronize background pictures to View Assist devices.
- **Automatic Blueprint Installation**: Enabling Slideshow via the View Assist integration automatically installs its linked automations!

## Installation & Enabling

You can enable this view directly using the View Assist integration UI:
1. In Home Assistant, go to **Settings** → **Devices & Services** → **View Assist**.
2. Click **Configure** on your **Master Configuration** entry.
3. Select **Manage Views & Features**.
4. Check **Slideshow** under **Community Contribution Views**.

When enabled, View Assist will automatically:
- Install the `slideshow` view onto your dashboard (`/view-assist/slideshow`).
- Install the linked blueprints:
  - `blueprint-slideshow_gesture_controls.yaml` (Gesture navigation)
  - `blueprint-sync_album_slideshow_background.yaml` (Album background sync)

## Changelog

| Version | Description |
| ------- | ----------- |
| v 1.0.0 | Initial release with automatic integration blueprint lifecycle support |
