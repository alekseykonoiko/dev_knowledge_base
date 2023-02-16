mac_pass: b4:2e:99:d8:22:5e

user: server

pass: A140595k

Old controller

ip: 192.168.1.87

user: root

pass: u@dco1ibri

`scp /home/akonoiko/ocr/datasets/docs_dataset2.zip root:192.168.1.87:/root/`

Kampf5: 56.135

Kampf6: 56.211

s1dt: 62.140

systemctl --type=service

systemctl cat videostream

Transfer model to server:

scp dataset_v3_zones1.zip [server@192.168.62.192](mailto:server@192.168.62.192):/home/server/detector/training/models/

**Time settings**

timedatectl set-time 23:38:40

timedatectl

date

timedatectl set-ntp false

cat /etc/timezone

/lib/systemd/systemd-timedated

Anydesk fix

`wget [<http://ftp.us.debian.org/debian/pool/main/p/pangox-compat/libpangox-1.0-0_0.0.2-5.1_amd64.deb>](<http://ftp.us.debian.org/debian/pool/main/p/pangox-compat/libpangox-1.0-0_0.0.2-5.1_amd64.deb>)`

`sudo apt install ./libpangox-1.0-0_0.0.2-5.1_amd64.deb`

sudo apt get install wondershaper

sudo wondershaper eth0 1024 1024

sudo wondershaper clear eth0

To display imx6 tempreture

cat /sys/devices/virtual/thermal/thermal_zone0/temp

```bash
psql --host 'localhost' --port 5432 --username "admin" -w --dbname "detector"
```

```sql
//print all machines
SELECT * FROM machines;
//update machine ip
UPDATE machines SET camera_ip='<http://192.168.56.211:8090/?action=stream>' WHERE id=2;
select * from gui_actions
delete from gui_actions where id between 1 and 10;
select * from orders
delete from orders where id between 6 and 10;

select * from all_speeds where order id = 2;
select * from all_speeds where order_id = 8 and speed >= 500;
s
```
order_id timestamp speed average_speed
stable_speeds
all_speeds

To activate siren
redis-cli -n 4
redis set tale_str_s1dt 1

If status of machines error:
`systemctl restart ws_handler`
and
`date -s '2023-01-06 15:20:56'`
`hwclock --systohc` or `hwclock --hctosys`


detector_speed - (detector/config.ini)
speed_profiler - (speed_profiler/config.ini)

ImpressArt Try&Buy (tb1)
server - 10.65.68.160
camera - http://10.65.68.197:8090/?action=stream
mac: **f0:2f:74:82:d2:e3**
pass: **$QT2wZ**




