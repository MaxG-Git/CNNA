# Diffenrent Commands used in CNNA 👩‍💻
* [Initialize Router and Reload](#initialize-router-and-reload-)
* [Initialize Switch and Reload](#initialize-switch-and-reload-)
* [Configure Switch](#configure-switch-)
* Some Simple Commands
    * [Enter Exec](#enter-exec)
    * [Erase Config](#erase-config)
    * [Configure Clock](#configure-clock-)
    * [Show Vlan](#show-vlan)
    * [Show Version](#show-version-)
    * [Status of Connected Interface](#status-of-connected-interface-)
    * [Configure Terminal](#configure-terminal)
    * [Configure MOTD Banner](#configure-motd-banner)


Use a `?` after any command to see it's proper syntax

</br>


## Initialize ROUTER and Reload ▶
#### Enter Exec

**[`^        back to top        ^`](#)**

Start by Pressing `enter` on the keybaord. Afterwards Enter Privilaged EXEC Mode by using enable command:
```console
enable
```
or
```console
en
```
<hr/>

#### Erase Config t

**[`^        back to top        ^`](#)**

Next Erase Prevoius Configurations
```console
erase startup-config
```
or
```console
erase st
```
<hr/>

Next use Reload Command to erase any old config info from memory.
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

**[`^        back to top        ^`](#)**

Start by Pressing `enter` on the keybaord. Afterwards Enter Privilaged EXEC Mode by using enable command:
```console
enable
```
or
```console
en
```
<hr/>

#### Show VLAN

**[`^        back to top        ^`](#)**

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

**[`^        back to top        ^`](#)**

```console
show version
```
</br>

## Status of Connected Interface ✔

**[`^        back to top        ^`](#)**

```console
show ip interface brief
```

</br>

## Configure Clock 🕒

**[`^        back to top        ^`](#)**

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

**[`^        back to top        ^`](#)**

Enter EXEC
```console
en
```

<hr/>

#### Configure Terminal

**[`^        back to top        ^`](#)**

Enter Configure Terminal Mode
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

#### Configure MOTD Banner

**[`^        back to top        ^`](#)**

This is the warning messaged displayed when trying to acess. I.E. "Unothorized access prohibeted"
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


