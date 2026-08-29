# Camera View

![](./cameraview.png)

- **Description**: A dynamic card that allows for full screen viewing of security cameras. Two variants are available: **Standard Camera (Grid)** using native Home Assistant cards, and **Advanced Camera Card** using `custom:advanced-camera-card`.
- **Default name**: `camera`
- **Current Version**: v2.1.0
- **Code link**: [Standard Camera Raw Code](https://raw.githubusercontent.com/dinki/View-Assist/main/View%20Assist%20dashboard%20and%20views/views/camera/camera.yaml) | [Advanced Camera Card Raw Code](https://raw.githubusercontent.com/dinki/View-Assist/main/View%20Assist%20dashboard%20and%20views/views/camera/advancedcamera.yaml)
- **Special Requirements**: Standard camera uses native cards. The Advanced Camera variant requires `custom:advanced-camera-card` (available in HACS).

## Configuration & Selection

Views are automatically installed and managed by the View Assist integration.

To choose your preferred camera card variant:
1. Go to **Settings** → **Devices & Services** → **View Assist**.
2. Click **Configure** on your **Master Configuration** entry.
3. Select **Manage Views & Features**.
4. Set **Camera View Style** to either **Standard Camera (Grid)** or **Advanced Camera Card**.

## Changelog

| Version | Description     |
| ------- | --------------- |
| v 2.1.0 | Added UI variant configuration support for Advanced Camera Card |
| v 1.0.0 | Initial release |
