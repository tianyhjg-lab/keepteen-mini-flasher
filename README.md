# KEEPTEEN MESHMINI Flasher

The web flasher offers two firmware families for KEEPTEEN MESHMINI:

```text
Meshtastic 2.7.15.d18f3f7
Build date: 2026-07-02

MeshCore v1.15.0
Mode: Bluetooth companion radio
Package date: 2026-07-11
Source revision: 910b1be
Bluetooth name: MeshCore-<node name>
Pairing code: 123456
Power: Type-C powered, reports 4200 mV / 100% battery
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

The MeshCore companion firmware advertises over Bluetooth Low Energy for the
MeshCore mobile client. It is not a USB mass-storage drive.
