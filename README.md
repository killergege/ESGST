# ESGST - Enhanced SteamGifts & SteamTrades

A script that adds some cool features to SteamGifts and SteamTrades.

---

## [Patrons](https://www.patreon.com/revilheart) - Thank you!

* [Pilda](https://www.steamgifts.com/user/Pilda)

---

## Installation

To install the extension:

* Firefox -> Download [this file](https://github.com/revilheart/ESGST/raw/master/Extension/esgst.xpi) and drag it into "about:addons".
* Chrome -> Download [this zip](https://github.com/revilheart/ESGST/archive/master.zip), extract it to a folder on your computer, go to "chrome://extensions/", tick "Developer mode" in the top right corner, click "Load unpacked extension" and select the "Extensions" folder where you extracted the zip to. Using the extension on Chrome might be a nuisance, since every time you open the browser you will get a message saying that using extensions in developer mode can be unsafe, and every time a new version is released you will have to download the zip again, extract it to the same folder, replacing the previous files, go to the extensions page and click "Reload" under ESGST.

Other browsers might work with the extension, but only Firefox and Chrome have been tested and confirmed as working.

To install the script, you must install [Greasemonkey](http://www.greasespot.net/) (not 100% compatible with the latest versions of Firefox), [Tampermonkey](https://tampermonkey.net/), or some other userscript manager first. Then [click here](https://github.com/revilheart/ESGST/raw/master/ESGST.user.js) and you should be prompted to install it.

You can also install the script in your Android through Firefox with Violentmonkey or USI. Though some features might not work.

To upgrade from the script to the extension, all you have to do is export all your data from the script, install the extension and import all the data you had exported into the extension.

---

## Compatibility

Fully tested and working in the latest version of:

* Firefox
* Google Chrome

Should be working in the latest version of:

* Opera

May or may not be working (try at your own risk) in the latest version of:

* Edge

---

# Features

---

## General

* [Fixed Elements](#fixed-elements)
* [Endless Scrolling](#endless-scrolling)
* [Grid View](#grid-view)
* [Header Icons Refresher](#header-icons-refresher)
* [Accurate Timestamp](#accurate-timestamp)
* [Points Refresher](#points-refresher)
* [Visible Attached Images](#visible-attached-images)

---

## Giveaways

* [Giveaway Templates](#giveaway-templates)
* [Stickied Giveaway Groups](#stickied-giveaway-groups)
* [Advanced Giveaway Search](#advanced-giveaway-search)
* [Pinned Giveaways Button](#pinned-giveaways-button)
* [Giveaway Filters](#giveaway-filters)
* [Entered Giveaways Filter](#entered-giveaways-filter)
* [Enter / Leave Giveaway Button](#enter--leave-giveaway-button)
* [Giveaway Description / Comment Box Popup](#giveaway-description--comment-box-popup)
* [Giveaway Winning Chance](#giveaway-winning-chance)
* [Giveaway Groups Popup](#giveaway-groups-popup)
* [Giveaway Winners Link](#giveaway-winners-link)
* [Giveaway Error Search Links](#giveaway-error-search-links)
* [Delivered Gifts Notifier](#delivered-gifts-notifier)
* [Unsent Gifts Sender](#unsent-gifts-sender)
* [Entries Remover](#entries-remover)

---

## Discussions

* [Active Discussions On Top](#active-discussions-on-top)
* [Discussions Highlighter](#discussions-highlighter)
* [Main Post Popup](#main-post-popup)
* [Discussion Edit Detector](#discussion-edit-detector)

---

## Commenting

* [Comment History](#comment-history)
* [Comment Tracker](#comment-tracker)
* [Comment Formatting Helper](#comment-formatting-helper)
* [Main Comment Box Popup](#main-comment-box-popup)
* [Multi-Reply](#multi-reply)
* [Reply From Inbox](#reply-from-inbox)
* [Reply Mention Link](#reply-mention-link)

---

## Users, Groups & Games

* [Username History](#username-history)
* [Permanent User Notes](#permanent-user-notes)
* [Real Won / Sent CV Links](#real-won--sent-cv-links)
* [Sent / Won Ratio](#sent--won-ratio)
* [SteamGifts Profile Button](#steamgifts-profile-button)
* [SteamTrades Profile Button](#steamtrades-profile-button)
* [Shared Groups Checker](#shared-groups-checker)
* [Permanent User Tags](#permanent-user-tags)
* [Whitelist / Blacklist Highlighter](#whitelist--blacklist-highlighter)
* [Whitelist / Blacklist Checker](#whitelist--blacklist-checker)
* [Not Activated / Multiple Wins Checker](#not-activated--multiple-wins-checker)
* [Not Received Finder](#not-received-finder)
* [User Giveaways Data](#user-giveaways-data)
* [Inbox Winners Highlighter](#inbox-winners-highlighter)
* [Avatar Popout](#avatar-popout)
* [Game Categories](#game-categories)

---

## Games

* [Entered Games Highlighter](#entered-games-highlighter)
* [Game Tags](#game-tags)

---

## Other

* [Featured Container Hider](#featured-container-hider)
* [Blacklist Stats Hider](#blacklist-stats-hider)
* [Multi-Tag](#multi-tag)
* [Groups Highlighter](#groups-highlighter)
* [Groups Stats](#groups-stats)
* [Archive Searcher](#archive-searcher)

---

* [Other Info](#other-info)

---

### Unfaded Entered Giveaways

`steamgifts.com/*`

* Removes SG's default fade for entered giveaways.

### Created/Entered/Won Giveaway Details

`steamgifts.com/giveaways/(created|entered|won)/*`

* Adds more details to the created/entered/won pages, such as the number of points, the link to the Steam store page of the game, the name of the creator, the type of the giveaway and the level. It also loads the giveaway groups below the giveaway if Giveaway Groups Loader is enabled.

### Is There Any Deal? Info

`steamgifts.com/giveaway/*`

* Adds Is There Any Deal? info to giveaway pages, including the best current deal, the historical lowest price (optional) and the list of bundles that the game has been in, with a cache that can be updated after 24 hours since the last check.

![](http://i.imgur.com/epF2am3.png)

### Last Page Link

`steamgifts.com/*`

* Adds a "Last Page" link to some places that are missing it, for example: discussion pages with 100+ pages, user pages, group pages with 100+ pages.

### Giveaway Maker

`steamgifts.com/giveaways/new/*`

* Allows you to create multiple giveaways or a train of giveaways (multiple giveaways that are linked to one another).
* You can view detailed information about a giveaway by hovering over it.
* You can re-order/remove the giveaways by dragging and dropping them in the correspondent areas.
* All giveaways will be created without reviewing or validating, so make sure all fields are filled correctly, or the giveaway creation will fail (if a train is being created, the failed giveaway will be disconnected and the previous giveaway will be connected to the next instead).

![](http://i.imgur.com/Pf9j7gN.png)

### Discussions Sorter

`steamgifts.com/discussions/*`

* Allows you to sort discussions by creation date (from newest to oldest).

![](http://i.imgur.com/pMAoVq9.png)

### Whitelist/Blacklist Sorter

`steamgifts.com/account/manage/whitelist|blacklist/*`

* Allows you to view your whitelist/blacklist sorted by added date, both from oldest to newest and from newest to oldest.

![](http://i.imgur.com/Vyr1LWi.png)

### Steam Activation Link

`steamgifts.com/giveaways/won*`

* Allows you to easily activate a won game.

![](http://i.imgur.com/0hnY0yD.png)

### User Filters

`steamgifts.com/*`

* Allows you to filter out posts, discussions and giveaways from users.
* Filtered posts are completely removed, along with all replies to it.
* Each user has their own settings, which can be configured through their profile (or their avatar if you're using Avatar Popout).
* You can enable an option in the settings menu to automatically filter out all users that you have blacklisted. If you set a custom setting to a blacklisted user on their profile, that setting will overwrite the automatic setting.
* You can see a list of filtered users in the settings menu.

### Giveaway Bookmarks

`steamgifts.com/*`

* Allows you to bookmark giveaways to enter later.
* You can enable an option to highlight the button if a giveaway is about to end, given a certain amount of hours specified in the settings menu.
* Giveaways that have not started yet will not appear in the list of bookmarked giveaways. Instead, they will stay in a sort of hidden state until they start. When they start, the header bookmark button will turn green, indicating that you must open the list of bookmarked giveaways so that the started giveaways can be updated with their end times. When giveaways are about to end, the button will red. If there are both started and ending giveaways, the button will be colored with a brown-ish color. Hovering over the button also gives you more details about how many giveaways have started and/or are ending.

![](http://i.imgur.com/6e8UyL3.png)
![](http://i.imgur.com/kNxEDZV.png)
![](http://i.imgur.com/7OAYXa9.png)

### Quick Giveaway Browsing

`steamgifts.com/*`

* Allows you to quickly go to recommended/wishlist/group/new giveaways without having to first go to the main page and then select it at the sidebar.

![](http://imgur.com/NDgqzFj.png)

### Game Categories

`steamgifts.com/*`

* Displays categories for games. Categories so far: bundled, trading cards, achievements, multiplayer, Steam cloud, Linux, Mac, DLC and genres.
* The bundle list must be synced through the settings menu for the bundled category to work.

![](http://i.imgur.com/DmYIM2V.png)
![](http://i.imgur.com/70Gyhxu.png)
![](http://i.imgur.com/jsL0aVB.png)
![](http://i.imgur.com/zGeKiag.png)

### Giveaway Filters

`steamgifts.com/giveaways/*`

* Allows you to filter out certain giveaways in a page.
* Works well with Game Categories.

![](http://i.imgur.com/Ez4NyMm.png)

### Real CV Calculator

`steamgifts.com/giveaway/new`

* Calculates how much real CV you should get for a giveaway.
* It's only accurate if you have synced the bundle list from the settings menu and also scanned your sent giveaways using User Giveaways Data. But even then, it's only 100% accurate if the user has 0 not received giveaways, since User Giveaways Data doesn't currently know if the giveaways have been received or not.
* In the example below, as I had previously given away 3 copies of Max Payne 3, the sixth copy is worth 10% less (18P). So the 3 new copies would equal 58P:

![](http://i.imgur.com/oCGStUq.png)

### Giveaway Encrypter/Decrypted

`steamgifts.com/*`

* Allows users of the script to encrypt giveaways and hide them in their posts, so that they can be easily seen by other users of the script.
* To add encrypt a giveaway and hide it in a post, you must have the option enabled for Comment Formatting Helper.
* If there are any encrypted giveaways hidden in a page, a button will be added to the header menu where you can access them.

### Settings Menu

`steamgifts.com/account/*`

* Allows you to enable / disable features.
* Allows you import / export your data.
* Allows you to manage `Whitelist / Blacklist Highlighter` and `Not Activated / Multiple Wins Checker` caches.
* Allows you to sync your data and enable / disable the automatic sync.

### Level Progress Visualizer

`steamgifts.com/*`

* Shows your level progress in the main button.

![](http://imgur.com/RJmCnpR.png)

### Hidden Featured Container

`steamgifts.com/giveaways/*`

![](http://i.imgur.com/QjTxvo2.png)

* Hides the featured container in the giveaways pages.

### Hidden Blacklist Stats

`steamgifts.com/stats/personal/community`

![](http://i.imgur.com/yB3pQSI.png)

* Hides blacklist stats in the stats page.

### Fixed Header
### Fixed Sidebar
### Fixed Main Page Heading
### Fixed Footer

`(steamgifts|steamtrades).com/*`

* Allows you to fix the header, heading, sidebar and footer, so that they scroll together with the page.
* You can disable any of the elements through the settings menu.
* In case it isn't clear, this is the heading:

![](http://i.imgur.com/6Hk0nus.png)

### Endless Scrolling

`(steamgifts|steamtrades).com/*`

![](http://i.imgur.com/sCJ97Dk.png)

* Allows you to endlessly scroll through pages.
* You can choose in which pages you want to enable the endless scrolling from the settings menu.
* If you click on the link to a page and that page is currently loaded, it will jump to the page instead of loading it. This only works on SteamGifts though, and if you jump between pages that aren't next to each other, the pagination gets messed up, but you can fix it by then going to the immediate previous / next page and returning.
* You can refresh pages without leaving the page.
* You can pause / resume the endless scrolling.
* You can enable reverse scrolling for discussions.

### Active Discussions On Top/Sidebar

`steamgifts.com/*`

* Moves the active discussions to the top/sidebar of the page.
* More info about the sidebar choice: if you have Advanced Giveaway Search enabled, it will be hidden and triggered when hovering hover the search field; the username and avatar of the user who last posted will be removed (the button to go to the last comment will remain intact); Accurate Timestamps will not run for any timestamps inside the active discussions; and any user tags you might have saved for users will be hidden inside the active discussions (they will still be visible if you click the tag button to edit them).

![](http://i.imgur.com/XEeroVn.png)

### Grid View

`steamgifts.com/giveaways*`

![](http://i.imgur.com/jhd1m4A.png)

### SteamGifts Profile Button

`steamtrades.com/user/*`

![](http://i.imgur.com/k4P3OMy.png)

* Adds a button that links to an user's SteamGifts profile.

### SteamTrades Profile Button

`steamgifts.com/user/*`

![](http://i.imgur.com/iJxVz6D.png)

* Adds a button that links to an user's SteamTrades profile.

### Shared Groups Checker

`steamgifts.com\/*`

![](http://i.imgur.com/5NkCrum.png)

* Allows you to check which groups you and another user have in common.

### Comment History

`steamgifts.com/*`

![](http://i.imgur.com/lDSXYcS.png)

* Keeps track of the comments you make (they can be seen from the settings menu).
* This feature **only** works with Main Comment Box Popup, Discussion Edit Detector and Multi-Reply / Reply From Inbox. If you submit a comment though SG's native comment box, the comment will not be tracked.

### Username History

`steamgifts.com/user/*`

![](http://i.imgur.com/cTnt7sk.png)

* Keeps track of usernames from the [database](https://docs.google.com/spreadsheets/d/1rZQuo6T02zutwSo1edbDzW8q9GmpDIbaVvKN79TyFqA/edit?usp=sharing) and detects username changes every month.
* There are currently 7200+ users being tracked.
* An user is added to the database when you click on the arrow next to their username.
* You can view recent username changes from the settings menu.

### User Notes

`(steamgifts|steamtrades).com/user/*`

![](http://i.imgur.com/lF9YKjm.png)
![](http://i.imgur.com/1AvN0Co.png)

* Allows you to add notes to users.
* The notes are permanent because they are tied to an user's SteamID64 instead of their username.
* The icon changes if the notes are not empty:

![](http://i.imgur.com/PYm3Ds7.png)

### User Tags

`(steamgifts|steamtrades).com/*`

![](http://i.imgur.com/AIPs4d1.png)
![](http://i.imgur.com/4660IaT.png)

* Allows you to add tags to users.
* Unlike the permanent user notes, the tags are not tied to an user's SteamID64, because that information is only available in the profile page, but they are still permament because upon adding a tag to an user, it automatically detects username changes and returns any old tags you might have saved for that user before they changed their username.
* While the tags are not tied to an user's SteamID64, it still has to retrieve the user's profile page in order to save to the storage, so if you're adding tags to an user for the first time, it might take a while to do so.
* Separation of tags is purely cosmetic.

### Multi-Tag

`(steamgifts|steamtrades).com/*`

![](http://i.imgur.com/aZRQkxr.png)
![](http://i.imgur.com/mhjTmn1.png)

* Allows you to tag multiple users / games at the same time.
* It goes without saying that this feature only works if either Permanent User Notes or Game Tags are enabled.

### Whitelist/Blacklist Highlighter

`(steamgifts|steamtrades).com/*`

![](http://i.imgur.com/rxqGu9i.png)
![](http://i.imgur.com/mRIrwb7.png)

* Adds a heart or ban icon next to the username of all users from your whitelist / blacklist.
* The users must be scanned through the settings menu for the feature to work. You can scan them manually or enable the automatic scan to run every once in a while.

### Whitelist/Blacklist Checker

`steamgifts.com/*`

![](http://i.imgur.com/KDAHDme.png)
![](http://i.imgur.com/x6AWyp7.png)

* Allows you to check if an user or a list of users have whitelisted / blacklisted you.
* Results are cached for 24 hours.
* The caches can be seen and updated from the settings menu.
* The checker has a simplified version that only checks / shows whitelists. It can be activated from the settings menu by enabling `Show blacklist information.`. If this version is activated and the checker finds an user that has blacklisted you, it will return `There is not enough information to know if you are whitelisted or blacklisted.` instead of `You are blacklisted.`.
* You can highlight users who have whitelisted / blacklisted you by enabling this option through the settings menu. This functionality is supported on SteamTrades (`steamtrades.com/*`). The following icons will be added next to their username:

![](http://i.imgur.com/yPoDrnm.png)
![](http://i.imgur.com/BRLSAXD.png)

### Real Won/Sent CV Links

`steamgifts.com/user/*`

![](http://i.imgur.com/NvGf47L.png)
![](http://i.imgur.com/Shwsgdh.png)

* Adds links to an user's SGTools real won / sent CV pages.
* Has an option to automatically load the real CV and show it on the profile.

### Sent/Won Ratio

`steamgifts.com/user/*`

![](http://i.imgur.com/eqBybQQ.png)

* Shows the sent / won ratio of an user.

### Not Activated/Multiple Wins Checker

`steamgifts.com/(user|giveaway/.../winners)/*`

![](http://i.imgur.com/QsNfLPJ.png)
![](http://i.imgur.com/vaSRuPJ.png)
![](http://i.imgur.com/nBeDvPw.png)

* Allows you to check if an user or a page of winners from a giveaway have any not activated / multiple wins.
* Results are cached for 7 days.
* The caches can be seen from the settings menu (updating all of them at once is not possible).
* You can highlight users who have not received / multiple wins by enabling this option through the settings menu. This functionality is supported on SteamTrades (`steamtrades.com/*`). Their username will change to the following colors:

![](http://i.imgur.com/6Oo1Bkg.png)
![](http://i.imgur.com/IH9khSq.png)

### Not Received Finder

`steamgifts.com/user/*`

![](http://i.imgur.com/lgjr9mo.png)
![](http://i.imgur.com/8AXpAd2.png)

* Allows you to find an user's not received giveaways.
* If the user doesn't have any not received giveaways, the button will not appear.
* Results are cached for 7 days.

### User Giveaways Data

![](http://i.imgur.com/1ZeyWtw.png)
![](http://i.imgur.com/Vq0Toc1.png)
![](http://i.imgur.com/q3xqDym.png)

* Gathers data about an user's giveaways, listing them by type and level.
* Lists the most given away games for sent checks and the users most won from for won checks.
* The data is not 100% accurate if the user has not received giveaways.

### Level Up Calculator

`steamgifts.com/user/*`

![](http://i.imgur.com/eTBR402.png)

* Approximately calculates how much real CV an user needs to level up.

### Inbox Winners Highlighter

`steamgifts.com/messages`

![](http://i.imgur.com/l5IeKoHg.png)

* Highlights the winners of your giveaways in your inbox.
* A winner is added to the storage when you send the gift to them through the winners page of the giveaway or through Unsent Gifts Sender.

### Avatar Popout

`steamgifts.com/*`

![](http://i.imgur.com/aEEKnim.png)
![](http://i.imgur.com/o8os3un.png)

* Pops out a box with info about an user / group if you click on their avatar.
* Has all the features that run on `steamgifts.com/user/*` built-in.

### Unsent Gifts Sender

`steamgifts.com/created/*`

![](http://i.imgur.com/IXgP9G0.png)
![](http://i.imgur.com/69wbkUP.png)

* Allows you to send all your unsent gifts directly from your created giveaways page.
* You can choose to only send the gifts to winners with 0 not activated / multiple wins or who are whitelisted.

### Entries Remover

`steamgifts.com/giveaways/entered/*`

![](http://i.imgur.com/kXTZeWo.png)

* Allows you to remove entries for owned games.
* In order for the feature to work, you must enter your Steam API Key in section 9 of the settings menu (get a Steam API Key [here](https://steamcommunity.com/dev/apikey)):

![](http://i.imgur.com/MK5cVax.png)

### Giveaway Templates

`steamgifts.com/giveaways/new`

![](http://i.imgur.com/yl9ogWx.png)
![](http://i.imgur.com/PFML0cc.png)

* Allows you to save giveaway templates for later use.
* To edit a template, simply apply it normally, perform your changes and save it with the same name.

### Stickied Giveaway Groups

`steamgifts.com/giveaways/new`

![](http://i.imgur.com/5QeKO7e.png)

* Allows you to sticky groups while creating a giveaway.

### Header Icons Refresher

`steamgifts.com/*`

* Updates the header icons every 60 seconds (only if the tab is active).
* You can enable an option that runs the refresher in the background and changes the icon of the tab when not active.

### Delivered Gifts Notifier

`steamgifts.com/*`

![](http://i.imgur.com/z4EZZm6.png)

* Notifies you if one of your won gifts has been delivered.

### Advanced Giveaway Search

`steamgifts.com/giveaways/*(!(wishlist|created|entered|won)`

![](http://i.imgur.com/RHYmAGs.png)

* Allows you to easily search giveaways using SG's [search parameters](https://www.steamgifts.com/discussion/8SzdT/).

### Pinned Giveaways Button

`steamgifts.com/giveaways/*`

![](http://i.imgur.com/oiXdLx3.png)

* Allows you to collapse the pinned giveaways container after expanding it.

### Points Refresher

`steamgifts.com/?`

* Updates your points every 60 seconds (only if the tab is active).
* You can enable an option that runs the refresher in the background and changes the title of the tab when not active.

### Visible Attached Images

`(steamgifts|steamtrades).com/*`

![](http://i.imgur.com/IoZ7JhK.png)

* Shows all attached images by default.

### Games Highlighter

`steamgifts.com/*`

![](http://i.imgur.com/gblD658.png)

* Highlights games you have already entered giveaways for.

### Giveaway Panel
### Entered Giveaways Filter

`steamgifts.com/*`

* Hides entered giveaways.

### Enter/Leave Giveaway Button

`steamgifts.com/(giveaways|user|group)/*`

![](http://i.imgur.com/dR5gyHW.png)

* Allows you to enter / leave giveaways directly from the giveaways pages.

### Giveaway Description/Reply Box Popup

`steamgifts.com/(giveaways|user|group)/*`

![](http://i.imgur.com/6HJTICj.png)

* Allows you to view giveaway descriptions and add comments to giveaways directly from the giveaways pages.
* You can enable an option to show it automatically upon entering a giveaway if Enter / Leave Giveaway Button is enabled.

### Giveaway Winning Chance

`steamgifts.com/(giveaways|giveaways/entered|giveaway|user|group)/*`

![](http://i.imgur.com/Pib5Tom.png)

* Displays your winning chance for a giveaway.

### Groups Highlighter

`steamgifts.com/giveaway/groups/*`

![](http://i.imgur.com/eaGeLUj.png)

* Highlights which groups you are a member of in the giveaway groups page.

### Groups Stats

`steamgifts.com/account/steam/groups/*`

![](http://i.imgur.com/b7jV7Gu.png?1)

* Shows your status in groups from your groups page.

### One-Click Hide Giveaway Button

`steamgifts.com/*`

* Allows you to hide giveaways with one click.

### Giveaway Groups Loader

`steamgifts.com/*`

![](http://i.imgur.com/PN73phv.png)

* Loads the groups of a giveaway and shows them below it.
* Groups that you are a member of are highlighted in bold.

### Giveaway Error Search Links

`steamgifts.com/giveaway/*`

![](http://i.imgur.com/GM6bX3s.png)

* Provides search links for the game when you cannot access a giveaway.

### Discussions Highlighter

`steamgifts.com/discussions/*`

![](http://i.imgur.com/A2o14yw.png)

* Allows you to highlight discussions.

### Comment Tracker

`(steamgifts|steamtrades).com/*(!messages)`

![](http://i.imgur.com/6nALh8y.png)

* Fades out giveaways / discussions / support tickets / trades you have already visited. Note that this does not mean every comment inside the page has been read, it simply means you have visited it.
* Keeps track of comments / editions and fades out those you have already read.
* To mark a comment as read, click on the eye icon below it:

![](http://i.imgur.com/UCb55vi.png)

* Adds a panel that allows you to go to the first unread comment of the page or mark all comments of the page as read:

![](http://i.imgur.com/8fPMwjG.png)

* Keeps track of discussion comments and shows how many comments are unread on the discussions page.
* Allows you to go to the first unread comment of a discussion or mark all its comments as read directly from the discussions page.

### Accurate Timestamps

`(steamgifts|steamtrades).com/*`

* Increases the accuracy of timestamps by changing them from `2 hours ago` to `1/1/2017, 0:00:00 AM - 2 hours ago`.
* You can disable it in the main giveaways pages through the settings menu.

### Comment Formatting Helper

`(steamgifts|steamtrades).com/*`

![](http://i.imgur.com/g9C3e0g.png)

* Adds a panel that helps you with comment formatting.
* Allows you to turn automatic links / images paste formatting on / off.
* You can disable any items of the panel through the settings menu, except for the automatic links / images paste formatting item.

### Reply Box Popup

`(steamgifts|steamtrades).com/*`

![](http://i.imgur.com/hmaZQYn.png)
![](http://i.imgur.com/ClGzBNS.png)

* Hides the main comment box and adds a button that pops up a box which allows you to add comments to the page.
* Has `Discussion Edit Detector` built-in.

### Multi-Reply

`(steamgifts|steamtrades).com/*`

* Allows you to reply to multiple comments at the same time, since each comment has their own comment box and the page isn't reloaded after submitting it.
* Has `Discussion Edit Detector` built-in.

### Reply From Inbox

`(steamgifts|steamtrades).com/messages/*`

* Allows you to reply to your messages directly from your inbox.
* Has `Multi-Reply` built-in.

### Game Tags

`steamgifts.com/*`

![](http://i.imgur.com/qCLDa2g.png)
![](http://i.imgur.com/g4pTzCe.png)

* Allows you to add tags to games.
* Separation of tags is purely cosmetic.

### Giveaway Winners Link

`steamgifts.com/*`

![](http://i.imgur.com/g2kaFD9.png)

* Adds a link to the winners page of a giveaway.

### Main Post Popup

`steamgifts.com/discussion/*`

![](http://i.imgur.com/lA9QNLM.png)

* Hides the main post and adds a button that pops it up.
* If `Comment Tracker` is enabled, the main post is only hidden if it has been marked as read.

### Discussion Edit Detector

`steamgifts.com/discussion/*`

* Detects if the discussion you're posting a comment to has been edited since the time you opened it and saves your comment correctly.
* This fixes a bug on SteamGifts that does not save your comment to a discussion if you submit it after the discussion has been edited.

### Reply Mention Link

`(steamgifts|steamtrades).com/*`

![](http://i.imgur.com/SgEzjXC.png)

* Adds a mention link to the comment replied to.

### Archive Searcher

`steamgifts.com/archive/*`

![](http://i.imgur.com/DtvFj5J.png)
![](http://i.imgur.com/bkUPFuV.png)

* Allows you to search the archive by exact title / AppID.

### Embedded Videos

`steamgifts|steamtrades.com*`

* Embeds YouTube and Vimeo videos into the page.
* Videos are only embedded if the links are in the format [URL](URL) and the only content in a line.

For example:

[https://www.youtube.com/watch?v=cD1e0BNNifk](https://www.youtube.com/watch?v=cD1e0BNNifk)

The video above gets embedded.

[Orange Sphincter To The Rescue](https://www.youtube.com/watch?v=cD1e0BNNifk)

The video above does not get embedded.

I watched [https://www.youtube.com/watch?v=cD1e0BNNifk](https://www.youtube.com/watch?v=cD1e0BNNifk) and it was hilarious.

The video above does not get embedded.

### Pagination Navigation On Top

`steamgifts|steamtrades.com*`

* Moves the pagination navigation to the top of the page.

### Reply Box On Top

`steamgifts|steamtrades.com*`

* Moves the reply box to the top of the page.

### Other Info

* All requests from `Whitelist / Blacklist Checker`, `Not Activated / Multiple Wins Checker`, `Not Received Finder` and `Archive Searcher` are limited to 2 per second, to prevent a stress on the SG servers.
* If you try to leave the page while `Whitelist / Blacklist Checker`, `Not Activated / Multiple Wins Checker`, `Not Received Finder` and `Archive Searcher` are running, you will get a confirmation dialog asking you if you want to leave the page. Additionally, while these features are running, their buttons are faded out.
* `Whitelist / Blacklist Checker`, `Not Activated / Multiple Wins Checker`, `Not Received Finder` and `Archive Searcher` allow for real-time options. For example, if you start `Whitelist / Blacklist Checker` with `Also check for whitelist.` enabled, but in the middle of the process you decide to disable that option, from that point onwards it will no longer check for whitelist.

---

## Changelog

**7.9.1 (November 26, 2017):**

<ul>
    <li><a href="https://github.com/revilheart/ESGST/issues/261">#261</a> Fix a bug that does not load the entire changelog</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/260">#260</a> Fix a bug in Avatar Popout that does not load for some users</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/262">#262</a> Fix a style issue in Giveaway/Discussion Filters</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/263">#263</a> Fix a bug that does not load Entered Games Highlighter and Game Tags in popups</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/264">#264</a> Reduce useless space in popups</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/265">#265</a> Fix a bug in Scroll To Bottom Button that does not scroll all the way down with Endless Scrolling</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/266">#266</a> Fix a bug that happens when filtering features in the settings menu</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/267">#267</a> Automatically expand sections when filtering features in the settings menu</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/268">#268</a> Add option to show Scroll To Top/Bottom Button in the main page heading</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/269">#269</a> More changes to Attached Images Carousel</li>
</ul>

**7.9.0 (November 24, 2017):**

<ul>
    <li><a href="https://github.com/revilheart/ESGST/issues/224">#224</a> Also trigger reverse scrolling from the main and inbox pages in Endless Scrolling</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/225">#225</a> Fix a bug that does not allow adding a second reply to a comment without refreshing the page in Multi-Reply/Reply From Inbox</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/226">#226</a> Open the authentication window for Dropbox, Google Drive and OneDrive in a small window instead of in a new tab</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/227">#227</a> Only show button to add description to filters if the option to filter useless descriptions is enabled in Enter/Leave Giveaway Button</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/228">#228</a> Add ratio filter to Giveaway Filters</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/229">#229</a> Make some changes to the structure of the code</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/230">#230</a> Fix a bug that happens when syncing from the account page</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/232">#232</a> Make some optimizations</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/236">#236</a> Remove sync button after the sync is complete when syncing through the account page</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/237">#237</a> Prevent sync results from duplicating when clicking on the sync button again</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/238">#238</a> Fix a bug that sometimes does not detect if the user is logged in to Steam in when syncing</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/239">#239</a> Add a feature: Scroll To Bottom Button</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/240">#240</a> Fix a bug that moves the start time column of a giveaway if it has both received and not received copies</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/234">#234</a> Highlight game ids for games that are not in the Steam API when syncing and therefore cannot be converted to a name</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/241">#241</a> Fix a bug in Whitelist/Blacklist Checker that happens when checking group giveaways</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/243">#243</a> Add option to automatically backup data every X days</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/244">#244</a> Remove the plus sign after the level in Created/Entered/Won Giveaway Details</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/245">#245</a> Extend #226 to Imgur uploads</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/246">#246</a> Add option to refresh active discussions when refreshing giveaways in the main page through Endless Scrolling</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/248">#248</a> Add a feature: Refresh Active Discussions Button</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/247">#247</a> Replace colon with underline in exported file names</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/249">#249</a> Allow custom names for exported files</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/250">#250</a> Add an easy way to debug directly from ESGST</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/254">#254</a> Fix a bug in Giveaway Bookmarks that does not unbookmark a giveaway when entering it through SG's native button</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/255">#255</a> Add options to Giveaway Bookmarks to automatically unbookmark entered giveaways and show the button for entered giveaways</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/256">#256</a> Fix a bug that does not detect entered giveaways in the Giveaway Bookmarks list</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/252">#252</a> Fix a style issue in Giveaways Manager</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/253">#253</a> Add search filters to the settings menu</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/257">#257</a> Make some visual changes to Attached Images Carousel</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/258">#258</a> Allow users to order the heading buttons however they want</li>
</ul>

**7.8.1 (November 18, 2017):**

<ul>
    <li><a href="https://github.com/revilheart/ESGST/issues/214">#214</a> Fix a bug in Scroll To Top Button that happens in ESGST-generated pages</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/215">#215</a> Fix a bug that happens when typing \` in Comment Formatting Helper with preview enabled</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/212">#212</a> Fix a bug in Search Magnifying Glass Button that does not work outside of the main page</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/210">#210</a> Show script version in the header menu</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/209">#209</a> Improve the left/right buttons in Attached Images Carousel</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/208">#208</a> Add button to start Attached Images Carousel from the header</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/218">#218</a> Revert how new features/options are highlighted to the [NEW] text instead of the star icon</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/219">#219</a> Fix a bug that happens when trying to load a group/whitelist giveaway in Blacklist Giveaway Loader</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/220">#220</a> Fix a bug in Comments Reverser that reverses giveaways in the main page</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/222">#222</a> Fix a bug that happens when syncing won games</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/221">#221</a> Fix a style issue where popups keep shaking when already repositioned</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/223">#223</a> Add option to open the automatic sync in a new tab</li>
</ul>

**7.8.0 (November 16, 2017):**

<ul>
    <li><a href="https://github.com/revilheart/ESGST/issues/9">#9</a> Add option to preview comments to Comment Formatting Helper</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/184">#184</a> Add "unlimitedStorage" permission to extension</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/191">#191</a> Fully add the script code to the extension code</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/190">#190</a> Fix a bug that does not load Giveaway Bookmarks in the entered page</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/186">#186</a> Remove text from SG sync</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/189">#189</a> Fix a bug in Giveaways Extractor that happens when opening in a new tab</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/76">#76</a> Fix a bug that does not filter discussions on page load if Comment Tracker is disabled</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/185">#185</a> Add option to collapse sections in the settings menu</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/192">#192</a> Make new features/options more visible in the settings menu</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/137">#137</a> Prevent Header Refresher from notifying about wishlist giveaways that are above the user's level</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/142">#142</a> Improve how Whitelist/Blacklist Checker results are stored</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/193">#193</a> Fix a side effect from #185 that collapses the import/export/delete menus</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/194">#194</a> Separate option to reverse comments from Endless Scrolling into a new feature: Comments Reverser</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/195">#195</a> Add option to Whitelist/Blacklist Checker to skip a user if X pages have been checked without any result</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/196">#196</a> Add button to Whitelist/Blacklist Checker to manually skip users</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/197">#197</a> Add option to Whitelist/Blacklist Checker to check only selected users in the page</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/199">#199</a> Fix a bug that does not sync alt accounts</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/198">#198</a> Add a feature: Comments/Entries Checker</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/202">#202</a> Fix a bug in Real CV Calculator that happens when reviewing a giveaway</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/204">#204</a> Fix a bug in Giveaway Filters that does not filter giveaways correctly when using Endless Scrolling</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/205">#205</a> Move the scroll to top button more to the bottom/right</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/206">#206</a> Add option to show scroll to top button inside of footer</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/200">#200</a> Add option to make popups static</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/203">#203</a> Show game names instead of IDs when syncing</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/207">#207</a> Add a feature: Hidden Pinned Giveaways</li>
</ul>

**7.7.4 (November 12, 2017):**

<ul>
    <li><a href="https://github.com/revilheart/ESGST/issues/167">#167</a> Fix a Comment History conflict with other scripts</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/168">#168</a> Move entries tracker from settings menu to the user menu in the header</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/166">#166</a> Fix a bug that happens when trying to create multiple giveaways</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/169">#169</a> Fix a bug that happens when there are less than 5 unhidden discussions</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/171">#171</a> Fix a bug that shows the wrong message for cases where the user has unblacklisted another user in Blacklist Giveaway Loader</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/172">#172</a> Fix a bug in Group Library/Wishlist Checker that does not check only wishlist if there is no Steam API key set</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/173">#173</a> Fix a bug that prevents some giveaway features from loading</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/175">#175</a> Refresh active discussions and pinned giveaways when refreshing main giveaway pages in Endless Scrolling</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/174">#174</a> Fix a bug in Giveaway Winning Ratio that does not round up the ratio correctly</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/176">#176</a> Fix a bug in Attached Images Carousel that does not close the popup when clicking on the source link</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/177">#177</a> Fix a bug that happens when uploading images through Imgur</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/178">#178</a> Fix a bug in Tables Sorter that does not sort some columns correctly</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/179">#179</a> Remove text from giveaway icons in popups in normal view</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/164">#164</a> Fix a bug that does not automatically collapse replies in Collapse/Expand Replies Button when using Endless Scrolling</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/163">#163</a> Fix a bug that does not set the gift/key field correctly when editing a giveaway in Multiple Giveaways Creator</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/181">#181</a> Fix a bug that happens when trying to import/export through Google Drive/OneDrive using the script or the extension on Firefox</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/180">#180</a> Fix a bug in Multiple Giveaways Creator that alters the date when editing a giveaway</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/182">#182</a> Fix a bug that shows wrong chance/ratio in the entered page</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/183">#183</a> Add the script code to the extension code</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/145">#145</a> Add option to Giveaways Extractor to only extract from the current giveaway onwards</li>
</ul>

**7.7.3 (November 11, 2017):**

<ul>
    <li><a href="https://github.com/revilheart/ESGST/issues/136">#136</a> Move recent username changes and comment history from the header menu</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/139">#139</a> Extend Time To Enter Calculator to Giveaways Manager</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/138">#138</a> Remove text from giveaway icons in popups</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/146">#146</a> Fix a bug in Whitelist/Blacklist Sorter that opens the whitelist in the blacklist page</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/135">#135</a> Add download link to the update notification popup in the extension</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/148">#148</a> Extend Blacklist Giveaway Loader to situations where the user has unblacklisted the other user</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/140">#140</a> Fix a bug in Reply From Inbox that shows the wrong time ago for replies</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/150">#150</a> Fix a bug that opens the automatic sync multiple times</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/151">#151</a> Prevent sync from clearing game data when store method is unavailable</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/149">#149</a> Fix a bug in Game Categories that happens when the Steam store does not have information about the base game of a DLC</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/154">#154</a> Fix a bug that does not update the storage in the current session when deleting data</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/155">#155</a> Fix a bug that happens when importing/exporting data through Dropbox</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/156">#156</a> Add option to import/export through Google Drive</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/157">#157</a> Add option to import/export through OneDrive</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/158">#158</a> Fix a bug that calculates the size of files incorrectly when importing through Dropbox/OneDrive</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/159">#159</a> Make the buttons in the import/export/delete menus inline so there is more room for the options</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/160">#160</a> Color the buttons in the import/export/delete menus white</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/161">#161</a> Extend #159 to other places where there are multiple buttons</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/153">#153</a> Add option to shuffle giveaways to Multiple Giveaways Creator</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/162">#162</a> Fix a bug that does not update the cache when reordering/deleting giveaways in Multiple Giveaways Creator</li>
</ul>

**7.7.2 (November 4, 2017):**

<ul>
    <li><a href="https://github.com/revilheart/ESGST/issues/133">#133</a> Fix a typo in the URL for groups in Group Library/Wishlist Checker</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/134">#134</a> Fix a bug that does not update the last sync date when performing an automatic sync</li>
</ul>

**7.7.1 (November 4, 2017):**

<ul>
    <li><a href="https://github.com/revilheart/ESGST/issues/128">#128</a> Fix a bug that does not show Time To Enter Calculator in the settings menu</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/130">#130</a> Fix a bug in Endless Scrolling that does not load the next page when the ended filter is set to hide all and there is a deleted giveaway in the page</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/131">#131</a> Extend deleted filter to the entered page in Giveaway Filters</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/132">#132</a> Fix a bug that does not detect won games correctly</li>
</ul>

**7.7.0 (November 4, 2017):**

<ul>
    <li><a href="https://github.com/revilheart/ESGST/issues/106">#106</a> Fix a bug in Discussions Sorter that does not sort by created time correctly</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/107">#107</a> Stop Endless Scrolling in the entered page when reaching ended giveaways with the ended filter enabled as "hide all"</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/108">#108</a> Allow setting different automatic sync frequencies for each data</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/109">#109</a> Separate single giveaway filters from multiple filters</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/110">#110</a> Add a fallback method to Next/Previous Train Hotkeys</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/111">#111</a> Add an option not to exclude deals from the discussions section in Old Active Discussions Design</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/112">#112</a> Add a feature: Time To Enter Calculator</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/113">#113</a> Fix a bug that happens when syncing games</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/115">#115</a> Fix a bug in Entries Tracker that does not sort the dates correctly</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/116">#116</a> Add more stats to Entries Tracker</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/117">#117</a> Fix a bug in Giveaway Filters that does not apply overrides correctly</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/118">#118</a> Add 2 new links to the header menu</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/120">#120</a> Allow exporting settings without personal data</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/121">#121</a> Fix a bug that happens when completing the active discussions/deals</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/122">#122</a> Refresh header when refreshing page through Endless Scrolling if Header Refresher is disabled</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/123">#123</a> Add a button to reset the Imgur setting in Comment Formatting Helper</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/124">#124</a> Separate the Grid View elements below the enter/leave button in two columns</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/125">#125</a> Fix a bug that does not set the default value for new settings correctly</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/126">#126</a> Go to the next unread comment after going to the first in Comment Tracker</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/127">#127</a> Save data for whitelisted/blacklisted users in Whitelist/Blacklist Checker</li>
</ul>

**7.6.4 (November 3, 2017):**

<ul>
    <li><a href="https://github.com/revilheart/ESGST/issues/86">#86</a> Add an option to highlight public/group giveaways in Giveaways Extractor</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/87">#87</a> Ignore inactive users in Group Library/Wishlist Checker</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/88">#88</a> Make the header dropdown menus work in ESGST generated pages</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/89">#89</a> Fix a bug in Comment Formatting Helper that does not correctly undo automatic link formatting</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/90">#90</a> Split Shared Groups Checker results in two columns: public and private</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/91">#91</a> Fix a bug in Giveaway Popup that adds a button to the review giveaway page when creating invite only giveaways</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/92">#92</a> Complete the active discussions/deals if some of them have been hidden through Discussion Filters</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/93">#93</a> Fix a bug in Old Active Discussions Design that shows deals in the discussions section</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/94">#94</a> Fix a bug in Giveaway Filters that does not automatically filter giveaways in popups</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/95">#95</a> Undo formatting when pressing backspace in Comment Formatting Helper</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/96">#96</a> Focus on text area after undoing/redoing formatting in Comment Formatting Helper</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/97">#97</a> Fix a bug in Group Library/Wishlist Checker that uses the incorrect URL for groups</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/98">#98</a> Fix a bug in Shared Groups Checker that does not return the groups</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/99">#99</a> Reposition open popups every second</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/100">#100</a> Allow navigating through Attached Images Carousel using the arrow keys</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/101">#101</a> Improvements to #99</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/102">#102</a> Close a div tag in addDhHighlightButton</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/103">#103</a> Fix a bug in Giveaway Filters that does not filter giveaways when the genre filter is enabled</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/104">#104</a> Fix a bug that does not load the features correctly when a discussion with 0 comments is in the page</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/105">#105</a> Fix a bug that shows the SG icon instead of the ESGST one in some ESGST generated pages</li>
</ul>

**7.6.3 (November 2, 2017):**

<ul>
    <li><a href="https://github.com/revilheart/ESGST/issues/7">#7</a> Add an option to prevent Game Categories from being links in Grid View</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/54">#54</a> Fix a bug in Header Refresher that shows duplicate notifications</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/78">#78</a> Fix a bug in Giveaways Recreator that uses assigned keys instead of unassigned</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/79">#79</a> Fix a bug in Giveaway Filters that duplicates the DefaultUser preset every time a profile page is loaded</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/80">#80</a> Allow separate Giveaway Filters presets/settings for Giveaway Bookmarks, Giveaways Extractor and Giveaways Encrypter/Decrypter</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/81">#81</a> Fix a bug in User Tags that does not delete tags</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/82">#82</a> Add 3 new encryption methods to Giveaways Encrypter/Decrypter</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/83">#83</a> Fix a bug in Main Post Popup that scrolls down the page when the main post is hidden</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/84">#84</a> Fix a bug in Header Refresher that sometimes does not notify about wishlist giveaways in the tab title</li>
    <li><a href="https://github.com/revilheart/ESGST/issues/85">#85</a> Fix a bug in Giveaway Filters that does not rename presets globally</li>
</ul>

**7.6.2 (October 31, 2017):**

<ul>
    <li>Made some style alterations to Quick Giveaway Search and added an option (Giveaways.2.1) to hide the native search when on the main giveaway pages (<a href="https://github.com/revilheart/ESGST/issues/77">#77</a>).</li>
    <li>Extended Giveaway Filters to the profile pages.</li>
    <li>Fixed a bug in Giveaway Bookmarks that was unbookmarking giveaways for which there were not enough points to enter.</li>
    <li>Fixed a bug in Discussion Filters that was not filtering discussions automatically (<a href="https://github.com/revilheart/ESGST/issues/76">#76</a>).</li>
</ul>

**7.6.1 (October 29, 2017):**

<ul>
    <li>Fixed a bug in Quick Giveaway Search that was messing the header (<a href="https://github.com/revilheart/ESGST/issues/72">#72</a>).</li>
    <li>Extended Giveaway Filters and Giveaways Manager to Giveaway Bookmarks.</li>
    <li>When using Giveaways Extractor, you no longer have to click on "Extract" to start extracting - it now starts automatically.</li>
    <li>Discussion Filters now has a different preset for the created discussions page (<a href="https://github.com/revilheart/ESGST/issues/71">#71</a>).</li>
    <li>Fixed a bug in Group Library/Wishlist Checker that was showing the wrong percentages.</li>
</ul>

**7.6.0 (October 24, 2017):**

<ul>
    <li>Added something that should prevent ESGST from loading more than once in the same page for some users (<a href="https://github.com/revilheart/ESGST/issues/59">#59</a>).</li>
    <li>Added an option to Header Refresher to only notify about unentered wishlist giveaways that are ending in X hours (<a href="https://github.com/revilheart/ESGST/issues/64">#64</a>).</li>
    <li>Added Giveaways.2 Quick Giveaway Search.</li>
    <li>The genre filter in Giveaway Filters now works as a three-state filter like the others ("hide all" hides the genres listed, "show only" shows only the genres listed and "show all" shows everything).</li>
    <li>Fixed a bug in Unhide Giveaway Button that was not correctly detecting hidden games for Giveaway Bookmarks (<a href="https://github.com/revilheart/ESGST/issues/68">#68</a>).</li>
    <li>Blacklist Giveaway Loader now shows "You Are Blacklisted" if you have been blacklisted by the creator and "On Your Blacklist" if you have blacklisted the creator.</li>
    <li>Fixed a bug that was happening for users with Avatar Popout on click enabled.</li>
    <li>Group Library/Wishlist Checker now verifies if the user is still a member of the group.</li>
</ul>

**7.5.1 (October 23, 2017):**

<ul>
    <li>The popup that notifies about a new version is now dismissed when closed and only appears again for the next version (<a href="https://github.com/revilheart/ESGST/issues/65">#65</a>).</li>
    <li>Added a "Update" link to the popup above in the script.</li>
    <li>Added buttons to select all/none/inverse when syncing.</li>
    <li>Prevented Giveaways Manager from loading in some pages (<a href="https://github.com/revilheart/ESGST/issues/69">#69</a>).</li>
    <li>Possibly fixed a bug in Unsent Gifts Sender that was not sending all gifts (<a href="https://github.com/revilheart/ESGST/issues/3">#3</a>).</li>
    <li>Fixed a bug in CFH (Comment Formatting Helper) that was placing the cursor in the wrong place after pasting a link/image without a title.</li>
    <li>When toggling the Automatic Links/Images Paste Formatting in CFH, the focus now returns to the text area (<a href="https://github.com/revilheart/ESGST/issues/60">#60</a>).</li>
    <li>Fixed a bug that was preventing Group Library/Wishlist Checker from working properly in the script.</li>
</ul>

**7.5.0 (October 22, 2017):**

<ul>
    <li>Fixed a bug that was happening when importing groups.</li>
    <li>Giveaway descriptions are no longer mandatory in Enter/Leave Giveaway Button. Yes, for the millionth time this has changed again. Here's why: making giveaway descriptions mandatory results in many complaints and users rolling back to old versions, which is a bad thing, especially since ESGST is in constant development and bugs are constantly being fixed. In the end, I still think this falls to the user. Forcing something on someone who doesn't care about it amounts to nothing, they will still find ways to ignore it.</li>
    <li>Giveaways Extractor now detects giveaways that you cannot enter correctly (<a href="https://github.com/revilheart/ESGST/issues/58">#58</a>).</li>
    <li>Added Giveaways.39 Blacklist Giveaway Loader</li>
    <li>Fixed a bug in Comment Formatting Helper that was happening for script users when pasting links/images.</li>
    <li>Added Users.15/Users.16 Whitelist/Blacklist Manager</li>
    <li>Added Groups.3 Group Library/Wishlist Checker</li>
</ul>

**7.4.0 (October 21, 2017):**

<ul>
    <li>Made ESGST a bit more welcoming to new users (users that are installing it for the first time will now get some basic information to help them get started).</li>
    <li>In the settings menu you will now see some red icons for features that require syncing, and upon hovering over the icons, tooltips will appear telling you which data needs to be synced to make the feature work correctly.</li>
    <li>Moved the sync section to the top of the settings menu.</li>
    <li>Fixed a bug that was happening for some users when syncing groups.</li>
    <li>Added an option to the settings menu that allows you to sync previously won games.</li>
    <li>Fixed a bug that was not allowing users to drag and drop on Firefox.</li>
    <li>Added General.13 Attached Images Loader.</li>
    <li>Fixed a bug that was adding the Giveaways Manager button to the right side of the main page heading instead of the left (<a href="https://github.com/revilheart/ESGST/issues/63">#63</a>).</li>
    <li>Giveaways Extractor now extracts giveaways that cannot be accessed because of blacklist issues and colors them with a red background.</li>
    <li>Added an option to use precise start/end dates to Giveaway Templates.</li>
    <li>Fixed a bug in CEWGD (Created/Entered/Won Giveaway Details) that was ordering the columns in the entered page wrong.</li>
    <li>Fixed a bug in CEWGD that was showing the wrong creator for giveaways in the won page.</li>
    <li>Fixed a bug in Comment Formatting Helper that was not formatting some links correctly (<a href="https://github.com/revilheart/ESGST/issues/62">#62</a>).</li>
    <li>Fixed a bug in Comment Searcher that was preventing the script from loading correctly (<a href="https://github.com/revilheart/ESGST/issues/61">#61</a>).</li>
    <li>Fixed a bug in Not Activated/Multiple Wins Checker that was not coloring users.</li>
</ul>

**7.3.0 (October 17, 2017):**

<ul>
    <li>Made some changes to the structure of the code.</li>
    <li>Fixed a bug that was deleting tags when saving data.</li>
    <li>Fixed a bug that was happening for some users when syncing groups.</li>
    <li>Fixed a bug that was preventing some features from working correctly in pages generated by the script, such as "/esgst/bookmarked-giveaways".</li>
    <li>Added the scroll to top button from Endless Scrolling as a separate feature: 1.21 Scroll To Top Button</li>
    <li>Fixed a bug that was preventing Enter/Leave Giveaway Button and Giveaway Popup from working correctly with Comment Formatting Helper disabled.</li>
    <li>Fixed a bug in Main Post Popup that was opening the popup at the wrong position.</li>
    <li>Added the button to the comment formatting page from Comment Formatting Helper as an option (<a href="https://github.com/revilheart/ESGST/issues/57">#57</a>).</li>
    <li>Fixed a bug in Whitelist/Blacklist Checker that was not updating the status of users who had whitelisted/blacklisted you and then removed you from those lists.</li>
</ul>

**7.2.2 (October 14, 2017):**

<ul>
    <li>Giveaway Bookmarks can now be accessed through "/esgst/bookmarked-giveaways".</li>
    <li>Giveaways Encrypter/Decrypter can now be accessed through "/esgst/decrypted-giveaways".</li>
    <li>Giveaways Extractor can now be accessed through "/esgst/extracted-giveaways?url=/giveaway/XXXXX/" or "/esgst/extracted-giveaways?url=/discussion/XXXXX/".</li>
    <li>Added an option to each feature above to open it in a new tab using the new URL.</li>
    <li>Fixed some style issues in Grid View with Image Borders disabled.</li>
    <li>Fixed a bug in Giveaway/Discussion Filters that was not applying overrides correctly.</li>
    <li>Fixed a style issue in Giveaway/Discussion Filters that was making the legend and preset panels overlap for users with few filters enabled.</li>
    <li>Extended Giveaways Manager to every page and added the option to bookmark/unbookmark/hide multiple giveaways at once.</li>
    <li>Fixed a bug in Enter/Leave Giveaway Button that was hiding the enter button for won giveaways marked as not received.</li>
    <li>Next/Previous Train Hotkeys now detects previous/next links based on how many giveaway links there are in the page instead of their text (experimental).</li>
    <li>Giveaways Extractor now extracts all giveaways in the page instead of just the ones in the giveaway description (<a href="https://github.com/revilheart/ESGST/issues/55">#55</a>).</li>
    <li>Fixed a bug in Created/Entered/Won Giveaway Details that was opening Steam links in the same page instead of in a new tab.</li>
    <li>Fixed a bug in Comment Formatting Helper that was not showing the Giveaway Encrypter button (<a href="https://github.com/revilheart/ESGST/issues/56">#56</a>).</li>
    <li>Fixed a bug that was happening when adding comments to giveaways without a description (<a href="https://github.com/revilheart/ESGST/issues/53">#53</a>).</li>
    <li>Added an option to Game Categories (Games.3.21.2) that indicates if the base game of a DLC is free or not.</li>
    <li>Because of the new option above, added new filters to Giveaway Filters: "DLC (Free Base)" and "DLC (Non-Free Base)"</li>
</ul>

**7.2.1 (October 13, 2017):**

<ul>
    <li>Fixed a bug in Comment Formatting Helper that was happening in discussion pages.</li>
</ul>

**7.2.0 (October 13, 2017):**

<ul>
    <li>Removed the update button from the header menu in the extension, since you have to update it through the browser.</li>
    <li>Added an option that was missing from the settings menu to import/export/delete Giveaway Bookmarks data.</li>
    <li>Fixed a bug in Header Refresher that was not notifying unread messages in the icon of the tab.</li>
    <li>Fixed a bug in One-Click Hide Giveaway Button that was happening when hiding giveaways in popups.</li>
    <li>Fixed a bug that was showing the button to unhide giveaways everywhere instead of just in the main/giveaway pages (<a href="https://github.com/revilheart/ESGST/issues/50">#50</a>).</li>
    <li>Added the functionality above as a feature so you can choose whether you want it or not (2.12 Unhide Giveaway Button).</li>
    <li>You can now choose whether to load the groups in Giveaway Groups Loader on a panel upon page load (default), on a popout upon hover, on a popout upon click or on a popup upon click.</li>
    <li>Renamed Giveaway Countries Popout to Giveaway Countries Loader.</li>
    <li>You can now choose whether to load the countries in the feature above on a popout upon hover (default), on a popout upon click or on a popup upon click.</li>
    <li>Revamped Comment Formatting Helper (CFH).</li>
    <li>Fixed some bugs in CFH.</li>
    <li>There is now only one CFH panel per page, instead of one panel per text box. When you focus on a text box, the panel will move to that box.</li>
    <li>The buttons in the CFH panel are now faded by default and unfaded on hover.</li>
    <li>Added a button at the end of the CFH panel that links to the comment formatting page on SG/ST.</li>
    <li>You can now choose whether to open Avatar Popout upon hover (default) or click.</li>
</ul>

**7.1.1 (October 11, 2017):**

<ul>
    <li>Fixed a bug that was happening when trying to save data for users that were not yet on the database.</li>
    <li>Fixed a bug in Endless Scrolling that was not updating the points after removing entries from page 2 onwards (closes <a href="https://github.com/revilheart/ESGST/issues/20">#20</a>).</li>
    <li>You can now unhide games from the main/giveaway page (closes <a href="https://github.com/revilheart/ESGST/issues/37">#37</a>).</li>
    <li>Fixed a bug in Real CV Calculator that was showing the wrong CV because of the recent changes to the point system on SG (closes <a href="https://github.com/revilheart/ESGST/issues/46">#46</a>).</li>
    <li>Added a button to User/Game Tags that allows you to reset a tag to its default color.</li>
    <li>You can now easily add tags from a list of all tags you have saved in User/Game Tags (closes <a href="https://github.com/revilheart/ESGST/issues/34">#34</a>).</li>
</ul>

**7.1.0 (October 10, 2017):**

<ul>
    <li>Fixed various bugs that were happening when importing/exporting/deleting data, such as some data not being imported/exported and some data remaining in the storage despite having all options selected while deleting them.</li>
    <li>Added an option to import/export/delete discussion/giveaway filters presets (closes <a href="https://github.com/revilheart/ESGST/issues/45">#45</a>) and stickied giveaway countries data.</li>
    <li>Added an option not to filter games with no rating to Giveaway Filters.</li>
    <li>The basic and advanced chances/ratios are now colored separately.</li>
    <li>The option to load the groups as a popup in Giveaway Groups Loader has changed to a popout (now you simply have to hover instead of clicking).</li>
    <li>The Giveaways Extractor button now correctly appears only when there are giveaways on the page.</li>
    <li>Fixed a bug in Discussion Edits Detector that was not detecting edits and therefore not saving the comments.</li>
    <li>When adding a link/image without a title to Comment Formatting Helper, the pointer will now move to between the "[" and "]" (closes <a href="https://github.com/revilheart/ESGST/issues/42">#42</a>).</li>
    <li>You can now undo/redo formatting in Comment Formatting Helper.</li>
    <li>Fixed a bug in User Tags that was not detecting username changes correctly.</li>
</ul>
<p>Added the following features:</p>
<ul>
    <li>2.19 Giveaway Countries Popout</li>
</ul>

**7.0.2 (October 8, 2017):**

<ul>
    <li>The extension should now update automatically on Firefox.</li>
</ul>

**7.0.1 (October 8, 2017):**

<ul>
    <li>Fixed a bug in requests for the same domain on the extension.</li>
</ul>

**7.0.0 (October 8, 2017):**

<ul>
    <li>Replaced the Dropbox SDK with the HTTP endpoints, which should fix some bugs.</li>
    <li>Fixed a bug in Header Refresher that was not updating the enter buttons in the page.</li>
    <li>When inside a giveaway that you have no points to enter, the "Not Enough Points" button will now be replaced by Enter/Leave Giveaway Button and update accordingly when you get more points without the need to refresh the page.</li>
</ul>
<p>
    <b>ESGST has been ported to an extension (currently only tested with Firefox and Chrome). Head over to the ESGST discussion or GitHub page to learn how to upgrade. The script version of ESGST will continue to be updated normally for now, whenever the extension is updated (I will decide whether or not to discontinue it based on the extension reception). The "Beta" drop in the version name does not mean the script has become stable.</b>
</p>