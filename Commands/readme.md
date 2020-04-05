# Diffenrent Commands used in CNNA 👩‍💻
* [Initialize Router and Reload](#initialize-router-and-reload-)
* [Initialize Switch and Reload](#initialize-switch-and-reload-)
* [Show Version](#show-version-)
* [Configure Clock](#configure-clock-)
* [Configure Switch](#configure-switch-)


Use a `?` after any command to see it's proper syntax

</br>

## Initialize ROUTER and Reload ▶
Start by Pressing `enter` on the keybaord. Afterwards Enter Privilaged EXEC Mode by using enable command:
```console
enable
```
or
```console
en
```
<hr/>

Next Erase Prevoius Configurations
```console
erase startup-config
```
or
```console
erase st
```
<hr/>

Next use Reload Command
```console
reload

```
<hr/>

Next You May Be Promted with the following:

* System Configuratiuons Has Been Modified. Save? [yes/no]: `no`
* Would you like to enter the initial configuration dialog? [yes/no]: `no`
* Would you like to terminate autoinstall? [yes/no]: `yes`

</br>

## Initialize SWITCH and Reload ▶
Start by Pressing `enter` on the keybaord. Afterwards Enter Privilaged EXEC Mode by using enable command:
```console
enable
```
or
```console
en
```
<hr/>
Detirmine if there is any VLAN (Virtual local-area networks) Enabled

```console
show flash
```

If the vlan.dat file is found, delete it

```console
delete vlan.dat
```

<hr/>


Next Erase Prevoius Configurations

```console
erase startup-config
```
or
```console
erase st
```
<hr/>

Next use Reload Command
```console
reload

```
<hr/>

Next You May Be Promted with the following:

* System Configuratiuons Has Been Modified. Save? [yes/no]: `no`
* Would you like to enter the initial configuration dialog? [yes/no]: `no`
* Would you like to terminate autoinstall? [yes/no]: `yes`

</br>

## Show Version ✔
```console
show version
```

</br>

## Configure Clock 🕒
Display Current Clock
```console
show clock
```

<hr/>

Enter Exec Mode
```console
en
```

<hr/>

Use the following sytax to set the clock `clock set Time Month Date Year`. For this example we will use 15:08 on October 26th 2012
```console
clock set 15:08:00 Oct 26 2012
```
</br>

## Configure Switch ⚙
Enter EXEC
```console
en
```

<hr/>

Configure Terminal
```console
configure terminal
```
or
```console
conf t
```

<hr/>

Set Name For this example name will be: `S1`
```console
hostname S1
```

<hr/>

Prevent Unwanted DNS Lookup
```console
no ip domain-lookup
```

<hr/>

Enter Local Password, Prevent un authorized users. For this example password is: `cisco`
```console
enable secret class
line con 0
password cisco
login
exit
```

<hr/>

Configure MOTD Banner
```console
banner motd #
```

<hr/>

Enter your message. End command with: `#`. For this example we will use `Your Message Here` as the MOTD Banner
```console
Your Message Here#
```

<hr/>

Save Configurations to Startup
```console
copy running-config startup-config
```

<hr/>

Show Current Running Configurations
```console
show running-config
```


