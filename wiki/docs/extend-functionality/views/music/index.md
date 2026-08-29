# Music View

![](./musicview.png)

*Music View (Standard)*

---

![](./musicview-alt.png)

*Music View (Mini Media Player Alternative)*

---

- **Description**: Used for streaming music and radio. Two variants exist: **Standard Music Player** (using native Home Assistant `media-control`) and **Mini Media Player** (using `custom:mini-media-player`).
- **Default name**: `music`
- **Current Version**: v1.2.0
- **Code link**: [Standard Music Raw Code](https://raw.githubusercontent.com/dinki/View-Assist/main/View%20Assist%20dashboard%20and%20views/views/music/music.yaml) | [Music View Alternative Raw Code](https://raw.githubusercontent.com/dinki/View-Assist/main/View%20Assist%20dashboard%20and%20views/views/music/music-alternative.yaml)
- **Special Requirements**: Standard variant uses native cards. The Mini Media Player alternative requires `custom:mini-media-player` (available in HACS).

## Configuration & Selection

Views are automatically installed and managed by the View Assist integration.

To choose your preferred music player style:
1. Go to **Settings** → **Devices & Services** → **View Assist**.
2. Click **Configure** on your **Master Configuration** entry.
3. Select **Manage Views & Features**.
4. Set **Music View Style** to either **Standard Music (Media Control)** or **Mini Media Player**.

## Changelog

| Version | Description     |
| ------- | --------------- |
| v 1.2.0 | Added UI variant configuration support for Mini Media Player |
| v 1.0.0 | Initial release |
