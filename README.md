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
+첫번째 시도
![1번 1차시도](https://user-images.githubusercontent.com/94365974/144589063-1833fa68-b600-482e-b549-1d67a9b31377.gif)
