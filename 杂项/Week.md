# Linux

### 进程



+ **ps**（Photoshop）：用来查看目前系统中有哪些正在执行的进程和他们的执行情况。

  PID：进程识别号

  TTY：终端机号

  TIME：进程所占用CPU时间

  START：进程开始时间

  CMD（COMMAND）：正在执行的进程名或命令

  VSZ：虚拟内存占用情况

  RSS：使用物理内存情况

  STAT：进程状态。S—休眠、r—运行、Z—僵尸进程、D—短期等待

  ps -a：显示当前所有进程信息

  ps -u：已用户格式

  ps -x：后台进程运行的运行参数

  ps -aux、ps -ef：全格式显示所有进程及父进程

  

+ **kill**、**killall**：终止进程

  kill [选项] 进程号

  kill 进程名（也支持通配符）

  踢出一个非法用户：ps -aux |grep sshd、kill 进程号 -9

  终止远程登录

+ pstree -pu

  -p：显示进程pid

  -u：所属用户

+ setup：查看服务

+ ls /etc/init.d:查看服务

+ vi /etc/inittab：查看默认或修改默认级别

