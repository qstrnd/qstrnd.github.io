---
layout: post
title: Geeky macOS Setup for Productivity
tags: [macOS, productivity]
author: andy
---

In this post, I would like to share my macOS setup, which I have developed over the years through my experience in programming and general computer usage. Every small amendment to my common routines stemmed from a fundamental need: how can I eliminate the time spent on repetitive actions? Initially, not everything was obvious, and it took time for me to realize that it was even possible. This is why I am sharing it and hoping that you will find some tips and tricks that will work well for you.

I'd like to note that I describe my own setup and don't urge you to copy it word by word. You may tweak individual shortcuts as you want and you may skip the whole sections altogether. The goal is to show you what I found useful and what you might have not thought of, and in no way to force you to thoughtlessly copy the approaches. Use this info to help you build your own! Believe me, it's a fun never-ending story.

## General

The first thing I do when I install my operating system is that I download [Raycast](https://www.raycast.com/). Why? Because it completely changes the way I interact with my laptop. I configure it so that it replaces Spotlight and can be opened by pressing `⌘` + `␣` (`Command` + `Space`). Some people prefer Alfred for similar reasons, but I stick with Raycast since it allows extensions with its free version. When I miss in the free version is the ability to sync the setup across devices, but it hasn't been a big issue for me.

So why would I replace the default Spotlight? The thing is, Raycast is not just another version of Spotlight. It does not only the search, but also extends your mac to support commands that integrate all your apps in a single prompt. You can open applications, open your bookmarks in browser, search for your notes in a third-party app like Notion, make a ChatGPT prompt, init a new repository, open an Xcode project and so on. The possibilitites are almost limitless and all tell you only a few that I use most of the time.

### App Launch & Window Switching

The first thing you probably do after you open boot your laptop is opening your favorite application. Clicking on an icon is good, but it can be a little time consuming. Search is a little better if you type fast (and it's the way how I often launch apps that I don't use much often), but another nerdy way is to assign a particular shortcut to a set of apps that you use the most. With Raycast, you can use this shortcut not only to open, but to switch to the windows of an opened application which can be way faster that both clicking on icon in dock or using `⌘` + `⇥` (`Command` + `Tab`).

I tried to make a pattern that will not overlap with existing shortcuts and decided to stick with `⌃` + `⌥` + `⌘` (`Control` + `Option` + `Command`) and another key of preference. Typically one that I can somehow associate with the application, like `I` for iTerm, `X` for Xcode or `M` for Spotify (i.e. **M**usic). Some I chose with the notion to be able to type it quicker, like `,` for ChatGPT (which I've been using a lot since the app was released).

My current shortcuts, each starting with `⌃` + `⌥` + `⌘` (`Control` + `Option` + `Command`), are:

| Key | Application | Comment |
|----------|----------|----------|
| `X` | Xcode | My main IDE for everything Swift / Objective-C |
| `S` | Xcode Simulator | |
| `I` | iTerm | My favorite terminal |
| `Z` | Figma | `Z` just to be close to Xcode because sometimes I switch between these apps every minute to make something as in the sketch |
| `,` | ChatGPT | `,` is just a convenient key that my middle finger can reach easily |
| `V` | Visual Studio Code | I use it for scripting, viewing text-based files and writing this blog post |
| `B` | Firebox | The **B**rowser that I use |
| `T` | Telegram | Extremely convenient cross-platform messenger |
| `M` | Spotify | My favorite **M**usic player |
| `N` | Notion | My current **N**ote-taking app |
| `I` | IntelliJ IDEA | For Kotlin programming |
| `A` | Android Studio | For **A**ndroid and Kotlin Multiplatform |
| `R` | iBooks | For **R**reading eBooks on programming. Also convenient to switch back and forth when I reproduce some code samples in a code editor |
| `F` | Finder | To open **F**inder windows |
| `D` | Diagrams.net (former draw.io)  | I occasionally draw UML **d**iagrams with it |
| `C` | Anki | I use it to study with **c**ards and spaced repetition  |
| `P` | Proxyman | A **p**roxy tool for debugging and mocking network responses   |

### Effective Search

I almost never use Finder to navigate through my file hierarchies. That's why I mostly keep them flat (e.g. I put every PDF or word in my iCloud Drive Documents folder) and try to name them in a way that would allow to easily search for it in the future.

I use Raycast for search and invoke it with `⇧` + `⌃` + `⌘` + `F` (`Shift` + `Control` + `Command` + `F`), where `F` stands for **F**ind. I noticed that it works much better Spotlight that sometimes cannot find particular documents on my laptop. 

As you can observe, I also use a special pattern for search commands: `⇧` + `⌃` + `⌘` (`Shift` + `Control` + `Command`) plus a letter, typically the one used to open the same application. Here are the ones I currently use:

| Key | Application / Service |  Raycast Extension Link | Comment |
|----------|----------|----------| ----------|
| `F` | Search Files | Raycast built-in | File search |
| `D` | DuckDuckGo | Raycast built-in | Open the query in default browser. You can use the search engine of your preference  |
| `N` | Notion | [Link](https://www.raycast.com/notion/notion) | Notes search |
| `G` | Google Workspace | [Link](https://www.raycast.com/raycast/google-workspace) | Search for my Google Drive files (I don't store the locally)  |
| `B` | Browser Bookmarks | [Link](https://www.raycast.com/raycast/browser-bookmarks) | Search for my bookmarks |
| `G` | Browser History | [Link](https://www.raycast.com/crisboarna/browser-history) | Search for browser history  |
| `X` | Xcode | [Link](https://www.raycast.com/SvenTiigi/xcode) | Open recent Xcode projects |
| `V` | Visual Studio Code | [Link](https://www.raycast.com/thomas/visual-studio-code) | Open recent VS Code projects |
| `R` | Github | [Link](https://www.raycast.com/thomas/github-repository-search) | Github **r**epository search |

In-app search is the primary reason why I use different Raycast extensions, but don't hesitate to explore other possibilities like project or document creation, derived data deletion, player control and so on. I usually just type in such commands, about which below.

### Commands

Whenever you need something, you usually have to ways: click through app launchers, folders, menus, and so on or search for it. As you have probably guessed, I prefer the latter for speed. But I'm not that crazy to remember *every* possible shortcut in the system. That's where search comes handy as my ultimate guide.

Want to lock the screen? Open Raycast and type "lock" instead of remembering the shortcut. Want to open Privacy & Security settings to allow the launch of some recently installed app? Just type in "Privacy" and proceed directly to that part of the Settings app. "Hide all apps"? Here you go! You get the idea. Search is usually faster and it doesn't take much as with exact shortcut memorization.

But here's one shortcut I recommend you to memorize. I use it a lot. You've probably noticed that every app has that Menu Bar that may contain infinity of commands. Some of them have their own shortcuts, but we've already discussed that we don't want to memorize every possible shortcut. Here's where our hero comes in:

- `⇧` + `⌘` + `/` (`Shift` + `Command` + `Slash`) Search any command in the Menu Bar.

I would also like to get you acquianted with another app usage pattern that may be called Command Palette, which is triggered by `⇧` + `⌘` + `P` (`Shift` + `Command` + `P`) in VS Code, or Quick Actions `⇧` + `⌘` + `A` (`Shift` + `Command` + `A`) in Xcode. It usually brings up a promt that allows to search for different commands of the app and can even allow natural language input. I prefer first using this feature and only switch to the Menu bar search when there's no special command launcher in the app.

### Window Management

Most of us work with multiple apps, pacely switching between their windows. Some apps can have more than one window, so it may be cumbersome to keep focus on the ones that you really need at the moment. Over the years, I have tried different approaches: using second monitor, assigning particular apps to particular virtual desktops, using Stage Manager, and just having everything on a single screen (I rarely even have the need to use a second monitor now). 

Every approach has pros and cons, and I'll elaborate on why the last one worked perfectly for me:
- Predictability: as I mentioned, the shortcuts to open / switch to different apps make the workflow predictable - whenever I need to switch to the browser, I just press the associated shortcut. Never will I find myself pressing the shortcut only to find the is no window in the right place, as may happen with multiple desktops. 
- Flexibility: also the reason why I gave up on multiple desktops — sometimes I need different combinations of apps present on the same screen. It's simpler to keep everything on one desktop and change the layout (more about it below) according to specific needs
- Speed: I love MacOS animations, they're really cute, but at the same time they're but a waste of precious seconds that is repeated throughout days. That's why I don't like desktop switching, as well as the fancy Stage Manager.

Below I will show you how to get the most out of this approach.

#### Basic Shortcuts

I've already shown you some custom shortcuts to launch apps and perform searches, but don't forget about the default ones that can be extremely useful:

- `⌘` + `⇥` (`Command` + `Tab`) Switch to the next most recently used app among your open app.
- `⌘` + `` ` `` (`Command` + `Grave accent`) Switch between the windows of the app you're using. It switches only between the apps on the same desktop, so using only one you'll never miss a window. A nice feature to mention here is App Exposé, which can be trigger by a swipe down with three fingers if you enable it in Settings. It can be convenient sometimes to get a grasp of all your windows related to the same app, but mostly I still stick with just the shortcut.

Simple as that. 

#### Layout

> Starting from macOS Sequoia, there's a feature called [Window tiling](https://9to5mac.com/2024/07/19/use-automatic-window-tiling-macos-sequoia/). I haven't used it at the time of the writing, but I value it as a nice move from the perspective of the OS development and maybe it can even replace third-party solutions
{: .prompt-tip }

There are different window managers available. Raycast comes with a built-in [Window Management](https://www.raycast.com/core-features/window-management) functionality. I never used this one as I saw I had to set shortcuts for every layout position manually.

I used [Magnet](https://magnet.crowdcafe.com/) for a long time but then I decided to switch to the free alternative [Rectangle](https://rectangleapp.com/). To me, they're identical. I memorized different shortcuts and even added little adjustments to them. Here are the ones that I use most often:

- `⌃` + `⌥` + `←` / `→` (`Control` + `Option` + `Left Arrow` / `Right Arrow`) Change current window size to fit the left / right half of the screen
- `⌃` + `⌥` + `↩` (`Control` + `Option` + `Return`) Almost maximize
- `⌃` + `⌥` + `⌘` + `↩` (`Control` + `Option` + `Command` + `Return`) Maximize
- `⌃` + `⌥` + `⌫` (`Control` + `Option` + `Backspace`) Restore size
- `⌃` + `⌥` + `C` (`Control` + `Option` + `C`) Center in the screen

I rarely use the others but I do when I need to fit more than two apps on the screen. An example of such situation: I code (VS Code), I read the guide (Browser or Books), and I want to see the result (Browser with a local build of my project).

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/layout.png)
*My layout of three applications fitting on the same screen*

I never use Full-screen Mode except for movies and videos that I really want to focus on. I just maximize the window I need. The reasoning stays the same: I try to escape additional desktops for simpler navigation.

### Clipboard History

Another staple feature, and I am so deeply surprised to see many people are not aware of, is a clipboard history. It's especially useful when you're dealing with chunks of code and commands. And it can also be a registery of quick-access info, such as your email-address or your current task tickets (hello to Jira users).

I've been using Raycast's built-in [Clipboard History](https://manual.raycast.com/core) since it's free and it works perfectly for me. It can work with different kinds of data (not only text-based), has previews (for example, for copied color names, image or web articles), stores your data for up to three months in the free-tier Raycast version.

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/clipboard.png)
*A piece of my current clipboard history*

There are, however, some features that I miss from my beloved [Paste](https://pasteapp.io/). It has unlimited storage, cloud sync, categories, special titles for the content you save, and so on. You can use it not only as a clipboard, but a separate database: for your code snippets, or common text that you repeat in your communication, and more. The only downside is that it's kind of pricy and at some point I decided to stick to a more affordable solution. 

### Dock

Another thing that gets me suprised is that people leave the default Dock as is. In my opinion, you should better remove the apps that you don't use that often from the Dock. 

Another trick is to group applications, and you can add a spacer for it with the following commands (use the terminal to type it).

Add a Regular Spacer:
```bash
defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="spacer-tile";}'; killall Dock
```

Add a Small Spacer
```bash
defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="small-spacer-tile";}'; killall Dock
```

And there's another thing: folders! You can put any folder for a quick access to your Dock, just find it in Finder or search with Spotlight / Raycast and drag and drop it near the default Downloads folder (also note that you can remove it if you want). In my dock, besides the Downloads folder, I also have Desktop (much easier that getting docs from the desktop behind the windows, especially if you plan to drop the file somewhere), Documents and Screenshots.

I prefer the Dock on the left side, but I temporarily put it on bottom to take this screenshot. I don't use groups scrictly as you can see, but it just helps my eyes to find the needed app quicker.

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/dock.png)
*My Dock*

I already mentioned it and I'll repeat: whenever I can, I launch / switch to apps and search for files with either shortcuts or search. But I still love the Dock to be present and never hide it (except for the full screen).

### Cleanup

As we work, we produce a lot of artefacts: downloaded images and documents, code files and projects, installed applications, caches and more. It's as natural for the tech world as in the nature itself. And sometimes you want to take more control over what and how should be spared and saved and what should be wasted. I use several apps that help me in this aspect.

#### Downloads & Desktop

I love [Hazel](https://www.noodlesoft.com/) to add some very basic automation rules to the very basic Downloads & Desktop folders. They're simple: delete the files that are there for more than a month and I haven't opened them for the same period; gather all downloaded documents of different kind to my iCloud Documents folder; move all screenshots to my Screenshots folder. Also I have my Trash automatically cleaned from the files that are older than a month. Some people use it for more strict categorization of their files, but as of now I don't have such need.

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/hazel.png)
*My rules in Hazel app*

I should also mention that the app is not free, but it's a one-time purchase and I think it's worth it. If you decided to give it a try and would like to import my rules to start with, you can download them [here](https://drive.proton.me/urls/GN9AVWRFK8#u3x1Hc9EvnKf).

#### Unused Apps

I use the free [AppCleaner](https://freemacsoft.net/appcleaner/). Whenever I want to delete an app from my Mac, I don't just move the app icon to the Trash folder, but a drag-and-drop it to this cleaner. I tries to find caches and other leftovers from the app you're about to delete, as you can see in the screenshot below. So it makes your deinstallation more clean!

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/appCleaner.png)
*Attempting to delete Parallels (just for example!)*

There's also a famous app called [CleanMyMac](https://cleanmymac.com/) which you can use to delete apps and do more. But to me it's a little overpriced since it requires a subscription. 

#### Storage

I have to admit, I still haven't dealt with the infamous [Mac System Data is large](https://discussions.apple.com/thread/253667048?sortBy=rank) problem completely. It's a pain, especially for developers, since our work involves involuntary production of many caches, logs and other data that may be there but in fact is not needed.

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/storageSettings.png)
*My storage. As you see, there's a lot of system data*

I do use the possibilities of native Settings app, but in practice it rarely helps. There're other tools which allow more granular control, one of them is [DaisyDisk](https://daisydiskapp.com/). I use it to locate the heaviest folders and occasionally delete them if I'm sure it's safe. The app is not free, but it's a one-time purchase.

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/daisyDisk.png)
*DaisyDisk comes in! You can already see that System Data mostly consists of caches*

I also use [DevCleaner](https://github.com/vashpan/xcode-dev-cleaner) which is a free tools for iOS developers. You can use it to clean simulators (very handy!), derived data, old archives, docs and logs.

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/devCleaner.png)
*DevCleaner*


## Command Line

### iTerm

### theme

### aliases. ruby manager (?)

###

## Git

gitworkflow
commit philosophy
make everything a repository

## Code Editor

## Browser

## Miscellaneous 

- pomodoro
- toggl
- appcleaner
- quick notes
- bartender
- more space
- hazel
- currency converter, weather
- cpu, memory, battery and other diagnostics


General principles
- learn shortcuts
- customize to your needs
- look for extensions

Tooling
- Xcodes
- App cleaner
- disk something (to clear space)
- puntoswitcher
- daisydisk
- wwdc