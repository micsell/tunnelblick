## June 2015 OS X and Application Vulnerabilities ##

**In June 2015, details of four vulnerabilities in OS X and iOS and many applications were released in  [Unauthorized Cross-App Resource Access on MAC OS X and iOS](http://arxiv.org/abs/1505.06836).**

<font color='red'>Tunnelblick is not vulnerable to attacks based on any of these vulnerabilities.</font>

## The "password stealing" (Keychain) vulnerability ##

This vulnerability is caused by applications that modify items stored in the Keychain without checking the access controls on the item. Tunnelblick never modifies an item stored in the Keychain and is thus not vulnerable. To modify an item stored in the Keychain, Tunnelblick deletes the old item and creates a new one with the proper access controls. If an attacker creates a new item after Tunnelblick deletes the old item but before creating the new one (attempting to exploit a possible race condition), Tunnelblick will be unable to create the new item and will report the failure, and the new item Tunnelblick was attempting to create will not be created.

## The "IPC interception" vulnerability ##

This vulnerability is caused by applications that communicate sensitive information using certain interprocess communications ("IPC") mechanisms built into OS X. Although Tunnelblick does communicate sensitive information (usernames, passwords, and passphrases) using IPC mechanisms, it uses different mechanisms than those found to be vulnerable.

## The "container cracking" vulnerability ##

This vulnerability is caused by applications that rely on certain features of the "container" facility built into OS X. Tunnelblick does not use this facility and is thus not vulnerable.

## The "Scheme Hijacking" vulnerability ##

This vulnerability is caused by applications that rely on the "scheme" facility built into OS X. Tunnelblick does not use this facility and is thus not vulnerable.



---


### PLEASE USE THE [TUNNELBLICK DISCUSSION GROUP](http://groups.google.com/group/tunnelblick-discuss) FOR COMMENTS OR QUESTIONS