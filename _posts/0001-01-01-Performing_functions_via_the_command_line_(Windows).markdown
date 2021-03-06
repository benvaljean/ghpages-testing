---
layout: post 
title: Performing functions via the command line (Windows)
---

### Start/Stop Services

    net start servicename
    net stop servicename

### Kill a local process

Download
[pskill](http://technet.microsoft.com/en-us/sysinternals/bb896683.aspx)

    pskill /accepteula
    pskill <process id or name>

### Kill a process on a remote machine

    pskill \\\\hostname -u username <process id or name>

### Reset local account password

    net user username password

### Map a network drive

    net use driveletter: \\\\server\\share

### Show running processes

    tasklist

### Add a user to a local group

    net localgroup localgroupnamehere /add usernamehere

For example to add domain\\\\user to the local administrators group:

    net localgroup Administrators /add domain\\user

### Command line tips

#### Filter/grep output

To show all tasks called notepad:

    tasklist|find "notepad"

#### Command line history

Press F7 or use the up and down cursor keys

#### Append to the %path% variable

    SET PATH=%PATH%;"insert additional path here"

### See Also

-   [Accessing a server remotely when RDP/Terminal services is
    down](Accessing_a_server_remotely_when_RDP/Terminal_services_is_down "wikilink")
-   \[<http://technet.microsoft.com/en-us/library/cc778084(WS.10>).aspx
    Command-line reference A-Z: Scripting\]
-   [The Windows Command Line, Batch Files, and
    Scripting](http://commandwindows.com/)
-   [Command Line Tools \| Free software and tools for Windows
    2003/XP/Vista](http://www.tools4ever.com/products/free/command/)
-   [19 hidden Windows XP
    Secrets](http://300allpctips.blogspot.com/2008/12/19-hidden-windows-xp-secrets.html)

[Category:Windows](Category:Windows "wikilink")
