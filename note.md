radarr http://192.168.178.89:7878
sonar: http://192.168.178.89:8989
jellyfinrr  http://192.168.178.89:5055
Jellyfin: http://192.168.178.89:8096
qbittorrent http://192.168.178.89:5080
Mount Point: nfs://192.168.178.247/nfs/qbittorrent
prowlerr http://192.168.178.89:9696
sudo mkdir -p /mnt/qbittorrent
sudo mount -t nfs -o rw,nolock,noatime,norelatime,ac,acregmin=60,acregmax=600,acdirmin=60,acdirmax=600,intr 192.168.178.247:/nfs/qbittorrent /mnt/qbittorrent


sudo tailscale funnel -bg 8123