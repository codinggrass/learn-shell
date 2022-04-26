### sh

#### 执行脚本使用shell引擎
- `./test.sh` 需要sh脚本具备可执行权限，首先检查test.sh脚本第一行是否有`#!/bin/bash`指定选用的
引擎，如果有则选用改引擎，如没有则使用当前用户默认指定的引擎。`cat /etc/passwd` 可查看默认sh引擎

- `/home/user/test.sh` 和上述情况一致

- `sh /home/user/test.sh` 使用用户默认shell引擎，将`/home/user/test.sh`作为参数传入shell

- `/bin/ksh test.sh` 指定某种shell进行执行，优先级高于脚本中第一行指定