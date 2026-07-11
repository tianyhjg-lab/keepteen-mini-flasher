# KEEPTEEN MINI Flasher

The web flasher offers two firmware families for KEEPTEEN MINI:

```text
Meshtastic 2.7.15.d18f3f7
Build date: 2026-07-02

MeshCore
Mode: USB companion radio
```

Open:

```text
https://tianyhjg-lab.github.io/keepteen-mini-flasher/flash.html
```

Flash layout:

```text
0x000000  bin/bootloader.bin
0x008000  bin/partitions.bin
0x010000  bin/firmware.bin
```

MeshCore files are kept separately under `bin/meshcore/` and are declared in
`manifest-meshcore.json`. Do not mix the bootloader, partition table, or
firmware files between the two manifests.
