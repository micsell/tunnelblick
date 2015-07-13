<font size='3'>Release Notes for Tunnelblick</font>




---


## Version 3.6 ##

**3.6beta08 build 4371 (2015-07-10)**

  * <font color='red'>SECURITY UPDATE:</font>**Replaces OpenSSL version 1.0.2c with version 1.0.2d.
  * Includes additional protection against attacks.
  * Includes additional logging when installer must be run.
  * Updates localization.**


---


**3.6beta06 build 4346 (2015-06-13)**

  * Replaces OpenSSL version 1.0.2b with version 1.0.2c.


---


**3.6beta04 build 4340 (2015-06-12)**

  * Replaces LZO version 2.08 with version 2.09.


---



**3.6beta02 build 4335 (2015-06-12)**

  * <font color='red'>SECURITY UPDATE:</font>**Replaces OpenSSL version 1.0.1m with version 1.0.2b.
  * Includes OpenVPN versions 2.3.7 in addition to 2.3.6.
  * Updates localization, including full Turkish localization and partial Latvian localization.
  * Changes OpenVPN 'verb' default from 1 to 3.
  * Highlights notes, warnings, and errors in the Tunnelblick log.
  * Launches Tunnelblick at login if any 'openvpn' processes are running (or 'openvpnstart' or 'tunnelblick-helper') or if Tunnelblick was running when the user logged out or the computer was shut down or restarted.
  * Includes a modified version of the 'openvpn\_xorpatch' to support the unofficial OpenVPN 'scramble' option. Modifications to the patch include better syntax checking of the option and repair of a buffer overflow bug. Uses the patched version of OpenVPN automatically but only when the configuration file includes the 'scramble' option. For more details, see [Tunnelblick and openvpn\_xorpatch](cOpenvpn_xorpatch.md).
  * Includes better diagnostic info.
  * Reduces non-error logging by tunnelblickd.
  * Fixes problems flushing the DNS cache on some versions of OS X.
  * Fixes problems that affect some TAP connections.
  * Fixes problems with 'Connect when computer starts' configurations.
  * Fixes problems reading configuration files that have CR (0x0D) characters.
  * Fixes misleading output in warnings about IP address changes.
  * Fixes a problem that caused incorrect restore DNS and restore WINS settings when connecting Tunnelblick to an already-running OpenVPN.
  * Fixes problems with Deploy/Welcome.bundle permissions.
  * Fixes typos in help for the 'Appearances' panel.**


---


## Version 3.5 ##

**3.5.3 build 4270.4371 (2015-07-10)**

  * <font color='red'>SECURITY UPDATE:</font>**Replaces OpenSSL version 1.0.1o with version 1.0.1p.**


---


**3.5.2 build 4270.4346 (2015-06-13)**

  * Replaces OpenSSL version 1.0.1n with version 1.0.1o.


---


**3.5.1 build 4270.4335 (2015-06-12)**
  * <font color='red'>SECURITY UPDATE:</font>**Replaces OpenSSL version 1.0.1m with version 1.0.1n.
  * Fixes problems flushing the DNS cache on some versions of OS X.**


---


**3.5.0 build 4265 (2015-04-03)**
  * This is the first stable version of Tunnelblick 3.5 -- many thanks to our tens-of-thousands of beta testers!
  * It is identical to 3.5beta10 except for version and build numbers.

> See [Major Changes from Version 3.4 to Version 3.5](cThreeFiveHighlights.md).


---


**3.5beta10 build 4262 (2015-03-30)**

  * Updates localization and credits.
  * Adds output from the 'ipconfig' command to the diagnostic info.
  * Fixes a problem that caused Tunnelblick to incorrectly report that there are no DNS settings.
  * Fixes a problem that caused Tunnelblick to be unable to perform privileged activity.
  * Fixes several problems when running on OS X 10.4 and 10.5 ("Tiger" and "Leopard").


---


