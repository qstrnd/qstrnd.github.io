---
layout: post
title: Geeky macOS Setup for Productivity
tags: [macOS, productivity]
author: andy
---

In this post, I would like to share my macOS setup, which I have developed over the years through my experience in programming and general computer usage. Every small amendment to my common routines stemmed from a fundamental need: how can I eliminate the time spent on repetitive actions? Initially, not everything was obvious, and it took time for me to realize that it was even possible. This is why I am sharing it and hoping that you will find some tips and tricks that will work well for you.

I'd like to note that I describe my own setup and don't urge you to copy it word by word. You may tweak individual shortcuts as you want and you may skip the whole sections altogether. The goal is to show you what I found useful and what you might have not thought of, and in no way to force you to thoughtlessly copy the approaches. Use this info to help you build your own! Believe me, it's a fun never-ending story.

## Principles

What you may find here can seem too much. And it may seem there are other ways to make it more conveniently. I don't want to argue. You may follow your own understanding what convenience and beauty is and what suits your needs best. What I want to highlight again, however, is that I didn't get from a newbie to the current state in my relationship with the computer in a night. Not even in a year. So as my relashionship matured, I tried and learned new approaches and adjusted the way I interact with my computer. What guided me, as I believe, were the following principles:

1. Reduce repetitiveness.
2. Try to make it faster.
3. Explore what others do and see how it suits me.

Guided by this principles, I learn shortcuts for the interactions I do the most, write scripts for something that needs automation, look at documentation and available extensions and so forth. 

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

Command line is something that is overlooked by many people, including developers. In most scenerios, what you can do in using command line, like browsing your files, committing git changes, installing programs and so on, can be done using a graphical interface. You should find out what's more convenient for you. 

But there's also one thing I adore about the command line: it's a unified interface for everything possible. You just write a command to make the app do something. You can combine these commands, redirecting the output of one command as the input for other. Add complex conditions, that's how scripts are born. And so much more. I urge you to read more about the [Unix philosophy](https://en.wikipedia.org/wiki/Unix_philosophy), it's about exactly the same: make some simple blocks (commands in our case) and allow them to work together.

So yes, command line, although a little old-fashioned, is simple and predictable. You find a new program, you check its commands with `program --help` or read its manual with `man program` and it's enough to get started. One can argue if it's really simpler than the graphical interface, but I can say that I sometimes find it harder to navigate to the right button that to type in the right command, especially with custom aliases for the most common use cases (more about it below).

### Basics

First of all, you don't have to repeat every command every time. Use `⌃` + `R` (`Control` + `R`) to search in your command history.

If you need to repeat a command that you've just types (you may needed it when you need to rerun something as the superuser), type `!!`, as in `sudo !!`. If you need to repeat the last argument from the previous command, use `!$`, as in `cd !$`.

Learn some shortcuts to navigate to the begining or end of line and to jump between words. I personally prefer `vi` mode which I enable with a plugin. See more about Vim below.

### iTerm

I use [iTerm](https://iterm2.com/features.html) almost for historical reasons. Probably the features that made me switch from the default Terminal app are full 24-bit and 256-color mode and more advances abilities to split panes. I just advice to check their website and see if there're any features you would miss in the deafult app.

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/terminal.png)
*iTerm*

### Appearance

As you might have noticed, I have a custom theme that I like a lot. It's called [Powerlevel10k](https://github.com/romkatv/powerlevel10k). It beautifully shortens the text for current working directory and highlights the current git branch. It has other awesome features which you might like, check them out. Many of them can be configured with an extremely convenient configuration wizard that is launches after installation.

### Plugins

Appearance is not the only thing you can customize. There are many plugins that your command line can be set up with, and some of them can be extremely useful.

