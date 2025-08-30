wget https://raw.githubusercontent.com/wucd18/cn-ip-block/refs/heads/main/block-ips.sh

chmod +x block-ips.sh

./block-ips.sh

# 添加到crontab
sudo crontab -e

# 每周一凌晨3点更新
0 3 * * 1 /usr/local/bin/block-ips.sh update
演示

1、封禁IP

<img width="587" height="226" alt="image" src="https://github.com/user-attachments/assets/3acdd8df-3693-42ee-b649-bae2bf83b430" />


2、查看封禁列表

<img width="589" height="153" alt="image" src="https://github.com/user-attachments/assets/b3f88473-d9de-4f2a-9f83-5ea7e2cad126" />


3、解封IP

<img width="590" height="168" alt="image" src="https://github.com/user-attachments/assets/188f24c5-460c-4dd1-841a-9c599bec0439" />


总结
一键屏蔽可以有效帮我们暂时防止一些CC攻击等，或者你不想让哪国的人进入博客也可以用，注意屏蔽cn的时候需谨慎，不然你SSH就上不去了。
