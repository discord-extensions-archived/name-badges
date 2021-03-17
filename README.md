![Banner](./assets/banner.png)

# Discord Name Badges
Some nice custom badges for next to usernames. If you want your **OWN, COOL, and AMAZING** custom badge, please read the **[badge request](https://github.com/Discord-Theme-Addons/discord-name-badges#badge-request)** segment of this readme.

![Preview](./screenshots/UsermodalPreview.png)
![Preview](./screenshots/MessagePreview.png)

## Installation
For **[Powercord](http://powercord.dev/)** or **[Vizality](https://vizality.com/)** installation, go to **Themes -> Open a CMD / Powershell / Terminal / Gitbash** in the folder, and enter the following:
```
git clone https://github.com/Discord-Theme-Addons/discord-name-badges
```

#### For BetterDiscord:
In order for this to work on BetterDiscord, you will need DevilBro's **[Plugin Library](https://github.com/mwittrien/BetterDiscordAddons/tree/master/Library/)**. I don't reccomend using this as it can cause performance issues due to it not being optimized that well. Proceed at your own risk.
- [Direct Download](https://betterdiscord.net/ghdl?id=3555)
- [View Source](https://raw.githack.com/Discord-Theme-Addons/discord-name-badges/main/src/main/betterdiscord/NameBadges.theme.css)

## Badge Request
I get it, you want your **VERY OWN** custom name badge. You may be wondering to yourself "omGGGG lucKFiEr HOw to gEt the CoOLeSt NamE bADgE/!?!" Well.. the process is a lot simpler than you would think. All you have to do is make an **[issue request](https://github.com/Discord-Theme-Addons/discord-name-badges/issues/new/choose)** using the right template. If you're first time requesting a badge, make sure you use the "Badge Request" template. If you're updating your badge, use the "Change Badge Request" template. As soon as I can, either Hoofer or I will update to give you your badge. Be on the lookout for your badge being added, because usually we will close the issue request and comment on it when it is added. Once your badge is added, please make sure you update the theme so it appears!
- **Please make sure your image is hosted on a trusted domain (such as i.imgur or cdn.discordapp) and that they are the same width by height so it wont look off.**

## Add it Yourself
If you're impatient and don't like waiting, you can add your badge yourself! However, for some people this process may be complicated, so I recommend waiting. Please note that others who have this theme will not be able to see your badge since it's added through your end. 

If you know what you're doing, you can proceed to follow the steps listed below.
1. Head over to `./src/main` an open `./_users.scss`.
2. All the way at the bottom, make a new line and enter:
```scss
@include badge("YOUR_USER_ID", 'YOUR_BADGE_IMAGE');
```
3. Replace `YOUR_USER_ID` with your user id and replace `YOUR_BADGE_IMAGE` with the image url that is the badge that you'd like.

## Credits 
A big thank you to everyone who helped with this!
- **[botato](https://github.com/bototo2)** (aka the CUTEST panda in the world) for helping me learn more CSS to make badges appear on the user profile popout modal. 
- **[Hoofer](https://github.com/HooferDevelops)** for helping me maintain this as well as adding basic Vizality support.
- **[Snapperito](https://github.com/Snapperito)** for touching up the readme by fixing grammar issues.