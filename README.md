# Beginner Learning Materials on Reverse Engineering Video Games

Here is a compiled list based on personally recommended learning materials to help people with the process of learning how to reverse engineer video games. <br>
I hope it will help others spend more time learning and less time searching.

Majority of the collected resources here will be focused on reversing PC games on the Microsoft Windows operating system with x86 assembly in mind over x64 as it is easier to learn.

Reversing engineering video games is more often than not related to "game hacking", they come and go together so don't be surprised if some of the learning materials come from such sites/sources.

## Recommended order to learn

1. Learn how to search efficiently on Google, all your answers and resources are found on the internet
2. Learn using Cheat Engine
3. Learn about hexadecimal and binary numbering systems, and about computer memory in general
4. Learn x86 assembly
5. Learn C++
6. Learn using IDA/Ghidra
7. Learn basics of game programming
8. Learn fundamentals of the Win32 API
9. Learn the inner workings of Windows operating system, aka Windows internals
10. Practice, practice, practice...

## Software needed for reversing

It's not recommended to run any of these tools (especially Cheat Engine) while playing multiplayer games that have anti-cheat systems in place, unless you know what you are doing.

For starters get familiar with Cheat Engine, and either IDA or Ghidra.

- Memory scanners:
    - [Cheat Engine](https://www.cheatengine.org/)

- Disassemblers / Decompilers / Debuggers:
    - [IDA (freeware edition)](https://www.hex-rays.com/products/ida/support/download_freeware/)
    - [Ghidra](https://ghidra-sre.org/)
    - [x64dbg](https://x64dbg.com)
    - [dnSpy (decompiler, debugger, and editor for C# applications)](https://github.com/dnSpyEx/dnSpy)

- Process Tools:
    - [ProcessHacker (monitor process and system resources)](https://processhacker.sourceforge.io/)
    - [ProcessMonitor (monitor real-time file system, registry and process/thread activity)](https://docs.microsoft.com/sysinternals/downloads/procmon)
    - [API Monitor (monitor and control API calls)](http://www.rohitab.com/apimonitor)

- PE Tools:
    - [Explorer Suite (PE editor)](https://ntcore.com/?page_id=388)
    - [Detect It Easy (file type and packer identifier)](https://github.com/horsicq/Detect-It-Easy)
    - [TrIDNet (file identifier)](https://mark0.net/soft-tridnet-e.html)

- Network Tools:
    - [Wireshark](https://www.wireshark.org)
    - [mitmproxy](https://mitmproxy.org/)
    - [Fiddler](https://www.telerik.com/fiddler)

- Other:
    - [HxD editor (basic hex editor)](https://mh-nexus.de/en/hxd/)
    - [ImHex (advanced hex editor)](https://github.com/WerWolv/ImHex)
    - [ReClass.NET (reverse-engineering data structures in memory)](https://github.com/ReClassNET/ReClass.NET)

## Picking the right tools

Before getting to work on a game you must know your target, so it's important to gather some information such as:
- What software technologies it uses
- What programming language and compiler it had been developed with
- Does it have any anti-reversing or anti-tamper technology in place
- Is it running on any popular third-party game engines (Unity, Unreal Engine, Source Engine, etc.)

Games sharing the same engines often have really similar and recurring codebase that you can use to your advantage. For third-party game engines such as Unreal Engine or Unity there are a lot of custom tools online that can ease the process of reverse engineering.

Games coded in high-level interpreted/intermediate programming languages such as C# or Java are generally much easier to reverse engineer as compared to C/C++, due to the metadata not being lost as they aren't compiled into low-level machine code.

For Unity-based games (and for any other games developed with the .Net Framework) use dnSpy instead of IDA/Ghidra.

We are mainly going to focus on reversing games coded in C++ as it is still the gold standard in video game programming.

- Examples of games made with C++:
    - Counter-Strike
    - Grand Theft Auto V
    - Fortnite
    - World of Warcraft
    - Tom Clancy's Rainbow Six Siege
    - Fallout 4
    - Borderlands
    - Rocket League
    - Destiny 2
    - ARK: Survival Evolved

- Examples of games made with C#:
    - Genshin Impact
    - Beat Saber
    - Rust
    - Hearthstone
    - Subnautica
    - RimWorld
    - Hollow Knight
    - Cuphead
    - Getting Over It
    - Risk of Rain 2

## Must-read beginner level materials

- Guides to game reversing:
    - [Game Hacking Academy](https://gamehacking.academy/)
    - [From coding to hacking: An introduction guide to practical (external) game hacking](https://www.unknowncheats.me/forum/programming-for-beginners/267073-coding-hacking-introduction-guide-practical-external-game-hacking.html)

- Guides to x86 assembly:
    - [What Is Assembly Language? - javidx9](https://www.youtube.com/watch?v=1FXhjErUz58)
    - [A Crash Course in x86 Assembly for Reverse Engineers - SensePost](https://sensepost.com/blogstatic/2014/01/SensePost_crash_course_in_x86_assembly-.pdf)

- Guides to IDA:
    - [IDA Pro Beginner Guide](https://guidedhacking.com/threads/ida-pro-beginner-guide.8006/)

- Basic game programming concepts:
    - [Game Programming Algorithms and Techniques - Sanjay Madhav](https://www.informit.com/articles/article.aspx?p=2167437&seqNum=2) (This article has 7 pages in total, read up to page 5-6)
    - [Understanding the Game Main Loop - Rodrigo Monteiro](http://higherorderfun.com/blog/2010/08/17/understanding-the-game-main-loop/)

- Books:
    - Reversing and game hacking:
        - [Game Hacking: Developing Autonomous Bots for Online Games - Nick Cano](https://www.amazon.com/Game-Hacking-Developing-Autonomous-Online-ebook/dp/B01J4NKSRI)
        - [Practical Malware Analysis: The Hands-On Guide to Dissecting Malicious Software - Michael Sikorski and Andrew Honig](https://www.amazon.com/Practical-Malware-Analysis-Hands-Dissecting/dp/1593272901)
    - Game programming:
	    - [Tricks of the Windows Game Programming Gurus, Second Edition (2002) - Andre Lamothe](https://www.amazon.com/Tricks-Windows-Game-Programming-Gurus-dp-0672323699/dp/0672323699)
	    - [Game Coding Complete, Fourth Edition (2012) - Mike McShaffry](https://www.amazon.com/Game-Coding-Complete-Fourth-McShaffry/dp/1133776574)

- Google:
    - [How to Search the Internet Effectively - WebTools Company](https://www.casey.org/media/CLS_ResourceGuides_subdocs_SearchInternetEffectively.pdf)
    - [GOOGLE CHEAT SHEET](https://web.archive.org/web/20220122205807/https://library.cbtsc.ca/wp-content/uploads/2019/10/GOOGLE-CHEAT-SHEET.pdf)
    - [The Ultimate Google Search Operators Cheatsheet - Helvis Smoteks](https://blog.linkody.com/guides/google-search-operators-cheatsheet)

## Must-watch youtube channels

- [Guided Hacking YouTube channel for reverse engineering and game hacking tutorials](https://www.youtube.com/c/GuidedHacking/videos)
- [Stephen Chapman's YouTube channel for Cheat Engine tutorials](https://www.youtube.com/c/StephenChapman/videos)

## Other really useful materials

- More x86 assembly learning material:
    - [x86 Assembly Language Applicable To Reverse Engineering: The Basics – Part 1](https://resources.infosecinstitute.com/x86-assembly-language-applicable-to-reverse-engineering-the-basics-part-1/)
    - [X86 Assembly Language, Part 2](https://resources.infosecinstitute.com/x86-assembly-language-part-2/)
    - Lena151 Assembly Tutorials (might be outdated, but it is still recommended a lot):
        - [LearnThenTeach YouTube channel](https://www.youtube.com/channel/UCVf5kcdOr535bta-XIdeb4Q/videos)
        - [Tuts 4 You - Collection 2011](https://forum.tuts4you.com/files/file/1865-tuts-4-you-collection-2011/)

- Other useful tools and tool guides:
    - [9 Best Reverse Engineering Tools for 2021](https://www.apriorit.com/dev-blog/366-software-reverse-engineering-tools)
    - [Steamless](https://github.com/atom0s/Steamless)
    - [RenderDoc](https://github.com/baldurk/renderdoc)
    - [NirSoft Programmer Tools](https://www.nirsoft.net/programmer_tools.html)
    - [NirSoft Network Tools](https://www.nirsoft.net/network_tools.html)
    - [NirSoft System Tools](https://www.nirsoft.net/system_tools.html)

- Practical reverse engineering and game hacking materials:
    - [Reverse Engineering/Game Patching Tutorial: Full Res Roller Coaster Tycoon with Ghidra+x64dbg+Python](https://www.youtube.com/watch?v=cwBoUuy4nGc)
    - [Reverse Engineering and Weaponizing XP Solitaire (Mini-Course)](https://www.youtube.com/watch?v=ZmPArvsSii4)
    - [DOOM95 | Making an aimbot](https://web.archive.org/web/20200317042324/https://0x00sec.org/t/doom95-making-an-aimbot/19862)
    - [Game Hacking: Hack, Slash, Loot](https://0x00sec.org/t/game-hacking-hack-slash-loot/3711)
    - [User Mode Rootkits: IAT and Inline Hooking](https://0x00sec.org/t/user-mode-rootkits-iat-and-inline-hooking/1108)
    - [x86 API Hooking Demystified](http://jbremer.org/x86-api-hooking-demystified/)
    - [[C/C++] Reverse Engineering Tutorial for newbies](http://rohitab.com/discuss/topic/35537-cc-reverse-engineering-tutorial-for-newbies/)
    - [Reverse Engineering and Function Calling by Address](https://www.codeproject.com/Articles/29527/Reverse-Engineering-and-Function-Calling-by-Addres)
    - [Reverse Engineering Online Games - Dragomon Hunter](https://0xbaadf00dsec.blogspot.com/2016/01/reverse-engineering-online-games.html)
    - [[Tutorial] Packet Hacking and Reversing MMO](https://progamercity.net/ghack-tut/137-tutorial-packet-hacking-reversing-mmo.html)
    - [Run-time directx hooking using code injection and vtable](http://www.rohitab.com/discuss/topic/34411-run-time-directx-hooking-using-code-injection-and-vtable/)
    - [How to implement pattern-scanning to obtain offsets dynamically](https://www.unknowncheats.me/forum/general-programming-and-reversing/133228-implement-pattern-scanning-obtain-offsets-dynamically.html)
    - [C++:How to patch Bytes using PatternScan (AOB) + Explanation / Snippet](https://www.unknowncheats.me/wiki/C%2B%2B:How_to_patch_Bytes_using_PatternScan_(AOB)_%2B_Explanation_/_Snippet)
    - [Reverse engineering a GameBoy Advance game — Complete Guide](https://macabeus.medium.com/reverse-engineering-a-gameboy-advance-game-introduction-ec185bd8e02)

- Bit flags and bit masks:
    - [Bit manipulation with bitwise operators and bit masks](https://www.learncpp.com/cpp-tutorial/bit-manipulation-with-bitwise-operators-and-bit-masks/)

- Books and papers:
    - Reversing and game hacking:
        - [Practical Video Game Bots: Automating Game Processes using C++, Python, and AutoIt - Ilya Shpigor](https://www.amazon.com/Practical-Video-Game-Bots-Automating/dp/1484237358)
        - [Reversing: Secrets of Reverse Engineering - Eldad Eilam](https://www.amazon.com/Reversing-Secrets-Engineering-Eldad-Eilam/dp/0764574817)
        - [X86 Disassembly - Wikibooks.org](https://upload.wikimedia.org/wikipedia/commons/5/53/X86_Disassembly.pdf)
        - [Learning Malware Analysis: Explore the concepts, tools, and techniques to analyze and investigate Windows malware - Monnappa K A](https://www.amazon.com/Learning-Malware-Analysis-techniques-investigate/dp/1788392507)
    - Game programming:
        - [Game Programming Algorithms and Techniques: A Platform-Agnostic Approach - Sanjay Madhav](https://www.amazon.com/Game-Programming-Algorithms-Techniques-Platform-Agnostic/dp/0321940156)
        - [Game Programming Patterns - Robert Nystrom](https://gameprogrammingpatterns.com/contents.html)
    - Windows and Win32 API programming:
        - [Programming Windows: The Definitive Guide To The Win32 Api - Charles Petzold](https://www.amazon.com/Programming-Windows-Definitive-Guide-Win32/dp/9350041057)
        - [Windows Kernel Programming - Pavel Yosifovich](https://www.amazon.com/Windows-Kernel-Programming-Pavel-Yosifovich/dp/1977593372)
        - [Windows Internals - Pavel Yosifovich, Alex Ionescu, Mark E. Russinovich, David A. Solomon](https://www.amazon.com/Windows-Internals-Part-architecture-management/dp/0735684189)
    - Bypassing anti-debugging, anti-reversing, and anti-tamper techniques:
        - [The Ultimate Anti-Reversing Reference - Peter Ferrie](https://anti-reversing.com/Downloads/Anti-Reversing/The_Ultimate_Anti-Reversing_Reference.pdf)
        - [The Art of Unpacking - Mark Vincent Yason](https://www.blackhat.com/presentations/bh-usa-07/Yason/Whitepaper/bh-usa-07-yason-WP.pdf)

- Curated lists of tools, tutorials, resources, and much more for reverse engineering video games:
    - [UnKnoWnCheaTs Game Hacking Wiki](https://www.unknowncheats.me/wiki/UnKnoWnCheaTs_Game_Hacking_Wiki)
    - [The Ultimate Game Hacking Resource](https://github.com/dsasmblr/game-hacking)
    - [The Ultimate Online Game Hacking Resource](https://github.com/dsasmblr/hacking-online-games)
    - [A Study Path for Game Programmer](https://miloyip.github.io/game-programmer/game-programmer.pdf)

- Guided Hacking resources (As of 2023 it is now paywalled content):
    - [GHB1 - Start Here Beginner Guide to Game Hacking](https://guidedhacking.com/threads/start-here-beginners-guide-to-learning-game-hacking.5911/)
    - [GHB2 - Beginners Guide To Reverse Engineering](https://guidedhacking.com/threads/beginners-guide-to-reverse-engineering-tutorial.13446/)
    - [GHB3 - Intermediate Guide to Game Hacking](https://guidedhacking.com/threads/ghb3-intermediate-guide-to-game-hacking.13495/)
    - [How to make an MMO Bot - MMORPG Bot Automation](https://guidedhacking.com/threads/how-to-make-an-mmo-bot-mmorpg-bot-automation.15173/)
    - [Internal vs. External Hacks - What's the difference?](https://guidedhacking.com/threads/internal-vs-external-hacks-whats-the-difference.8808/)

## Useful sites along the way

- [Google](https://www.google.com) (seriously, use it, a lot, all the time)
- [Official Microsoft documentation](https://docs.microsoft.com/en-us/) (includes documentations on MSVC, DirectX, Win32 API, etc.)
- [Godbolt](https://godbolt.org/) (Extremely useful to verify compiler generated C++ code)

## Keywords you want to learn about in general

- Memory scanning
- Memory editing
- Memory patching
- Pattern scanning
- x86 assembly
- x64 assembly
- Process debugging
- Disassembling code
- Decompiling code
- Function hooking
- API hooking
- Detouring functions
- Dll injection
- Internal cheats
- External cheats
- Threads
- Windows PE format
- Win32 API
- Windows internals
- Anti-debugging
- Anti-reversing
- Anti-tamper
- Software packers
- Software unpacking
