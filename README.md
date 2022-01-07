# watch-dogs-plymouth
A Plymouth theme inspired by Watch Dogs.
Forked from [OS1](https://github.com/t-gitt/OS1)

# Preview
_Not yet avaible_

# Installation

### Fedora
```bash
git clone https://github.com/Guaxinim5573/watch-dogs-plymouth.git
cd watch-dogs-plymouth/
sudo cp -r watch-dogs /usr/share/plymouth/themes/
sudo plymouth-set-default-theme watch-dogs -R
```
### Debian
```bash
git clone https://github.com/Guaxinim5573/watch-dogs-plymouth.git
cd watch-dogs-plymouth/
sudo cp -r watch-dogs /usr/share/plymouth/themes/
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/watch-dogs/watch-dogs.plymouth 100
sudo update-alternatives --config default.plymouth
sudo update-initramfs -u
```
> if you are using an encrypted boot drive, replace this line ```:89```  in ```watch-dogs.script```
``` Plymouth.SetRefreshFunction (refresh_callback); ```
with
```Plymouth.SetRefreshFunction (refresh_callback_with_password);```
#### Animation Credit
Ubisoft
[Youtube - WATCH DOGS Full boot animation - FiL0S0V](https://m.youtube.com/watch?v=lEpwxHhUJMg)
