# Format USB

## Step 1: Locate USB Drive

```bash
df
```

## Step 2: Unmount and Format USB Drive

### Unmount device
```bash
sudo umount /dev/<your device name>
```

### Format device

* To format a USB drive with FAT32 file system, use:
```bash
sudo  mkfs.vfat /dev/<your device name>
```

* To format a USB drive using NTFS file system run:
```bash
sudo  mkfs.ntfs /dev/<your device name>
```

* To format a USB drive in accordance with exFAT file system use:
```bash
sudo  mkfs.exfat /dev/<your device name>
```


## Step 3: Verify USB Drive Formatting

```bash
sudo fsck /dev/<your device name>
```