My personal favorite is [Oh My Zsh](https://ohmyz.sh/). It's not just a single extension, but rather a framework for easier management a magnitude of plugins and configurations. Shortly said: it makes the life much easier! I tried configuring my plugins manually but eventually decided to stick with Oh My Zsh. My theme, that I mentioned previously, is installed with it. As well as the plugins that I would like to mention:

| Plugin          | Description                                                      |
|-----------------|------------------------------------------------------------------|
| [git](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/git)           | Enhances Zsh with git-related aliases and functions              |
| [colored-man-pages](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/colored-man-pages) | Adds colors to man page output for better readability      |
| [alias-finder](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/alias-finder)  | Helps find and manage aliases                                    |
| [aliases](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/aliases)       | Simplifies alias creation and usage                              |
| [vi-mode](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/vi-mode)       | Enables vi key bindings in Zsh                                   |
| [autojump](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/autojump)      | Quickly navigates to frequently used directories                 |
| [pj](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/pj)            | Manages project directories                                      |
| [fzf](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/fzf)           | Integrates the fuzzy finder tool fzf for command-line operations |

[Here](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins) is an extensive list of all plugins that Oh My Zsh supports. Some of them are just aliases, while some vi-mode or fzf integrate into your shell. Try them out!

#### Aliases

Find what you do repeatedly. Make an alias! If you're just starting, I just suggest that you get around in the command line for a while and then run this command:

```bash
history | awk '{CMD[$2]++; count++;} END { for (a in CMD) printf "%d\t%d%%\t%s\n", CMD[a], CMD[a]/count*100, a;}' | sort -nr | head -n 10
```

It'll print your mostly used commands. Here are mine on my personal machine:

```bash
248	16%	gst
132	8%	ll
110	7%	cd
108	7%	git
81	5%	gaa
71	4%	xed
61	4%	gcmsg
43	2%	..
41	2%	bundle
39	2%	code
```

It shows that my mostly used command is `gst` which is an alias for `git status`. `ll` is also an alias for `ls -lh` which nicely prints the content of the current directory with some useful information. Imagine how much time these aliases have spared me!

Sometimes, easpecially when an alias is not your own, it may be hard to remember. That's why I use `alias-finder` plugin that mildly reminds me of the existing aliases that shorten the command I have just entered.

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/terminalStatus.png)
*I've typed **git status** and got a hint at my **gst** alias*

#### Scripts 

Customize your shell's configuration file! Not only aliases can be added to it, but also some custom logic. When you need to do something before your shell session is started, you put it to your shell config file. For Zsh, it would be `zshrc` in your Home directory. What I provide below is just a random example of some repetitive tasks that can be managed this way. 

If you've ever worked with ssh, you probably encountered the need to start the ssh agent in the background. That can be done with such command in your config file:
```bash
# Add ssh-agent for 
eval "$(ssh-agent -s)" > /dev/null 2>&1
```

Another recent example: I found myself constantly `cd`ing to the `~/Developer` folder almost every time I opened iTerm. I already had the alias `cdd` for it but I decided to go further and write this little script:
```bash
# open Developer directory instead of HOME if it exists on current machine
if [ "$PWD" = "$HOME" ]; then
  if [ -d "$HOME/Developer" ]; then
    cd "$HOME/Developer"
  fi
fi
```

So every time I open the terminal, I am in my favorite folder as my working directory! I addd some conditions because sometimes, when I open shell from VS Code as example and it opened the directory of the project I'm working on, I don't want to navigate to the Developer folder.

#### Git

I'd like to mention my git config separately since it's my primary activity in terminal. I mentioned the [git](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/git) plugin for aliases that I use, most common being aliases for `git status`, `git commit --message`, `git push`, `git pull`, `git checkout`. 

There are also more complex functions that are defined in my `gitconfig` under `[alias]` and been there for ages. Check this one:
```bash
 bclean = "!f() { DEFAULT=$(git default); git branch --merged ${1-$DEFAULT} | grep -v \" ${1-$DEFAULT}$\" | xargs git branch -d; }; f"
```

So every time I type `git bclean`, it deletes all branches that have been merged into the specified branch (or the default branch if none is specified), except for the currently checked-out branch.

Another one that I often use:
```bash
bdone = "!f() { DEFAULT=$(git default); git checkout ${1-$DEFAULT} && git up && git bclean ${1-$DEFAULT}; }; f"
```
It does what `bclean` does plus checks out to the default branch which is often `main`, `master` or `develop`.

I also like this one to pile up work in progress and quickly commit it:
```bash
save = !git add -A && git commit -m "SAVEPOINT"
```

And this one to clean correctly sync my submodules:
```bash
submod = "!f() { git submodule deinit -f . && git submodule update --init  && git submodule foreach --recursive git reset --hard  > /dev/null; }; f"
```

I mentioned above that I also see my current branch right in the terminal which helps me a lot. I have stats like how far my local branch is ahead or behind the respective origin branch. I also heavily use autocompletion that comes with Oh My Zsh: it helps me find the appropriate branch name, tag or even commit hash.

If you're a new developer, I highly recommend you to read about [Gitflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) and use it extensively. Have some personal projects for learning after reading an article? Do not just write them and throw away! Make a single repository, make feature branches for separate learning projects, commit your work as you progress and merge it when it's ready. I honestly wish I'd started doing it earlier since I've lost some pieces of code that I nostalgically (and sometimes practically!) miss. By having such a repository for your learning projects, you can keep track of how you learn and progress which is important, even encouraging for the next achievements.

#### Dotfiles Repo

