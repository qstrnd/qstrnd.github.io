---
title: Bookmarks 
icon: fas fa-bookmark
order: 1
---

> Please note that this is a list of my personal bookmarks! I’ll be saving articles I like in the order I read them.
{: .prompt-tip }

# Jan 2025

#### Build Tools
- [objc.io Issue 6: Build Tools](https://www.objc.io/issues/6-build-tools/) — a great series of articles to get an overview of tools that enable the build process for Xcode project:
    - [The Build Process](https://www.objc.io/issues/6-build-tools/build-process/) — breaks down the iOS/macOS build process, explaining how source code is transformed into executable binaries through preprocessing, compiling, assembling, and linking.
    - [The Compiler](https://www.objc.io/issues/6-build-tools/compiler/) — introduces the workings of compilers, focusing on Clang and LLVM, explaining steps from parsing source code to generating optimized machine code.
    - [Mach-O Executables](https://www.objc.io/issues/6-build-tools/mach-o-executables/) — explores the structure of Mach-O files, the executable format on Apple platforms, detailing components like headers, segments, and the symbol table; a little outdated in some details (for example, Mac’s architecture is now ARM), but still great for understanding the general structure of `.o`-files and binary executables.
    - [CocoaPods Under the Hood](https://www.objc.io/issues/6-build-tools/cocoapods-under-the-hood/) — explains how CocoaPods manages third-party library integration in Xcode projects, ensuring seamless builds by modifying project files.
- [Dynamic Library Programming Topics](https://developer.apple.com/library/archive/documentation/DeveloperTools/Conceptual/DynamicLibraries/100-Articles/OverviewOfDynamicLibraries.html) — diving even deeper into the world of dynamic libraries. For me, it was occasionally challenging, but a very enjoyable read. The document explains the possibilities and reasoning behind dylibs, how they can be linked and loaded into the app, and delves into the problems and considerations that arise when designing one. It also provides nice code samples in a variety of languages.
- [WWDC '18 — Behind the Scenes of the Xcode Build Process](https://wwdcnotes.com/documentation/wwdcnotes/wwdc18-415-behind-the-scenes-of-the-xcode-build-process/) — notes for the WWDC video that has probably already disappeared from the internet. May be hard to read because of its brevity, but I found some info useful. Here's [another article](https://suelan.github.io/2020/07/05/20200705Behind-the-Scenes-of-the-%E2%80%A2Xcode-Build-Process/) based on the same session, which I found more coherent — plus, it has more pictures.
- [Apple’s use of Swift and SwiftUI in iOS 18](https://blog.timac.org/2024/1208-state-of-swift-and-swiftui-ios18/) — a nice overview of what has changed in iOS 18 (spoiler: Swift usage increased drastically, and the first Swift binaries appeared in the Secure Enclave, suggesting the use of embedded Swift). The methodology uses the exact tools mentioned in the articles above (namely `otool`), so for me, it served as a great application of knowledge. The author explains the methodology itself in previous articles, like [this one](https://blog.timac.org/2020/1019-evolution-of-the-programming-languages-from-iphone-os-to-ios-14/).


#### Other
- [SE-0302 — `Sendable` and `@Sendable` closures](https://github.com/swiftlang/swift-evolution/blob/main/proposals/0302-concurrent-value-and-concurrent-closures.md) — a proposal that explains one of the most important concepts of Swift 5, defining a value that can be passed safely across concurrency domains. Love the extensive examples.

# Dec 2024

- [Apple's Human Interface Guidelines](https://developer.apple.com/design/human-interface-guidelines/) — took me over a week of evening reading, but it was definitely worth it. Just enjoyed brushing up on the concepts and honestly was impressed by the level of detail even a minor interface element can have. It’s no doubt the Bible for every iOS developer.
- [App Store Review Guidelines](https://developer.apple.com/app-store/review/guidelines/) — a must-read for every developer who is about to submit their app to the App Store. I just reviewed it today and liked the clear language that Apple uses here.
- [User privacy and data use](https://developer.apple.com/app-store/user-privacy-and-data-use/) and [App privacy details](https://developer.apple.com/app-store/app-privacy-details/) - a great explanation of how to handle private data, what tracking is, and how to clearly state what data the app uses and how it is used.