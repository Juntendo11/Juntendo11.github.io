#Clean install of wsl

Tried desktop docker 

Tried lab computers and same result...
Clean install wsl

In cmd administrator
# list all installed distros
wsl -l -v

# unregister distros
wsl --unregister Ubuntu
wsl --unregister Debian # and so on

# Search -> App & Features
Search Ubuntu and uninstall

# Search -> Turn off windows features On/Off
Untick Virtual Machine Platform checkbox
Untick Windows Subsystem for Linux checkbox

# Reboot
