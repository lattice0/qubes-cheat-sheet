# qubes-cheat-sheet
Some things that I need to setup in Qubes in case of reinstalls


on sys-usb, activae internet for a moment and do
```
sudo dnf install pcsc-lite qubes-gpg-split
sudo service pcscd start
```

so yubikey works on sys-usb and can be used from all VMs
