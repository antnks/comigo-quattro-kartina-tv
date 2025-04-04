# Hacking KartinaTV tv box

```
root@SB522:/ # cat /proc/cpuinfo
Processor	: ARMv7 Processor rev 1 (v7l)
processor	: 0
BogoMIPS	: 7.52

processor	: 1
BogoMIPS	: 7.52

processor	: 2
BogoMIPS	: 7.52

processor	: 3
BogoMIPS	: 7.52

Features	: swp half thumb fastmult vfp edsp neon vfpv3 tls vfpv4
CPU implementer	: 0x41
CPU architecture: 7
CPU variant	: 0x0
CPU part	: 0xc05
CPU revision	: 1

Hardware	: Amlogic Meson8B
Revision	: 000a
Serial		: 1b00000000000000

root@SB522:/ # free -m
             total         used         free       shared      buffers
Mem:           799          732           67            0           16
-/+ buffers:                715           84
Swap:            0            0            0

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
root@SB522:/ # pm disable com.comigo.welcome
root@SB522:/ # pm disable com.comigo.remoteshellconnector
root@SB522:/ # pm disable com.comigo.cloud.res
root@SB522:/ # pm disable com.comigo.welcome
root@SB522:/ # pm disable com.comigo.tr069client
root@SB522:/ # pm disable com.comigo.applicationupdater
root@SB522:/ # pm disable com.comigo.upgrader
root@SB522:/ # pm disable com.comigo.tv
root@SB522:/ # pm disable com.comigo.payment.stb
root@SB522:/ # pm disable com.comigo.operator.stb
```
