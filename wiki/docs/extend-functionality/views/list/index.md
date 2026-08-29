# List View

![](./listview.png)

- **Description**: Provides a view for presenting Home Assistant to-do list entities. Two variants are available: **Standard List (with Checkboxes)** for interactive task checking, and **No Checkbox List** for clean glanceable displays.
- **Default name**: `list`
- **Current Version**: v1.0.2
- **Code link**: [Standard List Raw Code](https://raw.githubusercontent.com/dinki/View-Assist/main/View%20Assist%20dashboard%20and%20views/views/list/list.yaml) | [List View No Checkbox](https://raw.githubusercontent.com/dinki/View-Assist/main/View%20Assist%20dashboard%20and%20views/views/list/list-nocheckbox.yaml)
- **Special Requirements**: None

## Configuration & Selection

Views are automatically installed and managed by the View Assist integration.

To choose your preferred list style:
1. Go to **Settings** → **Devices & Services** → **View Assist**.
2. Click **Configure** on your **Master Configuration** entry.
3. Select **Manage Views & Features**.
4. Set **List View Style** to either **Standard List (with Checkboxes)** or **No Checkbox List**.

## Changelog

| Version | Description                          |
| ------- | ------------------------------------ |
| v 1.0.2 | Added UI variant configuration support |
| v 1.0.1 | Move list variable out of dictionary |
| v 1.0.0 | Initial release                      |
