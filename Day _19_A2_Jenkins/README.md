enkins running slowly on an AWS EC2 t3.micro instance is a common issue, and it's mainly due to the hardware limitations of the instance type. 
Here’s a breakdown of why and what you can do about it:


🛠️ Fixes and Workarounds
✅ 1. Add Swap Memory
You can add a 1–2GB swap file:

``` bash 
sudo fallocate -l 2G /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile
echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab
```

This can drastically improve performance on memory pressure.
