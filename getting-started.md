# Getting Started

Here you will learn how to build your first GStyle2 pack.

## The folder

First, inside the packs folder you should create a new folder named after what you want to name your pack once you have an idea of what to make.
  
Examples would be `jarvisdevil.mypack` or `jarvisdevil.my_pack_name`. You should go by the `author_name.pack_name` format otherwise we will do it for you if you ever choose to submit your pack.  
  
**Inside that folder you will have three very important files:**
```
main.gstyle2 - The actual script file that will be executed when the pack is loaded.
banner.png - The banner that will be shown in the GStyle2 menu.
info.txt - Information of the pack.
```
**If you are going to run audio or sprite creation related commands, you will need to create two folders inside your pack: `audio` and `sprites`. Make sure to use MP3 for Audio and PNG, WebP or GIF for Sprites then put what you want in those folders.**

## The banner.png File

**This will be the banner that will be shown in the GStyle2 menu.**  
  
Go onto any photo editing software or website like Pixlr X, Adobe Photoshop or anything else and make something cool.  
Make sure the image is in the 3:1 aspect ratio (So try 1200x400).

## The info.txt File

**This will be information related to the GStyle2 pack which will be used a lot so this is important.**  
  
Example:
```
name = My Awesome Pack
description = Does something cool.
version = 1.0.0
author = jarvisdevil
```
**IMPORTANT: Do not put spaces or anything special in the author or version, you cannot list multiple developers as the author.**

## The .gstyle2 File

**The main.gstyle2 file is the main script file that will be executed when the pack is loaded.**  
  
Example:
```
# This is a comment
for "CreatorLayer" {
    log.info "Hello, World!"
}
```
  
Then you can enable the pack using the GStyle2 menu and it should work!

### Undestanding for

**A for defines what should be executed on what layer which is useful for those who want stuff on different menus or places in Geometry Dash.**  
  
You can find what layer you are in by opening DevTools and looking at the first thing you see under tree. When you launch the game for example, going stright into DevTools reveals you are under MenuLayer.  
  
**A list of all layers that are supported in GStyle2 (we still support the same layers as the original GStyle):**
```
LikeItemLayer, LevelInfoLayer, LevelBrowserLayer, GJShopLayer, LevelSelectLayer,
LevelAreaInnerLayer, ProfilePage, MessagesProfilePage, FriendsProfilePage,
FRequestProfilePage, FriendRequestPopup, ShareCommentLayer, GJAccountSettingsLayer,
DailyLevelPage, GauntletSelectLayer, GauntletLayer, SongInfoLayer, LevelLeaderboard,
InfoLayer, PauseLayer, UIOptionsLayer, SetIDPopup, CreateGuidelinesLayer, SelectArtLayer,
ColorSelectPopup, CustomSongLayer, LevelSettingsLayer, LevelEditorLayer, EditLevelLayer,
GJPathPage, SetTextPopup, SetFolderPopup, AudioAssetsBrowser, LevelSearchLayer,
NCSInfoLayer, MusicBrowser, GJColorSetupLayer, LevelPage, MenuLayer, CreatorLayer,
GJGarageLayer, LevelAreaLayer, SecretLayer5, RewardsPage, ChallengesPage,
EditorOptionsLayer, GJPathsLayer, MoreSearchLayer, LevelCell
```
(if you want to add something to somewhere and we are missing something, let me know. i'll be happy to add support for it!)

### Understanding Comments

**Comments are lines that start with `#` and are ignored by the executor, this way you can add notes or anything you want to your script.**