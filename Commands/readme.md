# Diffenrent Commands used in CNNA 👩‍💻
* [Initialize Router and Reload](#initialize-router-and-reload)
* [Initialize Switch and Reload](#initialize-switch-and-reload)

Use a `?` after any command to see it's proper syntax
</br>

## Initialize ROUTER and Reload
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

## Initialize SWITCH and Reload
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

