# NTOSKRNL
Include ntoskrnl in kernel-mode programs.

> [!WARNING]
> <b>The main purpose of this project is to integrate ntoskrnl.lib in Native-API apps,<br>
> So don't to use this in drivers.</b>


## How to use?

First make sure that your program is using the latest Windows SDK. 

Next you need to include ntoskrnl64 or ntoskrnl86 (located in .\lib) to your Visual Studio Project

Last add this two lines to your source file

```
#define _X86_ // Project architecture (_X86_  or _AMD64_)
#include <ntoskrnl.hpp>
```
First Line is Project Architecture that is set in BUILD

Second Line includes ntoskrnl header

# LICENSE: MIT
Copyright (c) 2025 RuSHeRRE2

