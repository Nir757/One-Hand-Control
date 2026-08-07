<a id="top"></a>

# One Hand Control Background & Accessibility Reliability Guide

If One Hand Control stops working after closing the app, after some time in the background, or after using **Clear all** in Recent Apps, this is most likely related to Android or your phone manufacturer's background/battery management.

On some devices, the Accessibility permission can still appear enabled even though the service itself is no longer functioning correctly.

This is usually **not caused by your edge settings**. Your configuration may be completely fine while the system has stopped the background service.

## Quick navigation

### General

* [General steps to try first](#general)
* [Temporary workaround if nothing works](#workaround)
* [Still having problems?](#still-having-problems)

### Find your phone

* [Xiaomi / Redmi / POCO](#xiaomi)
* [vivo / iQOO](#vivo)
* [realme](#realme)
* [OPPO](#oppo)
* [OnePlus](#oneplus)
* [Huawei](#huawei)
* [HONOR](#honor)
* [ASUS / ROG Phone / Zenfone](#asus)
* [Samsung](#samsung)
* [Motorola](#motorola)
* [Google Pixel](#pixel)
* [TECNO / Infinix](#tecno-infinix)

---

<a id="general"></a>

# General steps to try first

## 1. Allow unrestricted background/battery usage

Open:

**Settings → Apps → One Hand Control → Battery / App battery usage**

Choose **Unrestricted**, **No restrictions**, **Allow background activity**, or the closest option your phone provides.

The exact name depends on your phone.

## 2. Temporarily disable Battery Saver

Turn off **Battery Saver / Power Saving mode** and check whether the issue still happens.

Some phones become much more aggressive about background apps while Battery Saver is enabled.

## 3. Lock One Hand Control in Recent Apps

If your phone supports it:

1. Open One Hand Control.
2. Open **Recent Apps**.
3. Open the menu for the One Hand Control card or long-press it.
4. Tap the **Lock** icon.

Not every phone supports this option.

## 4. Avoid repeatedly swiping One Hand Control away

If possible, avoid repeatedly opening One Hand Control and then removing it from Recent Apps.

On some Android skins, especially Xiaomi / Redmi / POCO, removing an app from Recents can cause the system to treat it as something you intentionally want stopped.

[↑ Back to top](#top)

---

# Manufacturer-specific settings

Menu names can vary slightly depending on your phone model and Android/software version.

<a id="xiaomi"></a>

## Xiaomi / Redmi / POCO

Enable **Background autostart**:

**Settings → Apps → Manage apps (if shown) → Background autostart**

Enable **One Hand Control**.

On some versions it may instead be:

**Settings → Apps → Permissions → Background autostart**

Also open:

**Settings → Apps → One Hand Control → Battery**

and choose **No restrictions**.

Video guide for enabling Autostart:

https://www.youtube.com/watch?v=4zC8NitQuN0

[↑ Back to top](#top)

---

<a id="vivo"></a>

## vivo / iQOO

Search Settings for:

**Autostart**

and enable it for **One Hand Control**.

On many versions it can be found under:

**Settings → Apps → Special app access → Autostart**

Also check One Hand Control's battery/background settings and allow background activity or high background power usage if available.

[↑ Back to top](#top)

---

<a id="realme"></a>

## realme

Open:

**Settings → Battery → App battery management → One Hand Control**

Enable:

* **Allow background activity**
* **Allow auto launch**

On some versions you can also find Auto-launch under:

**Phone Manager → Privacy Permissions → Auto-launch apps**

If supported, also lock One Hand Control in Recent Apps.

[↑ Back to top](#top)

---

<a id="oppo"></a>

## OPPO

Search Settings for:

**Auto launch**

and enable it for **One Hand Control**.

Then open:

**Settings → Apps → One Hand Control → Battery usage**

and enable **Allow background activity** if available.

The exact location of Auto launch varies between ColorOS versions.

[↑ Back to top](#top)

---

<a id="oneplus"></a>

## OnePlus

On newer OxygenOS versions, open:

**Settings → Battery → More settings → App battery management → One Hand Control**

Enable **Allow background activity**.

Older OxygenOS versions may also show an **Auto-launch** option. If you have it, enable it for One Hand Control.

If supported, you can also lock One Hand Control in Recent Apps.

[↑ Back to top](#top)

---

<a id="huawei"></a>

## Huawei

Open Settings and search for:

**App launch**

Find **One Hand Control** and turn off **Manage automatically**.

Then enable:

* **Auto-launch**
* **Secondary launch**
* **Run in background**

If supported, also lock One Hand Control in Recent Apps.

[↑ Back to top](#top)

---

<a id="honor"></a>

## HONOR

Open:

**Settings → Apps → App launch**

Find **One Hand Control** and turn off **Manage automatically**.

Then enable:

* **Auto-launch**
* **Secondary launch**
* **Run in background**

[↑ Back to top](#top)

---

<a id="asus"></a>

## ASUS / ROG Phone / Zenfone

Open:

**Settings → Battery → Auto-start Manager**

Find **One Hand Control** and set it to **Allow**.

[↑ Back to top](#top)

---

<a id="samsung"></a>

## Samsung

Samsung does not use a normal Auto-start switch.

Open:

**Settings → Battery → Background usage limits → Never sleeping apps**

Tap **+** and add **One Hand Control**.

Also make sure One Hand Control is **not** listed under:

* **Sleeping apps**
* **Deep sleeping apps**

Depending on your Android/One UI version, also check:

**Settings → Apps → One Hand Control → Battery**

and allow background usage if the option is available.

[↑ Back to top](#top)

---

<a id="motorola"></a>

## Motorola

On newer Motorola devices:

**Settings → Battery → Manage background apps → Background use → Smart use**

Select **One Hand Control** and choose:

**Always allow**

If you don't have this menu, check:

**Settings → Apps → One Hand Control → Battery**

and choose the least restrictive background option available.

[↑ Back to top](#top)

---

<a id="pixel"></a>

## Google Pixel

Open:

**Settings → Apps → One Hand Control → App battery usage**

Enable **Allow background usage**.

If your Android version provides an **Unrestricted** option, select it.

You can also open:

**App info → Unused apps**

and disable **Pause app activity if unused**.

[↑ Back to top](#top)

---

<a id="tecno-infinix"></a>

## TECNO / Infinix

These settings vary quite a lot between HiOS/XOS versions.

Search Settings or Phone Master for:

* **Auto-start**
* **Auto-start Management**
* **App launch**

and enable One Hand Control.

Also check:

**Settings → Apps → One Hand Control → Battery**

and use **Unrestricted / Allow background activity** if available.

[↑ Back to top](#top)

---

<a id="workaround"></a>

# If nothing above works — temporary workaround

If One Hand Control still stops working after being closed, this workaround can restore the Accessibility service without reopening the app.

First, open **One Hand Control** and finish configuring everything the way you want. This workaround works best when you don't expect to need to open the app itself again for a while.

Then:

1. Leave One Hand Control and remove it from **Recent Apps**.
2. Open **Settings → Accessibility → Downloaded apps → One Hand Control**.
3. Turn the Accessibility service **off**, then **back on**.
4. Check whether the edges are working again.

If it doesn't recover on the first try, toggle the Accessibility service off and on again. On some devices it may take **2–3 attempts**.

Once it starts working, you can use One Hand Control normally without opening the main app. It should continue working until the issue is triggered again.

[↑ Back to top](#top)

---

<a id="still-having-problems"></a>

# Still having problems?

Android manufacturers frequently change their background-management settings, so the exact menus may be slightly different on your phone.

This website also has manufacturer-specific background-app guides:

https://dontkillmyapp.com/

If you've tried everything above and One Hand Control still stops working, please send me a **bug report from inside the app** and I'll try my best to help 😄

[↑ Back to top](#top)
