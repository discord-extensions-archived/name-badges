![Banner](./assets/banner.png)

# Discord Name Badges
Some nice custom badges for next to usernames. If you want your OWN, COOL AMAZING CUSTOM badge, please read the **[badge request](https://github.com/Discord-Theme-Addons/discord-name-badges#badge-request)** segment of this readme.

![Preview](./screenshots/UsermodalPreview.png)
![Preview](./screenshots/MessagePreview.png)

## Installation
I see you have your badge, congrats! Installation time: for **[Powercord](http://powercord.dev/)** or **[Vizality](https://vizality.com/)** installation, go to **Themes -> Open a CMD / Powershell / Terminal / Gitbash** in the folder, and enter the following:
```
git clone https://github.com/Discord-Theme-Addons/discord-name-badges
```

#### For BetterDiscord:
In order for this to work on BetterDiscord, you will need DevilBro's **[Plugin Library](https://github.com/mwittrien/BetterDiscordAddons/tree/master/Library/)**. I don't reccomend using this as it can cause performance issues, due to it not being optimized that well. Proceed at your own risk.
- [Direct Download](https://betterdiscord.net/ghdl?id=3555)
- [View Source](https://raw.githack.com/Discord-Theme-Addons/discord-name-badges/main/src/main/betterdiscord/NameBadges.theme.css)

## Badge Reqeust
I get it, you want your **VERY OWN** custom name badge, but you may be wondering to yourself, "omG lUCkFiRE HoW dO gET CoOL nAMeBAdge/!?!?" well.. the process is a lot simpler than you would think. Make an **[issue request](https://github.com/Discord-Theme-Addons/discord-name-badges/issues/new)** on this repo, and fill out the form. I'll update to give you your badge as soon as I can. Be on the lookout for your badge being added because usually hoof or I close the issue request and comment on it when I add it. Once I've added your badge, make sure you update the theme to get it!
- **Please make sure your image is hosted on a trusted domain (such as i.imgur or cdn.discordapp) and that they are the same width by height so it wont look off.**

## Add it Yourself
If you don't like waiting, you can add your badge yourself! However, this process may be complicated for some people so I recommend just waiting. If you know what you're doing, proceed to follow the steps listed. If you add your badge this way, others who have this theme will not be able to see it.
1. Head over to `./src/main` an open `./_users.scss`.
2. All the way at the bottom, make a new line and enter:
```scss
@include badge("YOUR_USER_ID", 'YOUR_BADGE_IMAGE');
```
3. Replace `YOUR_USER_ID` with your user ID and replace YOUR_BADGE_IMAGE with the image url that is the badge that you'd like.

## Credits 
Thank you to [botato](https://github.com/bototo2) (aka mr cute panda) for helping me learn a bit more CSS to make it appear on at least 1 of the user modals.

Thank you to [Hoofer](https://github.com/HooferDevelops) for helping me maintain this, as well as adding basic Vizality support.

Thank you to [Snapperito](https://github.com/Snapperito) for grammar fixes.
