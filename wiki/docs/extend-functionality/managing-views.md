---
title: "Managing Views & Features"
sidebar_position: 1
---

# Managing Views & Features

View Assist provides a built-in, UI-driven interface to customize which views appear on your View Assist dashboard, select between alternative view templates (variants), enable community-contributed views and automations, and load your own custom views.

---

## Accessing View Management

To manage views and features:
1. In Home Assistant, go to **Settings** → **Devices & Services**.
2. Locate the **View Assist** integration.
3. Click **Configure** on your **Master Configuration** entry.
4. Select **Manage Views & Features** from the menu.

---

## 1. Core Standard Views

View Assist comes with 15 core views designed for voice satellite displays. By default, all core views are enabled.

In the **Core Standard Views** selector, you can check or uncheck views to control which ones are included on your dashboard (`/view-assist`):

| View | Purpose | Associated Sentence Blueprint |
| :--- | :--- | :--- |
| **Clock** | Home time, date, and weather display | `What_time_is_it` |
| **Alarm** | Timer and alarm display with countdowns | `Alarms_Reminders_Timers` |
| **Alert** | Device alerts and popup banners | `Device_Alerts` |
| **Calendar** | Daily/monthly calendar agenda | `View_Calendar` |
| **Camera** | Security camera grid and full-screen streaming | `View_Camera` |
| **Info** | Wikipedia and general voice response information | `Search_Wikipedia`, `Spell_a_Word` |
| **Infopic** | Voice response text accompanied by images | `Search_Wikipedia` |
| **Intent** | Masonry layout for quick action controls | — |
| **List** | To-do and shopping list management | `List_Management` |
| **Locate** | Map view tracking family members or devices | `Locate_a_Person` |
| **Music** | Media player and streaming music control | `Play_Music_with_Music_Assistant`, `Play_Radio_with_Music_Assistant` |
| **Sports** | Live game scores and match tracking | `Get_Sports_Scores` |
| **Thermostat** | Climate control, temperature, and HVAC modes | `Thermostat_Control` |
| **Weather** | Forecast, hourly conditions, and weather stats | `Hows_the_weather` |
| **Webpage** | Embedded web content and iFrames | `Show_Webpage` |

When you uncheck a view, the integration automatically removes it from your dashboard without affecting your other configurations or templates.

---

## 2. Choosing View Variants (Alternative Views)

Several core views offer alternative layouts and card templates. You can choose your preferred style from the dropdown selectors:

### Camera View Style
- **Standard Camera (Grid)**: Uses Home Assistant native `picture-entity` cards in a responsive grid.
- **Advanced Camera Card**: Uses the `custom:advanced-camera-card` for PTZ controls, 2-way audio, and advanced streaming options.

### Music View Style
- **Standard Music (Media Control)**: Uses Home Assistant native `media-control` card.
- **Mini Media Player**: Uses `custom:mini-media-player` for a compact, rich media interface with progress bars and source selectors.

### List View Style
- **Standard List (with Checkboxes)**: Displays interactive checkboxes next to to-do items.
- **No Checkbox List**: Clean display without checkboxes, ideal for glanceable displays.

### Weather View Style
- **Standard Weather**: Clean forecast card with daily/hourly predictions.
- **Dynamic Weather**: Changes the background art dynamically to match real-time weather conditions.

### Clock View Style & Tap-to-Swap
- **Standard Digital Clock**: Large digital time with day, date, and weather badges.
- **Clock Alternative (Stacked)**: Stacked hour/minute display with ambient styling.
- **Clock with Movement**: Periodically shifts position across the screen to prevent OLED screen burn-in.
- **Enable ClockAlt Secondary View (Tap-to-Swap)**: When enabled, both `clock` and `clockalt` are installed on the dashboard. Tapping the time on the clock view seamlessly swaps between the standard and alternative views!

---

## 3. Community Contributions & Linked Blueprints

Official community views and blueprints are cached locally in your Home Assistant installation.

- When you check a community view (such as **Slideshow**), the View Assist integration:
  1. Installs the community view into your Lovelace dashboard.
  2. Automatically installs the linked community blueprints (e.g. gesture controls and background synchronization automations) into `blueprints/automation/dinki/`.
- When you uncheck the community view, the view is removed from the dashboard and the associated blueprints are cleaned up.

---

## 4. User Custom Views & Custom Blueprints (`custom/`)

You can create and use your own custom views and blueprints without modifying the integration code:

### Adding Custom Views
1. Place your view YAML file in:
   ```text
   /config/view_assist/views/custom/<view_name>.yaml
   ```
2. Open **Settings** → **Devices & Services** → **View Assist** → **Master Configuration** → **Manage Views & Features**.
3. Your custom view will appear under **User Custom Views** tagged with `[Custom]`.
4. Check the box to enable it on your dashboard!

### Adding Custom Blueprints
1. Place your automation blueprint YAML file in:
   ```text
   /config/view_assist/blueprints/custom/<blueprint_name>.yaml
   ```
2. In **Manage Views & Features**, select your custom blueprint under **Custom Blueprints** to install it into Home Assistant.
