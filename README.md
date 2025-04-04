# comigo-quattro-kartina-tv
Hacking KartinaTV tv box (OEM Comigo Quattro)

```
root@SB522:/storage/external_storage/sda1 # ls /dev/block
boot
cache
data
env
logo
loop0
loop1
loop2
loop3
loop4
loop5
loop6
loop7
mmcblk0
mmcblk0boot0
mmcblk0boot1
platform
pri_gpt
recovery
recovery_bak
reserved
sda
sda1
sec_gpt
system
vold

root@SB522:/storage/external_storage/sda1 # dd if=/dev/block/boot of=boot.img
32768+0 records in
32768+0 records out
16777216 bytes transferred in 1.060 secs (15827562 bytes/sec)
```
# Debloat
```
root@SB522:/ # pm disable com.comigo.cloud
root@SB522:/ # pm disable ru.start.kartinatv
root@SB522:/ # pm disable com.comigo.kartina.kiosk
root@SB522:/ # pm disable com.comigo.rootkeeper
```
