## 检出代码
在开发主机上执行下面的git复制代码
```
git clone --recursive https://github.com/CodePlayerBox/docker-pi-box.git
```

## 构建运行

1. 在开发主机上，通过Ansible将代码同步到树莓派上
```
cd playbooks
ansible-playbook -i inventories/hosts deploy-to-rpi.yml
```

2. 在树莓派上，执行下面的命令进行构建
```
cd ~/CodePlayerBox/docker-pi-box
docker-compose build
```

3. 进入script目录下，然后执行下面的命令启动
```
cd script
./pi_box start
