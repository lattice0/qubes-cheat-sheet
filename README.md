# qubes-cheat-sheet
Some things that I need to setup in Qubes in case of reinstalls


on sys-usb, activae internet for a moment and do
```
sudo dnf install pcsc-lite qubes-gpg-split
sudo service pcscd start
```

so yubikey works on sys-usb and can be used from all VMs. Don't forget to run

```
export QUBES_GPG_DOMAIN=sys-usb
```

on each VM to inform which domain to use as GPG split

TODO: does it work if we do

```
echo "export QUBES_GPG_DOMAIN=sys-usb" >> ~/.profile
```
?
