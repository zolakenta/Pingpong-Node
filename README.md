


![pingpong](https://github.com/user-attachments/assets/3f9816ec-5edd-4c47-b833-fdae7035e5dc)

# Pingpong-Node

[Web Login](https://harvester.pingpong.build) \
[Tutorial Ori](https://docs.pingpong.build/multi-mining-app/run-pingpong-app/configuration-guide)


## Tutor dari Maouam ( Founder Maouam's Node Labs )

### Run PINGPONG
Update paket
```
apt update && apt upgrade -y
```
Install docker jika blm install
```
apt install docker.io -y
```
Install tmux jika belum install
```
apt install tmux -y
```
Buat session tmux
```
tmux new -s pingpong
```
Download pingpong
```
wget https://pingpong-build.s3.ap-southeast-1.amazonaws.com/linux/latest/PINGPONG
```
Beri permission file
```
chmod +x PINGPONG
```
Run pingpong (your_device_id ambil di dashboard web)
```
./PINGPONG --key your_device_id
```
Jika sudah run, keluar dari tmux
``` ctrl b lepas, d```


### Run Other Token opsional ( Tidak Perlu tmux )

OG
```
./PINGPONG config set --0g=your_key
./PINGPONG stop --depins=0g
./PINGPONG start --depins=0g
```
Run aioz
```
./PINGPONG config set --aioz=your_key
./PINGPONG stop --depins=aioz
./PINGPONG start --depins=aioz
```
