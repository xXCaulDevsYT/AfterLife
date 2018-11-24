# AfterLifePlus Features
Fully Featured KitPvP Custom Scoring And Stats Tracking Plugin!

### Original Edition
[Download Here](https://github.com/Aurora-Development/AfterLife)

### Plus Edition
[Download Here](https://github.com/xXCaulDevsYT/AfterLifePlus)

![Total downloads](https://img.shields.io/badge/downloads-1-blue.svg)
![Total views](https://img.shields.io/badge/views-15-blue.svg)

### To Do List
 - [x] Score points on Kill! `(+ gain xp)`
 - [x] Losse xp on Death!
 - [x] Calculates kill/death ratio 
 - [x] Level up when acheved spesified amount of XP `(see config)`
 - [x] Commands to see your or another players' stats `(suports formAPI)`
 - [x] Enable floating texts to see leaderboard of stats `(see commands)`
 - [ ] Add commands to easialy change settings in config
 - [ ] Add Level up timer `(level up over time, so stay online to level up!)`
 - [ ] Add Minutes Spent In Combat Leaderboards `(Plus Edition Only)`
 - [ ] Add Top XP Leaderboards `(Plus Edition Only)`
 - [ ] Add Longest Bow Kills & Hits Leaderboards `(Plus Edition Only)`
 - [ ] Add Kill Rewards `(Plus Edition Only)`
 - [ ] Add Levels Into PurePerms Prefix `(Plus Edition Only)`
 - [ ] Add Custom Eventing for Kills & Deaths `(Plus Edition Only)`
 
### Custom Event
The custom event is simple, it disables the title screen to prevent accedendal quit to menu ;)
```yml
# config.yml
#choose between 'custom' or 'default'
death-method: "custom"
```

### Commands
```yml
stats: 
    description: "Shows PvP Stats '/stats or /stats <player>'"
    
setleaderboard: 
    description: sets leader board that displays player stats (floating texts)
```

### Full Config
```yml
#Set world to what world you want the texts to spawn in. Currently only supports one world.
#enable floating texts.
#true: false:
texts-enabled: true
texts-world: "lobby"

#how many players to display on leaderboard
texts-top: 5

#setts the title for each leaderboard
texts-title:
  levels: "&b< PvP Levels Leaderboard >"
  kills: "&b< Kills Leaderboard >"
  kdr: "&b< K/D Ratio Leaderboard >"
  streaks: "&b< Top Killstreaks >"

#Disables PvP at spawn... uses server default level, 
#if want to use custom level set this to false and use (no-PvP-in-level)
no-PvP-at-spawn: true

#disables PvP in spesified world
#works if no-PvP-at-spawn: is set to false
#may add worlds!
no-PvP-in-level:
  - "world1"
  - "world2"
  - "world3"

#choose to use unique "form" or "standard" message to display stats
#form requires FormApi plugin
#methods => "form" "standard"
profile-method: "form"

#choose between 'custom' or 'default'
#custom bypasses the death 'main menu' screen and default does not
death-method: "custom"

#use built in level up system that adds levels on kill and removes level on death
#choose 'false' if you alredy have a level up plugin
#true: false:
use-levels: true

#use level up timer
#adds xp over time
#(example) stay online to gain xp
# THIS IS A W.I.P (doesnt work yet)
use-level-up-timer: false

#amount of xp to be given on kill
add-level-xp-amount: 50

#amout of xp to be lost on death
loose-level-xp-amount: 10

#how much xp is required for level up
xp-levelup-ammount: 1000
```
## Developers
1. @cosmicAtom (Original Author)
2. @iShabbz102 (Original Author)
3. @xXCaulDevsYT (Plus Edition Author)

