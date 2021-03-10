![Banner](./assets/banner.png)

# Discord Name Badges
Some nice custom badges for next to usernames. If you want your OWN, COOL AMAZING CUSTOM badge, please read the **[badge request](https://github.com/Discord-Theme-Addons/discord-name-badges#badge-request)** segment of this readme.

![Preview](./screenshots/UsermodalPreview.png)
![Preview](./screenshots/MessagePreview.png)

## Get Your Own
I get it, you want your **VERY OWN** custom name badge, but you may be wondering to yourself, "omG lUCkFiRE HoW dO gET CoOL nAMeBAdge/!?!?" well.. the process is a lot simpler than you would think. Make an **[issue request](https://github.com/Discord-Theme-Addons/discord-name-badges/issues/new)** on this repo, and fill out the form. I'll update to give you your badge as soon as I can. Be on the lookout for your badge being added because usually hoof or I close the issue request and comment on it when I add it. Once I've added your badge, make sure you update the theme to get it!
- Please make sure your image is hoste on a trusted domain (such as i.imgur or cdn.discordapp) and that they are the same width by height so it wont look off.

If you don't like waiting, you can add your badge yourself! However, this process may be complicated for some people so I recommend just waiting. If you know what you're doing, proceed to follow the steps listed. If you add your badge this way, others who have this theme will not be able to see it.
### Powercord:
1. Head over to `./src/main/powercord` and open `_messages.scss` and `_profile.scss`
2. In `_messages.scss`, make a new line and enter:
```scss
@include messageBadge("YOUR_USER_ID", 'YOUR_BADGE_IMAGE');
// Make sure you replace YOUR_USER_ID with your User ID and YOUR_BADGE_IMAGE with the url you want as your badge.
```
3. In `_profile.scss`, make a new line and enter:
```scss
@include profileBadge("YOUR_USER_ID", 'YOUR_BADGE_IMAGE');
// Make sure you replace YOUR_USER_ID with your User ID and YOUR_BADGE_IMAGE with the url you want as your badge.
```
4. Make sure you save everything. Your badge should now appear if you've done everything right.

### Vizality
1. Head over to `./src/main` an open `./_vizality.scss`.
2. In this file, add a new line an enter:
```scss
@include badge("YOUR_USER_ID", 'YOUR_BADGE_IMAGE');
// Make sure you replace YOUR_USER_ID with your User ID and YOUR_BADGE_IMAGE with the url you want as your badge.
```
4. Make sure you save everything. Your badge should now appear if you've done everything right.


## Installation
I see you have your badge, congrats! Installation time: for **[Powercord](http://powercord.dev/)** or **[Vizality](https://vizality.com/)** installation, go to **Themes -> Open a CMD / Powershell / Terminal / Gitbash** in the folder, and enter the following:
```
git clone https://github.com/Discord-Theme-Addons/discord-name-badges
```

## Credits 
Thank you to [botato](https://github.com/bototo2) (aka mr cute panda) for helping me learn a bit more CSS to make it appear on at least 1 of the user modals.

Thank you to [Hoofer](https://github.com/HooferDevelops) for helping me maintain this, as well as adding basic Vizality support.

Thank you to [Snapperito](https://github.com/Snapperito) for grammar fixes.
