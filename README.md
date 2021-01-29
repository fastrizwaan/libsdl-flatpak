# libsdl-flatpak
libsdl 1.2 required for games like bit trip beat on linux

### libsdl 1.2.15 module for flatpak 20.08 runtime 

#Build
```
flatpak-builder --force-clean build-dir libsdl1.2.15.yaml
flatpak-builder --install --user --force-clean build-dir libsdl1.2.15.yaml
```
# run
```
flatpak run org.libsdl.sdl
```


