Role Name
=========
ubuntu_setup_docker_role

## Description
UbuntuでDockerを使うための環境構築用のロール

## Requirements
ansible

使い方
-----

#### インストール
以下のような `requirements.yml` を用意する。

```yml
---
roles:
  - src: git+git@github.com:realglobe-Inc/ubuntu_setup_docker_role.git
```
次のコマンドでロールをインストールできます。

```console
ansible-galaxy install -r requirements.yml
```

#### Playbook内での利用

```yml
- hosts: servers
  become: yes
  roles:
    - role: ubuntu_setup_docker_role
````
