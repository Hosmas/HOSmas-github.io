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