**3.5beta08 build 4236 (2015-03-19)**

  * <font color='red'>SECURITY UPDATE:</font>**Includes OpenSSL 1.0.1m. See [OpenSSL Security Advisory 19 Mar 2015](https://www.openssl.org/news/secadv_20150319.txt).
  * Updates localization for several languages.
  * Adds partial localization for Estonian and Turkish.
  * Adds log entries from helper programs to the output of 'Copy Diagnostic Info to Log'.
  * Fixes problems with configurations that connect when the computer starts.
  * Fixes problems scrolling the log in the 'VPN Details...' window.
  * Fixes problems that caused log entries to not be logged properly.**


---


**3.5beta06 build 4211 (2015-01-22)**

  * Uses a launchd daemon instead of an SUID helper to start OpenVPN on OS X Version 10.5 ("Leopard") and higher.
  * Updates Arabic, Japanese, and Chinese (traditional) localization.
  * Fixes problems with IP address checking on OS X 10.10 ("Yosemite").
  * Fixes problems with the VPN login or passphrase window appearing when waking from sleep or the displays change.
  * Fixes a problem that caused an older version of the tun/tap kexts to be used on OS X 10.6-10.8.
  * Fixes problems with certain malformed updates to Tunnelblick or to configurations.
  * Fixes a problem if certain errors occurred during an update.
  * Fixes a problem showing the failure notification window when an install fails.
  * Fixes a minor memory leak.


---


**3.5beta04 build 4198 (2015-01-08)**

  * <font color='red'>SECURITY UPDATE:</font>**Includes OpenSSL 1.0.1k. See [OpenSSL Security Advisory 08 Jan 2015](https://www.openssl.org/news/secadv_20150108.txt).
  * Adds easy-rsa version 3.0-rc2 to the easy-rsa folder.
  * Adds the per-configuration '-waitForDHCPInfoIfTap' preference which, for TAP configurations, causes the 'up' script to wait until the DHCP info has been processed before continuing with the VPN setup.
  * Adds the 'managementPortStartingPortNumber' preference, which specifies the port number Tunnelblick uses for communication with OpenVPN. If the port is unavailable, successive ports will be tried until an available port is found.
  * Includes complete localization in 20 languages.
  * Flushes DNS cache even if no DNS changes are made by Tunnelblick.
  * Logs additional information about DNS servers being used when connected to the VPN.
  * Fixes problems when Tunnelblick is denied access to the Keychain.
  * Fixes the tab sequencing in the VPN username/password dialog.**



---


**3.5beta02 build 4165 (2014-12-02)**

  * <font color='red'>SECURITY UPDATE:</font>**Includes OpenVPN 2.3.6.  See [OpenVPN Security Announcement-97597e732b](https://community.openvpn.net/openvpn/wiki/SecurityAnnouncement-97597e732b).
  * Includes complete localization in 18 languages including Danish and Greek and partial localization in 7 others, including Arabic and Bulgarian.
  * Uses new (2014-11-04) tun/tap kexts when on OS X 10.9 or 10.10 ("Mavericks" or "Yosemite").
  * Includes new status icon animation which clarifies the connected/connecting/disconnected VPN status -- thanks to William Faulk.
  * Adds the ability to save only the VPN username to the Keychain without saving the VPN password.
  * Adds ability to localize configuration names (and folder names).
  * Moves the 'VPN Details…' menu item to be above the configurations. May be disabled with the 'putVpnDetailsAtBottom' preference is set TRUE.
  * Recreates the status icon only when necessary.
  * Centers the login or passphrase window in the new screen when a screen change occurs or if the computer awakens from sleep unless the 'doNotRedisplayLoginOrPassphraseWindowAtScreenChangeOrWakeFromSleep' preference is set to TRUE.
  * Deletes log files not modified in the last week.
  * An empty name for an 'added menu item' (or the name after translation) causes the item to be skipped.
  * Adds crash report log entries for Tunnelblick components such as openvpn and atsystemstart to the 'Diagnostic Info'.
  * Flushes DNS cache via 'discoveryutil udnsflushcaches' and 'discoveryutil mdnsflushcache' if available.
  * Fixes a problem that caused double-clicks on configurations to not be processed when a window was left open.
  * Fixes several problems with Tunnelblick's handling of 'private keys' (passphrases).
  * Fixes a problem with updates to Deployed versions of Tunnelblick and a problem causing failures on OS X 10.4 ('Tiger').
  * Fixes a problem renaming configurations.
  * Fixes visibility problems with the standard status icon in 'dark mode' on OS X 10.10 ('Yosemite').
  * Fixes problems on OS X 10.4 and 10.5 Intel machines using OpenVPN versions higher than 2.2.1.
  * Fixes a problem with invalid permissions in IconSets contents.
  * Fixes problems that caused digital signature checking to fail on OS X 10.5.
  * Fixes a problem with password and passphrase windows.
  * Fixes status window icon animation.
  * Fixes typo of Feetu Nyrhinen's name on the Info panel.
  * Fixes a problem that caused the 'tun' kext to not be loaded even if 'dev-node tun' was specified in the OpenVPN configuration file.**



---


## Older Versions of Tunnelblick ##

Release notes for older versions are available on the [Old Release Notes page](RlsNotesOld.md).


---


## Uninstaller ##

**Version 1.7 (2015-06-20)**
  * Uninstalls even if the Tunnelblick application has been damaged or does not exist (for example, it has been put in the Trash).
  * Unloads Tunnelblick daemons if they are loaded.
  * Removes OpenVPN and tunnelblickd crash logs.
  * Removes tunnelblickd logs in rebranded versions of Tunnelblick.
  * Removes the temporary authorization icon.
  * Includes better error messages.
  * Fixes a problem that caused the tunnelblickd daemon to be unloaded even when the uninstaller is only being tested.
  * Fixes a problem that displayed a 'Details' button (which was ignored) when certain error conditions arose.
  * Fixes a problem that sometimes caused an error when removing part of the Tunnelblick application.

**Version 1.6 (2015-03-29)**
  * Fixes problems when run on a PowerPC G3 processor.

**Version 1.5 (2015-01-14)**
  * Removes the new entry in /Library/LaunchDaemons made by Tunnelblick 3.4beta05 (build 4204) and higher

**Version 1.4 (2014-09-10)**
  * Removes the new entries in /Library/LaunchDaemons made by Tunnelblick 3.4beta37 (build 2957) and higher

**Version 1.3 (2014-07-10)**
  * Removes the new entry in ~/Library/LaunchAgents made by Tunnelblick 3.4beta32 and higher

**Version 1.2 (2014-02-11)**
  * Fixes a problem causing "application is damaged" warnings on Mavericks
  * Fixes a problem with text being repeated in the opening window
  * Fixes a problem with the opening window not appearing until the Uninstaller icon in the Dock is clicked

**Version 1.1 (2014-01-08)**
  * Removes preferences cache if it is present
  * Warns user if Tunnelblick or OpenVPN is running
  * Ready for localization

**Version 1.0 (2013-03-28)**


---


### PLEASE USE THE [TUNNELBLICK DISCUSSION GROUP](http://groups.google.com/group/tunnelblick-discuss) FOR COMMENTS OR QUESTIONS ###