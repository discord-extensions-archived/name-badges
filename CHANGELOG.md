# v1.4.0
Some minor adjustments / changes.
- Repo has been completely redone.
    - New README & assets.
    - Redid the file structure.
    - Some class changes for badges being applied.
- There is no longer any Vizality support, as I have no way to add it (for the recent rework anyways). If you're an Alpha tester for Vizality, and want to add it "properly," feel free to make a pull request doing so.

# v1.3.0
Some minor adjustments / changes:
- A lot less specific on what classes are used.
- Switched to `@each` from `@mixins`. I feel like this is a way better system, tho generally it does the same thing.
- Some file structure recostruction.

# v1.2.2
Changed imports to use `./_users.scss` instead of `./users`. This should hopefully prevent & fix any issues with operating system types, assuming that was the issue to begin with. This hopefully will resolve [pull #85](https://github.com/Discord-Theme-Addons/discord-name-badges/pull/85).

# v1.2.1
Split updates for this version, I don't feel like a version bump is that necessary for a small change.
- Badges now appear in Mutal Friends on the profile modal for Powercord and Vizality. 
- BetterDiscord now uses an import instead of being a dedicated file, making updates more reliable.

# v1.2.0
Added some changes I missed from a previous update to Vizality and BetterDiscord, as well as changing the classes that are used. I feel like this change was needed as the way it was done before looked pretty wonky, it may look worse but compared to before I feel like it's way better. Small chance I may revert that part of this update.

# v1.1.9
Badges will now appear on the left side and not right. I felt this was a good change, but I may revert it if enough people ask. (please spare me from that hell..) I've also changed some of the classes and attributes to be "better". Badges should now also appear in pinned messages + message searching.

# v1.1.8
Added badge support to the beginning of DMs. This will only appear on Vizality and Powercord. I also changed how the SCSS compiles into CSS, should clear up a few excess lines. Might revert this later on depending on if it causes poor performance.

# v1.1.7
There were many split updates along this version, basically just me changing things up.
- Added support for BetterDiscord. You will need DevilBro's **[Plugin Library](https://github.com/mwittrien/BetterDiscordAddons/tree/master/Library/)** for this to work properly.
- Added badge support to friends list on Powercord. On the topic of Powercord, now everything is inside of one file instead of spilt across multiple. 
- Finally, all users will be in ONE file instead of me having to copy-paste across multiple. This makes it SOOOOO MUCH EASIER for me to add people's badges!

# v1.1.6
Yet another enhancement update (well for me at least). Learnt something new with mixins: you can have a variable set in an attribute using them. With this information, I can make the layout of everything practically the same, I'd only have the change the name of the mixin. This makes it easier for me to add badges to other files. Here's a basic example of that:
```scss
// Taking a close look, you can see how this is applied.
@mixin badge($userID, $badgeLink) {
    [data-author-id="#{$userID}"].message-2qnXI6 .contents-2mQqc9 h2 .username-1A8OIy {
        &::before {
            content: " ";
            background: url($badgeLink) center/90% no-repeat;
            padding: 0 10px 0 10px;
            margin-left: 2px;
        }
    }
}

            // $userID               $badgeLink
@include badge("399416615742996480", "https://cdn.discordapp.com/emojis/635936642372337674.png?v=1");
```
Following this update, I had to do some wonky copy-pasting. If your badge isn't appearing right, submit an issue request asking for a fix.

# v1.1.5
Vizlaity finally has the vz-user-id attribute on message, as well as on user modal popouts. Messages will no longer use the src*= magic attribute, so there should be some optimization. I also changed the files that the manifests target, so whichever client mod you're using will target the proper files.

# v1.1.4
A small change for the future: restructured the file structure a bit to separate Powercord and Vizality better. Since the data-author-id attribute is originally a Powercord one, once Vizlaity re-adds the vz-user-id attribute to messages I can change some things back over. For now, it'll continue using src*=. (which is probably gonna be really unoptimized)
- **BUG:** An issue I found out with doing it this way is since it relys on the user's profile picture url, if the user removes their profile picture, the badge will not show as Discord uses a special asset for default profile pictures.

# v1.1.3
Semi-big changes coming to this repo (finally), originally was gonna do it sometime in the future but thanks to Discord changing attribute selectors for the 50th time.. yeaaa.
- Fixed for badges not displaying on usernames in messages.
- Restructured the file structure a bit.
- Better Vizality support (so if you're on Vizality, badges should appear on more things compared to Powercord).
- Small repo rewrite, looks nicer doesn't it?
- Changelog for v1.1.0 and later. Guess what, you're reading it right now!

# v1.1.1 - v1.1.2
Attempts at basic Vizality support by [Hoofer](https://github.com/HooferDevelops/).

# v1.1.0
In order for better maintainability, I recoded this to be in SCSS instead of CSS. You may be asking "well, what's the difference!?!? do i still have my badge?!??!!" First off, there really isn't much of a difference besides it's easier for me to work with and is less of an eye sore. Secondly, yes you still have your badge. If you have name badges before this update, make sure you reinstall the theme completely to prevent any issues. If you're using the import, you have to install the theme as is because you cannot import an SCSS file. If your badge isn't appearing / appearing properly, make an issue request and ill look into it. 
