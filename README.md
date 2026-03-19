# Nuke your Social Media and Pornography usage.


![High Friction Setup](https://raw.githubusercontent.com/creativeidiot123/Completely-kill-your-phone-addiction/main/kill-the-access-to-new-content-and-stop-doom-scrolling-v0-ylisxrl7gj0f1%20(1).webp)

This guide outlines a robust method to lock down your device, creating significant "friction" to prevent bypassing productivity blocks.

When properly implemented, this system is extremely resilient and designed to withstand nearly all common bypass attempts, including booting into Safe Mode, changing the device time, or uninstalling key applications without authorization.

---

## Phase 1: Preparation

### Download Initial Apps

On your phone download:
- **Destination:**  
  https://github.com/creativeidiot123/destination
  
- **The specified locker App:**  
  https://github.com/creativeidiot123/Lockey/releases  
  This will be used to store your emergency password.


### Secure and "Forget" the Password

Download lockey app above 

Generate a highly complex and random password. It should be impossible to memorize.

Example: b$ca{76r>t<3.w7yrqrt6dab?rtfg3iqrdasa

**Crucial Step:** You must not have easy access to this password.

Entrust it to a reliable person (like a family member or trusted friend) and put it in lockey app. Send it to them and then delete all records of it from your own devices and message history. The goal is that you cannot retrieve it on your own.

Put it in the Lockey app provided above, and put a 450+ character protection minimum.


# Destination Setup Guide

## Overview
This guide covers complete setup of Destination: installation, device-owner provisioning, permissions, DNS/VPN hardening, rule design, schedules, limits, and final lock protection.

## Prerequisites
- Android device
- Latest Destination APK
- `adb` installed on your computer
- USB debugging enabled
- A strong password

---

## Step 1: Install the APK
Download and install the latest Destination release APK.

## Step 2: Remove Accounts Temporarily
Go to:

`Settings -> Passwords & Accounts`

Remove all accounts (Google, etc.). You will re-add them after setup.

Verify no accounts remain:
```bash
adb shell dumpsys account
```

If any app still shows accounts, uninstall that app temporarily.

## Step 3: Set Device Owner
```bash
adb shell dpm set-device-owner com.ankit.destination/.admin.FocusDeviceAdminReceiver
```

## Step 4: Grant Usage Access
```bash
adb shell cmd appops set com.ankit.destination GET_USAGE_STATS allow
```

## Step 5: Grant Accessibility
```bash
adb shell settings put secure enabled_accessibility_services com.ankit.destination/com.ankit.destination.YourAccessibilityService
adb shell settings put secure accessibility_enabled 1
```

## Step 6: Finish Base Setup
Open Destination, then re-add your Google and device accounts.

---
# In app settings:

## Network Protection Setup (Choose One)

### Option A: DNS (Recommended)
1. Install NextDNS.
2. Set it up.
3. Keep the NextDNS password the same as your Destination password (harder to tamper with).
4. Setup adblocking and porn blocking and bypass blocking in nextdns, Copy your DNS link/profile endpoint.
5. Paste that DNS link into Destination.

### Option B: VPN
1. Add the package name of your VPN app in Destination.
2. Configure Destination so internet outside approved VPN/DNS apps does not work.

---

## Enable All Protection Toggles
Enable all major security restrictions, including:
- Date & time restriction
- Debugging/developer settings protection
- User creation restriction
- Other available hardening toggles in Destination

---

## Rules Configuration

### Allowlist
Put apps here that should remain usable even during strict “all apps blocked” schedules.

### Blocklist
Put apps here that should be blocked permanently. There's a advanced blocklist section as well to block forks and similar 3rd party apps so you cant block one app and install similar app to use.

### Uninstall Protection
Use this for blocker/security apps you never want removed, even if someone tries bypass methods.
If you have installed my ankiblocker app then enable this here, or if you use any other blocker then enable it here as well.

---

## Groups, Schedules, and Limits

### Group Settings
Keep **schedule groups** and **limit groups** separate for easier maintenance and cleaner management.

### Schedules
Create your blocking schedules first (focus windows, night block, etc.).

### Individual Time Limits
Then set per-app usage limits.

### Individual App Settings
Finally, apply app-level rules and exceptions.

---

## Final Security Step
1. Set your Destination password.
2. Store it in Lockey.
3. Take a backup from lockey app which is encrypted so your password is safe but not readable.
4. Forget the password.
5. Turn protection ON.

---

## Recommendations from the Creator
- Make night block a strict all-app block.
- Search ChatGPT for package names of clone/third-party clients of Instagram, Reddit, YouTube, etc.
- Add those package names to Blocklist to prevent bypass when limits are reached.
- Report any issues on GitHub.

---

## Done
Your Destination setup is now complete and hardened.

---

# Bonus (Optional): App Recommendations for a Less Addictive Experience

Blocking apps is effective, but you can also improve your digital wellbeing by changing how you use them.

The goal is to remove the most addictive, low-value features like:

- Infinite-scrolling short-form video feeds  
- Endless content  
- Useless creators  

---

## For YouTube & Instagram (Removing Shorts/Reels)

Easy way: download https://github.com/libre-tube/LibreTube and set it up so theres only susbcribed channels and no related videos in your feed and below the video player.

OR

For nerds (the hard but better way)

Consider using a tool like ReVanced Manager.

Guide:  
https://github.com/KobeW50/ReVanced-Documentation/blob/main/YT-ReVanced-Guide.md#before-you-begin

This is an application that allows you to "patch" official apps like YouTube with custom modifications.

Its most powerful feature is the ability to completely remove the "Shorts" tab from the YouTube app, allowing you to focus on intentional, long-form content.

It also allows removal of suggested content below the comment section.

Similar patches can sometimes be applied to other apps to hide features like Instagram Reels.

Use the Reel block feature of Mindful to put a time limit on scrolling.

If your attempt is to kill infinite scrolling, make sure to:

- Unfollow and unsubscribe from useless creators that create mindless content or trends  
- Support niche creators who do this for hobby and family and friends  
- Unfollow mainstream creators, influencers, meme channels, fact channels, big YouTubers like MrBeast etc.  
- Follow niche or hobby-based creators that upload maybe once a month  

### Instagram Patch Using ReVanced

Download:  
https://github.com/AbdurazaaqMohammed/AntiSplit-M  

Use it to convert the Instagram APKM bundle to APK to load in ReVanced Manager.

Enable:

- Hiding ads  
- Following-only feed  
- Hiding suggested content  
- Hide stories (Optional)  
- Hide explore page  
- Hide navigation buttons  
- Hide reels  

Next:

- Put a daily timer on reels scrolling in Mindful  https://github.com/akaMrNagar/Mindful
- Put an overall hourly and daily limit on Instagram usage in destination.

Do the same for YouTube.

For YouTube, import these in:

**Settings > ReVanced > Misc > Import**

```json
"change_start_page": "subscriptions",
"change_start_page_always": true,
"custom_filter": true,
"custom_filter_strings": "video_lockup$relatedH\nsubscriptions_channel_bar",
"disable_resuming_shorts_player": true,
"disable_signin_to_tv_popup": true,
"end_screen_suggested_video": true,
"header_logo": "premium",
"hide_album_cards": true,
"hide_artist_cards": true,
"hide_community_posts": true,
"hide_crowdfunding_box": true,
"hide_endscreen_cards": true,
"hide_filter_bar_feed_in_feed": true,
"hide_filter_bar_feed_in_related_videos": true,
"hide_filter_bar_feed_in_search": true,
"hide_for_you_shelf": true,
"hide_home_button": true,
"hide_navigation_button_labels": true,
"hide_notifications_button": true,
"hide_related_videos": true,
"hide_related_videos_overlay": true,
"hide_shorts_history": true,
"hide_shorts_home": true,
"hide_shorts_search": true,
"hide_shorts_subscriptions": true,
"hide_ticket_shelf": true,
"miniplayer_type": "minimal",
"shorts_disable_background_playback": true,
"shorts_player_type": "regular_player"
```


---

## For Reddit

Avoid the official Reddit app, which is designed for maximum engagement with video feeds and algorithmic content.

Instead, use a third-party client. like this https://play.google.com/store/apps/details?id=allen.town.focus.red&hl=en_IN

or An excellent and popular choice is Sync for Reddit. 
Guide:  
https://github.com/KobeW50/ReVanced-Documentation/blob/main/Reddit-Client-ID-Guide.md

These clients typically offer a cleaner, more text-focused interface, remove promoted posts, and give you far more control over the content you see, making for a much less addictive experience.

Use ReVanced for it and only allow viewing top posts of everyday as your default page.



## Pornography

Bulldog blocker is the only app i couldnt override, it works on all the apps and basically runs an AI that actively monitors your content (its all offline so dont worry about privacy). 

Add this into uninstall protection apps in destination rules tab.

## Student

If you are a student I have two recommendations for you. 

https://github.com/creativeidiot123/LibreTube Is a libretube fork, i have removed search icon from it so you are stuck with your subscriptions, download a normal libretube client from fdroid, subscribe to your study youtubers, then export the subscriptions and import in our fork, mark our fork as usable as unlimited apps in family link so you can study from youtube while normal youtube is blocked

AnkiBlocker

Anki is a repetition app, alot of students use it, this blocker uses it to trigger app blocks. read more here https://github.com/creativeidiot123/Blocker

Also add this into uninstall protection apps in destination rules tab.

