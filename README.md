# Snap package for RTL-SDR tools

[![Snap Package](https://snapcraft.io/rtlsdr/badge.svg)](https://snapcraft.io/rtlsdr)

This snap provides the [RTL-SDR](https://osmocom.org/projects/rtl-sdr) tools.

It can be installed from the store via:

```bash
    sudo snap install rtlsdr
```

The `rtl_<name>` tools will be available as `rtlsdr.<name>` .


## Connecting interfaces

After install, some snap interfaces need to be connected manually for the tools to be able to access devices:


```bash
    sudo snap connect rtlsdr:raw-usb
    sudo snap connect rtlsdr:network-observe
```


## TCP service

The `rtl_tcp` tool is also available as a managed service in the snap.

It's shipped disabled by default. To enabled it, with the device connected, run 

```bash
    sudo snap start rtlsdr
```


[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/rtlsdr)
