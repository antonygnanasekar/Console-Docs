---
title: Console Code Pages
description: A code page is a mapping of 256 character codes to individual characters. Different code pages include different special characters, typically customized for a language or a group of languages.
author: bitcrazed
ms.author: richturn
ms.topic: article
ms.prod: console
keywords: console, character mode applications, command line applications, terminal applications, console api
---

# Console Code Pages


A *code page* is a mapping of 256 character codes to individual characters. Different code pages include different special characters, typically customized for a language or a group of languages.

Associated with each console are two code pages: one for input and one for output. A console uses its input code page to translate keyboard input into the corresponding character value. It uses its output code page to translate the character values written by the various output functions into the images displayed in the console window. An application can use the [**SetConsoleCP**](setconsolecp.md) and [**GetConsoleCP**](getconsolecp.md) functions to set and retrieve a console's input code pages and the [**SetConsoleOutputCP**](setconsoleoutputcp.md) and [**GetConsoleOutputCP**](getconsoleoutputcp.md) functions to set and retrieve its output code pages.

The identifiers of the code pages available on the local computer are stored in the registry under the following key.

**HKEY\_LOCAL\_MACHINE\\SYSTEM\\CurrentControlSet\\Control\\Nls\\CodePage**

For information about using the registry functions to determine the available code pages, see [**Registry**](https://msdn.microsoft.com/library/windows/desktop/ms724871).

 

 




