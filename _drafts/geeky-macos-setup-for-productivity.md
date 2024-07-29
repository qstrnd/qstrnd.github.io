---
layout: post
title: Geeky macOS Setup for Productivity
tags: [macOS, productivity]
author: andy
---

In this post, I would like to share my macOS setup, which I have developed over the years through my experience in programming and general computer usage. Every small amendment to my common routines stemmed from a fundamental need: how can I eliminate the time spent on repetitive actions? Initially, not everything was obvious, and it took time for me to realize that it was even possible. This is why I am sharing it and hoping that you will find some tips and tricks that will work well for you.

## General

The first thing I do when I install my operating system is that I download [Raycast](https://www.raycast.com/). Why? Because it completely changes the way I interact with my laptop. I configure it so that it replaces Spotlight and can be opened by pressing `⌘` + `␣` (`Command` + `Space`). Some people prefer Alfred for similar reasons, but I stick with Raycast since it allows extensions with its free version. When I miss in the free version is the ability to sync the setup across devices, but it hasn't been a big issue for me.

So why would I replace the default Spotlight? The thing is, Raycast is not just another version of Spotlight. It does not only the search, but also extends your mac to support commands that integrate all your apps in a single prompt. You can open applications, open your bookmarks in browser, search for your notes in a third-party app like Notion, make a ChatGPT prompt, init a new repository, open an Xcode project and so on. The possibilitites are almost limitless and all tell you only a few that I use most of the time.

### Application Launch & Window Switching

The first thing you probably do after you open boot your laptop is opening your favorite application. Clicking on an icon is good, but it can be a little time consuming. Search is a little better if you type fast (and it's the way how I often launch apps that I don't use much often), but another nerdy way is to assign a particular shortcut to a set of apps that you use the most. With Raycast, you can use this shortcut not only to open, but to switch to the windows of an opened application which can be way faster that both clicking on icon in dock or using `⌘` + `⇥` (`Command` + `Tab`).

I tried to make a pattern that will not overlap with existing shortcuts and decided to stick with `⌃` + `⌥` + `⌘` (`Control` + `Option` + `Command`) and another key of preference. Typically one that I can somehow associate with the application, like `I` for iTerm, `X` for Xcode or `M` for Spotify (i.e. **M**usic). Some I chose with the notion to be able to type it quicker, like `,` for ChatGPT (which I've been using a lot since the app was released).

My current shortcuts, each starting with `⌃` + `⌥` + `⌘` (`Control` + `Option` + `Command`), are:

| Key | Application | Comment |
|----------|----------|----------|
| `X` | Xcode | My main IDE for everything Swift / Objective-C |
| `S` | Xcode Simulator | |
| `X` | iTerm | My favorite terminal |
| `I` | Figma | `Z` just to be close to Xcode because sometimes I switch between these apps every minute to make something as in the sketch |
| `,` | ChatGPT | `,` is just a convenient key that my middle finger can reach easily |
| `V` | Visual Studio Code | I use it for scripting, viewing text-based files and writing this blog post |
| `B` | Firebox | The **B**rowser that I use |
| `T` | Telegram | Extremely convenient cross-platform messenger |
| `M` | Spotify | My favorite **M**usic player |
| `N` | Notion | My current **N**ote-taking app |
| `I` | IntelliJ IDEA | For Kotlin programming |
| `A` | Android Studio | For Android and Kotlin Multiplatform |
| `R` | iBooks | For **R**reading eBooks on programming. Also convenient to switch back and forth when I reproduce some code samples in a code editor |
| `D` | draw.io  | I occasionally draw UML diagrams with it |
| `F` | Finder | To open finder windows |

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
| `V` | Visual Studio Code | [Link](https://www.raycast.com/thomas/visual-studio-code) | Open recent VSCode projects |
| `R` | Github | [Link](https://www.raycast.com/thomas/github-repository-search) | Github **r**epository search |

In-app search is the primary reason why I use different Raycast extensions, but don't hesitate to explore other possibilities like project or document creation, derived data deletion, player control and so on. I usually just type in such commands.

### Window Management

cmd `

### Clipboard History

### Dock

- spaces
- folders


## Command Line

### iTerm

### theme

### aliases. ruby manager (?)

### 

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