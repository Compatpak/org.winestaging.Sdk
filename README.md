# Wine Staging SDK/Platform
## Building
> **_NOTE:_**  With org.freedesktop.Sdk//24.08 org.freedesktop.Platform//24.08 org.freedesktop.Sdk.Extension.mingw-w64//24.08 org.freedesktop.Sdk.Compat.i386//24.08 org.freedesktop.Sdk.Extension.toolchain-i386//24.08 installed.
```console
flatpak run org.flatpak.Builder build-dir --repo=../Compatpak/repo --ccache --force-clean org.winestaging.Sdk.yml
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