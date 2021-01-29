# libsdl-flatpak
libsdl 1.2 required for games like bit trip beat on linux

### libsdl 1.2.15 module for flatpak 20.08 runtime 

# install flatpak requirements
```
sudo dnf install flatpak-builder flatpak; #fedora
sudo apt install flatpak-builder flatpak; #debian / ubuntu

flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
flatpak install flathub org.freedesktop.Platform/x86_64/20.08 org.freedesktop.Sdk/x86_64/20.08
```

#Build
```
flatpak-builder --force-clean build-dir libsdl1.2.15.yaml
flatpak-builder --install --user --force-clean build-dir libsdl1.2.15.yaml
```
# run
```
flatpak run org.libsdl.sdl
```


