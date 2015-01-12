# sskm
Simple Ssh Key Manager for Linux (and possibly Unix)

##### Looking for programmmers
Right now there is nothing but the concept and some sketches. I'm not a good enough programmer to get this going and I don't have the time to become one. If you're interested in this project, just let me know and I'll add you as a collaborator.

### Usecase
Imagine a small network of Linux and Unix machines withthout centralized authentication instances like LDAP or NIS. This might be the case in a home network (NAS, mobile phones, notebooks, VCRs,...) or in small sports clubs. Setting up Kerberos would be overkill and you might not have root on all machines anyway. You log into the various devices and machines via **ssh** and would like to **facilitate the management of your public keys**.

### UI sketches and description of functionality

The program consists of three tabbed panels "Manage Hosts", "Manage Keys" and "Key Distribution".

#### Main Menu / Manage Hosts

![Main Menu / Manage Hosts](https://raw.githubusercontent.com/jniggemann/sskm/master/UI_sketches/01_main.png)

This is how the program could look like when started. The first panel "Manage Hosts" is shown and the user can:
 - Add a new account@host
 - Edit an existing account@host
 - Delete an existing account@host
 - Show all public keys available on account@host

##### Manage Hosts: Context Menu
These actions are available on right-clicking on a host entry. The context menu could look like this:
![Main Menu / Manage Hosts - context menu](https://raw.githubusercontent.com/jniggemann/sskm/master/UI_sketches/02_right_click_on_host.png)

##### Manage Hosts: add / edit host
![Main Menu / Manage Hosts - add/edit host](https://raw.githubusercontent.com/jniggemann/sskm/master/UI_sketches/03_add_new_or_edit_host.png)

##### Manage Hosts: List keys
![Main Menu / Manage Hosts - list keys](https://raw.githubusercontent.com/jniggemann/sskm/master/UI_sketches/04_list_all_keys_on_host.png)

#### Manage Keys

![Manage Keys](https://raw.githubusercontent.com/jniggemann/sskm/master/UI_sketches/05_manage_keys.png)
Actions the user can perform (through the context menu):
 - Add new public key from file
 - Delete public key
 - Show all hosts this key is on
 
 ##### Manage Keys: Context menu
![Manage Keys - context menu](https://raw.githubusercontent.com/jniggemann/sskm/master/UI_sketches/06_right_click_on_key.png)

 ##### Manage Keys: Add new key
![Manage Keys - add new key from file](https://raw.githubusercontent.com/jniggemann/sskm/master/UI_sketches/07_add_new_key.png)
