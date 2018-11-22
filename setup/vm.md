# Setting Up a Windows VM on Mac

1. Download the [Virtual Box](https://www.virtualbox.org/wiki/Downloads)
2. Download the [IE11 for VirtualBox](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/)
3. From the terminal, allow the downloaded file to execute by typing chmod +x filename.sfx on the SFX file only.
4. Run the SFX file from a terminal, such as by ./filename.sfx and it will expand into the OVA you can open with VirtualBox.
5. Open OVA file
6. In Windows VM:
    - Open terminal as an admin `cd C:\Windows\System32\drivers\etc`
    - Update HOSTS file to access local host
    - Open text editor using the run as admin command
    - Open `C:\Windows\System32\drivers\etc\hosts`
    - Add the following entry `10.0.2.2 localhost`
    - You can then use http://10.0.2.2:SomePort to access that port from your mac

Example HOSTS file

```bash
# localhost name resolution is handled within DNS itself.
# 127.0.0.1       localhost
# ::1             localhost

10.0.2.2          localhost
```

*After updates are done make sure to flush the DNS cache*

```bash
dscacheutil -flushcache
```
