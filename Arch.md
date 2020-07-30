## Arch stuff as well as some general stuff

Change the caps key to work as esc key
[[https://linux.die.net/man/1/setxkbmap|setxkbmap]]
`setxkbmap -option caps:escape`

[[https://wiki.archlinux.org/index.php/bluetooth#Front-ends|Bluetooth]]
If bluetooth does not turn on in networkmanager it might not be running
Check status
`systemctl status bluetooth`
If down, then start it
`systemctl start bluetooth`



