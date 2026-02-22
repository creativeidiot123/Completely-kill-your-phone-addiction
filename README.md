# A Comprehensive Guide to a High-Friction Digital Environment


![High Friction Setup](https://raw.githubusercontent.com/creativeidiot123/Completely-kill-your-phone-addiction/main/kill-the-access-to-new-content-and-stop-doom-scrolling-v0-ylisxrl7gj0f1%20(1).webp)

This guide outlines a robust method to lock down your device, creating significant "friction" to prevent bypassing productivity blocks. The core principle is to combine the rigid, scheduled blocking of Google Family Link with the flexible, daily management of a dedicated blocker app like Mindful.

When properly implemented, this system is extremely resilient and designed to withstand nearly all common bypass attempts, including booting into Safe Mode, changing the device time, or uninstalling key applications without authorization from the Parent Account.

---

## Phase 1: Preparation and Account Creation

This phase is best performed on a PC for ease of copying and pasting complex passwords.

### Download Initial Apps

On your phone download:

- **Mindful** (You will configure app blocking with this later).  
  https://github.com/akaMrNagar/Mindful  

- **The specified Blocker App:**  
  https://github.com/creativeidiot123/Lockey/releases  
  This will be used to store your emergency password.

### Create the "Parent" Account

Open a web browser and create a brand new Google Account. This account will act as the administrator or "Parent" for your device.

Do not save that password in any password manager or your browser's autosave feature, and do not add any phone number or recovery emails to this new mail.

Generate a highly complex and random password. It should be impossible to memorize.

Example:


### Secure and "Forget" the Password

**Crucial Step:** You must not have easy access to this password.

Entrust it to a reliable person (like a family member or trusted friend). Send it to them and then delete all records of it from your own devices and message history. The goal is that you cannot retrieve it on your own.

Put it in the Lockey app provided above, and put a 350 character protection minimum.

### Enable Two-Factor Authentication (2FA)

On your phone, download and set up Google Authenticator.

In the settings for your new "Parent" account, enable 2FA and link it to any Authenticator app on your phone. This adds a critical layer of security to the parent account so you cannot just login to any other device with it.

---

## Phase 2: Linking Your Device with Family Link

Now, you will configure your phone so that the new "Parent" account supervises your primary account.

### Enable Parental Controls

Go to your phone's:

**Settings > Digital Wellbeing & parental controls**

Select the option to set up parental controls.

### Assign Roles

When prompted, designate your phone as a Child's device.

Your primary, day-to-day Google account will now be the Child Account.

Follow the on-screen instructions to link it to the Parent Account you created in Phase 1. You will need to sign in with the Parent Account's credentials one time for this setup.

### Note on Multiple Email Accounts

Since your device will now be locked to a single primary Google Account, the Gmail app will only show emails for that account.

To manage emails from your other accounts, you will need to download a third-party email client (such as K-9 Mail or FairEmail) from the Play Store.

If you have any third party apps, either convert them to email and password accounts or login before removing those accounts.

---

## Phase 3: Configuring Parent Account Permissions

Log in to the Google Family Link website using your Parent Account credentials. Select your device from the dashboard to manage its settings.

The strategy here is to use Family Link for its most rigid features, while leaving flexible blocking to other apps.

### Content Restrictions

Set everything to "Allow all." This includes app installations, websites, etc.

### Device Settings to Block  
(Available in device settings in Family Link on the Parent side)

- Block Developer Options  
  This is critical to prevent bypasses using ADB (Android Debug Bridge).

- Disable Changes to Time & Date  
  Prevents manipulating time to get around time-based limits.

- Enable "Allow installation from unknown sources"  
  This allows you to sideload apps if needed.

---

## Configure Downtime (For Night Blocks)

It is recommended to use Family Link's Downtime feature only for a strict night-time block (e.g., 10 PM to 7 AM).

Enable a schedule for these hours.

By default, all apps will be blocked during Downtime.

Go through the app list and mark only the absolute essentials (like Phone, Messages, Maps, Uber, Payment, Clock) as "Always Allowed."

Leave all other apps in their default, restricted state.

Crucially, this includes:

- Browsers  
- Social media  
- The Blocker App holding your password  
- Your 2FA app (e.g., Google Authenticator)

Blocking these last two prevents any attempts to access the Parent Account and disable the system during the block.

---

## App Time Limits

While Family Link offers app time limits, we will use Mindful for this purpose instead.

Mindful is less rigid and better for daily management with its emergency usage and upcoming session block features.

However, if you want daily time limits in a rigid way then use Family Link's daily app time limits.

---

## Phase 4: The Final Lock-In

This phase makes the system difficult to undo.

### Secure the Parent Password

Open the Blocker App you downloaded earlier.

Copy and paste the long, complex Parent Account password into this app.

Set the app's unlock mechanism to something extremely time-consuming, such as requiring a 300 to 400 character phrase to be typed perfectly.

This ensures that accessing the password in an emergency is a deliberate 10 to 20 minute process.

### Sign Out Everywhere

On your PC and any other device, sign out of the Parent Account.

Do not save the password in any browser or password manager.

The only place this password should now exist is with your trusted person and inside the heavily locked Blocker App on your phone.

If you delete the locker app by accident your password is gone.

---

## Set Up Mindful for Daily Management

Now, open the Mindful app.

It is highly recommended for:

- Daily App Time Limits (e.g., 1 hour of social media per day)  
- Session Blocks for focused work or study periods  

Use Mindful's features for your flexible, day-to-day productivity needs.

Enable its strictness features so you cannot uninstall it.

Your system is now complete.

Family Link provides the unbreakable, foundational rules for night-time, while Mindful provides the flexible limits and blocks needed for daytime productivity.

---

# Bonus (Optional): App Recommendations for a Less Addictive Experience

Blocking apps is effective, but you can also improve your digital wellbeing by changing how you use them.

The goal is to remove the most addictive, low-value features like:

- Infinite-scrolling short-form video feeds  
- Endless content  
- Useless creators  

---

## For YouTube & Instagram (Removing Shorts/Reels)

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

- Put a daily timer on reels scrolling in Mindful  
- Put an overall timer on Instagram usage in Family Link  

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

Instead, use a third-party client.

An excellent and popular choice is Sync for Reddit.

These clients typically offer a cleaner, more text-focused interface, remove promoted posts, and give you far more control over the content you see, making for a much less addictive experience.

Use ReVanced for it and only allow viewing top posts of everyday as your default page.

Guide:  
https://github.com/KobeW50/ReVanced-Documentation/blob/main/Reddit-Client-ID-Guide.md


## Pornography

Bulldog blocker is the only app i couldnt override, it works on all the apps and basically runs an AI that actively monitors your content (its all offline so dont worry about privacy).
