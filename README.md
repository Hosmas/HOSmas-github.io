# HOSmas-github.io
오픈소스SW개론 2차 과제

# 문제1. Add quotes to ansible playbook
---------------------------------------
```
//Start file
- hosts: all
  vars:
    ssh_state: True
  tasks:
    - name: Manage openssh
      package:
        name: openssh
        state: {{ ssh_state }}
```

```
//End file
- hosts: all
  vars:
    ssh_state: True
  tasks:
    - name: Manage openssh
      package:
        name: openssh
        state: "{{ ssh_state }}"
```
첫번째 시도

![1번 1차시도](https://user-images.githubusercontent.com/94365974/144589181-ff377111-767d-4346-9262-2471a990783b.gif)