So many configs already. So many files to put them it. It may be hard to move to a new laptop and manually copy all your configurations. That's why some people use a separate git repository for their dotfiles and I'm among them (here's [mine](https://github.com/qstrnd/dotfiles), originally forked from [Holman's](https://github.com/holman/dotfiles)).

Basically, it's just a repo for config files (or as many people would refer to them, dotfiles, since they usually start with a dot to make them hidden by default which is a common pattern for configuration files). 

This particular dotfiles repo has some scripting magic, like this:

> Anything with an extension of .zsh will get automatically included into your shell. Anything with an extension of .symlink will get symlinked without extension into $HOME when you run script/bootstrap.

A symlink (short for symbolic link) is just a reference in your file directory to another file. It's very handy to link the actual config file with its expected place in the system, as in the example:
```bash
ln -s dotfiles/actualGitconfig ~/.gitconfig
```

I urge you to commit your dotfiles so that you never miss your configs on another machine!

#### More

Many principles that I follow in my approach in dealing with the command line were brought or solidified by the course called [The Missing Semester of Your CS Education](https://missing.csail.mit.edu/). It focuses on practical lessons, like how to work in command line, what are the most used command-line programs, how to write scripts and automate repetitive tasks with them, and more. Check it out!

## Code Editor



## Browser

Browser is a special app that not only allows you to access the web, but with web-applications it becomes somewhat like an operating system in its own, so that many people prefer using web apps to their native counterparts. I personally use Firefox for my home environment and Chrome for my work environment. I gave up on using Safari for its lack of many extensions (though there are some really nice ones!). I won't compare different browsers here, but I can say that I value Firefox for being pretty lightweight, pretty customizable, and with privacy in focus.

### Privacy

I'm not very ideological, but I like to be cautious with what I share. If you want to learn more, check this public [Privacy Guide](https://www.privacyguides.org/en/basics/why-privacy-matters/). This website also contains some info about particular apps, as well as some tricks and techniques, and I found some of the recommendations useful.

Besides choosing Firefox as my default browser, at some point I decided to use [DuckDuckGo](https://duckduckgo.com/) as my default search engine. It worked surprisingly well compared to others and currently covers my needs.

I use [uBlock Origin](https://ublockorigin.com/), an extension that blocks not only ads, but also ad trackers. And as a second protection level I utilize [Ghostery](https://www.ghostery.com/). Aside of a few websites that require you to allow ads, the experience of browsing the web is much better with these extensions. It also makes your browsing a little more private.

#### Security

Where there's privacy, security should also follow suite. I won't cover it deeply, but would rather mention some very basics.

I setup my browser following a privacy guide, as this one for [Firefox](https://www.privacyguides.org/en/desktop-browsers/#recommended-firefox-configuration). I sync my data via Firefox servers, except for passwords. I decided to store passwords in a separate place intentionally, and use [Bitwarden](https://bitwarden.com/) for it. I've got installed both the extension and the app. I use the free version, and it's enough to get all my devices synced, including iPhone, where Bitwarden can be selected as the default password manager and will provide autofill ability wherever it's supported.

For some services, including social and financial ones, I setup 2FA (two-factor authentication) through an OTP (one-time password), which I [prefer over SMS](https://www.okta.com/blog/2020/05/why-you-should-ditch-sms-as-an-auth-factor/). There are plenty of apps that allow you to set up an OTP, among them are [Raivo](https://raivo-otp.com/) or [Google Authenticator](https://apps.apple.com/us/app/google-authenticator/id388497605).

### Useful Extensions

There are other extensions that I like a lot and use daily. I'll describe them a little below. The links below will direct either to the extension's website, where you can find a version for your browser of choice, or to the respective [Firefox Addons](https://addons.mozilla.org/en-US/firefox/) if I wouldn't be able to find one.

| Extension | Description |
| --- | --- |
| [Vimium](https://vimium.github.io/) | A keyboard shortcut extension for navigation and control in the browser. Nerdy but very cool! |
| [Dark Reader](https://darkreader.org/) | Turns on dark mode for websites to reduce eye strain |
| [Highlight by Trix](https://addons.mozilla.org/en-US/firefox/addon/highlight-by-trix/) | Allows you to highlight text on web pages for reference or emphasis. I use `⌥` + `H` (`Option` + `H`) to trigger it |
| [Bonjourr - Minimalist Startpage](https://bonjourr.fr/) | A customizable, minimalist start page with weather and bookmarks (my favorite so far!) |
| [DeepL Translate: Reading & Writing Translator](https://www.deepl.com/en/app) | Provides translations for reading and writing in multiple languages. I use `⌥` + `D` (`Option` + `D`) to translate a selected piece of text |
| [History AutoDelete](https://addons.mozilla.org/en-US/firefox/addon/history-autodelete/) | Automatically deletes your browsing history based on rules you set |
| [Pin Unpin Tab](https://addons.mozilla.org/en-US/firefox/addon/pinunpin-tab/) | Quickly pin or unpin tabs in the browser. I use `⌥` + `P` (`Option` + `P`) to toggle it |
| [Close Other Tabs Button](https://addons.mozilla.org/en-US/firefox/addon/close-other-tabs-button/) | Adds a button to close all other tabs except the current one. I miss `⌥` + `⌘` + `W` (`Option` + `Command` + `W`) from Safari |

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/bonjourr.png)
*Bonjourr as my Startup Page*

And in case you wonder what theme I use, it's called [Firefox Alpenglow](https://addons.mozilla.org/en-US/firefox/addon/firefox-alpenglow/).

#### Vimium

Yes, this Vim-like extension. I want to say more about it. It's the reason why I highly reduced the usage of trackpad. I use it to switch between tabs, navigate inside the page, open bookmarks and so on. Below is a demo of one of its functions that highlights links on the webpage and allow to navigate to the link by pressing the corresponding keys. 

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/vimium.png)
*Vimium extension mode after pressing **f** on a webpage*  

## Miscellaneous 

I would assume that you use macOS so below there will be links to the macOS App Store if the will be no separate website for the app.

#### Pomodoro Timer

I use the [Pomodoro Technique](https://en.wikipedia.org/wiki/Pomodoro_Technique) at work and for personal activities. I work concentrated during 25 minutes, then make a pause for 5, then repeat for times, with the last time having a pause of 15 minutes instead. There are different applications, and I decided to stick with Raycast's buil-in Pomodoro. A also have a nice timer in the Menu Bar that comes with it.

#### Time Tracking

Sometimes I use [Toggl](https://toggl.com/) to track how much time I devote to different projects and endeavors. It's a nice cross-platform app, it supports features like pomodoro and billing, so it's worth giving a try.

#### Menu Bar

If you feel your Menu Bar is a little cluttered, you can explore [Bartender](https://www.macbartender.com/) app. I don't use it, but I once tried and the idea itself was funny: to customize when and where you see the menu items in the upper-right corner of your screen. You can hide them, show different sets of them in different modes, customize spacing in between and more.

#### Floating Notes

I use Notion as my note-taking app, but sometimes there's the need to make and show notes in some lighter shape. That's where Raycast's built-in Floating Notes come in handy. I use it for the words that I jot down while watching a movie in a foreign language, some thought not to forget later, or even meeting notes when I share my screen and don't want to accitentally show my other notes since they may be private. Here's how it look right now for example:

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/floatingNotes.png)
*Floating Notes*

Apple's Quick Notes are good as well, but I don't use them since they appeared after I learned about Floating Notes.

#### More Space

I do have to mention it! I think my Mac's screen is big enough to fit more text and elements, so I go to the Display settings and enable higher rosolution (under More Space). Here you can compare it and decide wha't better for you:

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/lessSpace.png)
*Default Space*  

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/moreSpace.png)
*More Space*

#### Keyboard Input Source

For Russian-speaking users, it can be convenient to use apps like [Puntoswitcher](https://yandex.ru/soft/punto/mac/?noredirect=1). It can be handy to remap what you've entered in English into Russian and vice versa. Not sure if it sends some data to Yandex, that's why I don't use it myself now.

#### Xcodes Management

If you need to manage multiple installations of Xcode (which can be common at work), thre's a nice app called [Xcodes](https://github.com/XcodesOrg/XcodesApp). You can install and remove different versions and control when to update.

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/xcodes.png)
*Xcodes*  

#### WWDC

You can access WWDC videos with Apple's official [website](https://developer.apple.com/videos/all-videos/) or [app](https://apps.apple.com/us/app/apple-developer/id640199958), but I'd recommend using this unofficial [WWDC app](https://github.com/insidegui/WWDC). It has really nice search, ability to make a watch list, bookmark sessions and add notes to them.

![img-description](assets/posts/geeky-macos-setup-for-productivity/img/wwdc.png)
*Unofficial WWDC app*

#### Currency Conversion

I just type something like `50 EUR to AMD` and it works out of the box. I think it's not even a Raycast feature but the system search feature, which is available even on iOS.

#### Diagnostics & Stats

I don't use widgets or special tools for diagnostics. The most "advanced" stuff I do here is to check what cycle count my battery has. But I do use Activity Monitor sometimes, mostly to find out what makes my Mac lag sometimes (and it goes lag, I experience crashes sometimes and so on — nothing is perfect).

And I also enable battery percentage in the Menu Bar item. I still want to be precise about it.