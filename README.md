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
------------------------
+ 나의 최초 시도
![1번 1차시도](https://user-images.githubusercontent.com/94365974/144589181-ff377111-767d-4346-9262-2471a990783b.gif)

첫 번째 시도에서는 상하좌우 방향키만을 이용하여서 큰따옴표를 삽입할 위치까지 이동했고 그 후에 i(현재 위치에서 입력 시작)하여 " 두 개를 각기 위치에 입력했다.

----------------------------------------
+ 나의 최고점 시도
![1번 2차 시도](https://user-images.githubusercontent.com/94365974/144589376-c1024039-d9ff-4d63-9e57-ec4bc38ec181.gif)
 이번 시도에서는 위의 시도에서 상하좌우 방향키를 통해 이동하는 것은 매우 큰 낭비라고 생각하여 G(파일의 마지막 라인으로 이동)을 이용하여 타자 수를 줄였다.
 그 후에도 A(현재 라인 끝에서 입력 시작)하여 불필요하게 이동할 필요를 없앴고, 라인 끝에 "을 삽입한 후에는 b(단어 단위로 이동)하여 방향키보다 더 적게 다음 위치로 이동하여 "을 삽입했다.
