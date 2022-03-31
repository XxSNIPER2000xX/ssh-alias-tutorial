# ssh-alias-tutorial
simple tutorial on using a config file to alias your remote device


<h2>Introduction</h2>

this tutorial will change something like this:
```
ssh username@remote.device.ip
scp username@remote.device.ip:somefile ./somefile
```

into something like this 😎:
```
ssh your_alias
scp your_alias:somefile ./somefile
```

<h2>Steps</h2>

open a text editor to ```~/.ssh/config```

write or copy and paste:
```
Host your_alias
User remote_username
Host remote_ip_adress
```
replace your_alias with what you want your alias to be

replace remote_username with the username of your remote device

replace remote_ip_adress with the ip address of your remote device, can be found using ```ifconfig``` on the remote device

save the file

complete!!
