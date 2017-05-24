
## 机器要求

os: CentOS6.x/CentOS7.x 64bit

数量 2 : 1 master,1 slave

mysql版本：5.7

## 部署db


默认root密码在 roles/mysql/defaults/main.yml

创建db及user在 group_vars/mysql

### 修改inventory中集群ip信息

```
vi inventory
```

### 执行playbook

```
ansible-playbook -i inventory mysql.yml

```
