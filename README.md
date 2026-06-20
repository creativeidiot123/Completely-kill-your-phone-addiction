# Nuke your Social Media and Pornography usage.


![High Friction Setup](https://raw.githubusercontent.com/creativeidiot123/Completely-kill-your-phone-addiction/main/kill-the-access-to-new-content-and-stop-doom-scrolling-v0-ylisxrl7gj0f1%20(1).webp)

pp Recommendations for a Less Addictive Experience

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


If your attempt is to kill infinite scrolling, make sure to:

- Unfollow and unsubscribe from useless creators that create mindless content or trends  
- Support niche creators who do this for hobby and family and friends  
- Unfollow mainstream creators, influencers, meme channels, fact channels, big YouTubers like MrBeast etc.  
- Follow niche or hobby-based creators that upload maybe once a month  


### Instagram Patch Using ReVanced

Easy way: download InstaPrime https://t.me/InstaPrimeOfficials and set it up so theres only followed pages and Hiding suggested content, Hide reels, disable Scrolling in reels is enabled.

OR

For nerds (the hard but better way)

Download:  
https://github.com/AbdurazaaqMohammed/AntiSplit-M  
Guide:  
https://github.com/KobeW50/ReVanced-Documentation/blob/main/YT-ReVanced-Guide.md#before-you-begin

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

---

## For Reddit

Avoid the official Reddit app, which is designed for maximum engagement with video feeds and algorithmic content.

Instead, use a third-party client. like this https://play.google.com/store/apps/details?id=allen.town.focus.red&hl=en_IN or Infinity+ or redreader

Hard way for nerds:
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

https://github.com/creativeidiot123/LibreTube Is a libretube fork, i have removed search icon from it so you are stuck with your subscriptions, download a normal libretube client from fdroid, subscribe to your study youtubers, then export the subscriptions and import in our fork, mark our fork as usable as allowed apps in destination so you can study from youtube while normal youtube is blocked

AnkiBlocker

Anki is a repetition app, alot of students use it, this blocker uses it to trigger app blocks. read more here https://github.com/creativeidiot123/Blocker

Also add this into uninstall protection apps in destination rules tab.

