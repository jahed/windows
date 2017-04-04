---
title: Shells
description: 
---

Windows ships with multiple shells. Let's go through them.

> Note: Shells, terminals, consoles etc. have different meanings. Here I'm specifically talking about the prompt and environment they provide.

## Command Prompt

[Command Prompt](https://en.wikipedia.org/wiki/Cmd.exe) (`cmd.exe`) is the oldest and most common shell in Windows. Most of the documentation related to Windows will refer to using this. My advice is to avoid it completely since as far as I can tell, Powershell does everything it can do, and more.

## Powershell

[Powershell](https://en.wikipedia.org/wiki/PowerShell) is the latest official terminal for Windows. Considering this, I highly suggest getting familiar with it.

One of the biggest improvements that came with Powershell is that it provides aliases to a lot of Unix-like commands.

Powershell doesn't *just* provide a terminal, however. It's an entire framework with its own scripting language.

### Powershell ISE

Powershell ISE is an IDE for Powershell scripting, allowing you to debug scripts and have multiple tabs per window.

## Bash on Ubuntu on Windows

One of the latest offerings that came with Windows 10 is the [Linux Subsystem](https://en.wikipedia.org/wiki/Windows_Subsystem_for_Linux). This is essentially a layer on top of Windows that provides a complete Ubuntu environment.

However, the Linux Subsystem is still in Beta and so I suggest avoiding it as much as possible. Updates are rarely released outside of their Windows Beta Participants and there are a lot of missing features. The biggest one at the point of writing this is the lack of being able to list network interfaces which a lot of web-related libraries require.

## Cygwin, MinGW

[Cygwin](https://en.wikipedia.org/wiki/Cygwin) provides a complete Unix environment within Windows with Cygwin-specific builds of the most popular tools available on Unix-like platforms including GCC. As such, it can compile programs to run on Windows via Cygwin and has its own [Bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell)) shell.

[MinGW](https://en.wikipedia.org/wiki/MinGW) is a fork of Cygwin with different design goals. Unlike Cygwin, it allows compiling programs to run on Windows without needing to go through another layer.

I personally haven't had the need to use the major capabilities of what Cygwin and MinGW provide over the alternatives so I can't recommend either.

## Conclusion

To conclude, for general development on Windows, I suggest using Powershell as it's officially supported by Microsoft. It provides useful aliases to Unix commands without needing to have an entire Unix layer on top of your Windows installation.