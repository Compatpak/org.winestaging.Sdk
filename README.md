# Wine Staging SDK/Platform
## Building
> **_NOTE:_**  With org.freedesktop.Sdk//25.08 org.freedesktop.Platform//25.08 org.freedesktop.Sdk.Extension.mingw-w64//25.08 org.freedesktop.Sdk.Compat.i386//25.08 org.freedesktop.Sdk.Extension.toolchain-i386//25.08 org.freedesktop.Sdk.Extension.vala//25.08 installed.
```console
flatpak-builder build-dir --repo=../Compatpak/repo --ccache --force-clean --gpg-sign=GPGKey org.winestaging.Sdk.yml
```
## Installing
> **_NOTE:_**  With Compatpak repo added.
```console
flatpak install org.winestaging.Sdk org.winestaging.Platform
```
## Removing
```console
flatpak remove org.winestaging.Platform org.winestaging.Sdk
```
## Updating External Data
> **_NOTE:_**  With org.flathub.flatpak-external-data-checker installed.
```console
flatpak run org.flathub.flatpak-external-data-checker --update org.winestaging.Sdk.yml
```