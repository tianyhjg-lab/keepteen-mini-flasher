# KEEPTEEN MINI 本地刷机页

## 本地打开

在本目录运行一个静态服务器，然后用 Chrome 或 Edge 访问：

```powershell
python -m http.server 8088
```

打开：

```text
http://localhost:8088/flash.html
```

## 固件写入地址

```text
0x000000  bin/bootloader.bin
0x008000  bin/partitions.bin
0x010000  bin/firmware.bin
```
