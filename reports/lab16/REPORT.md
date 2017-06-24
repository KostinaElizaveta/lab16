## Laboratory work XVI

Данная лабораторная работа посвещена изучению систем организации совместных сеансов разработки на примере **tmux**

```ShellSession
$ open https://wiki.archlinux.org/index.php/Tmux_(Русский)
```

## Tasks

- [v] 1. Ознакомиться со ссылками учебного материала
- [v] 2. Выполнить инструкцию учебного материала
- [v] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**

## Tutorial

```ShellSession
$ tmux # запуск окна
$ tmux new -s myname #запуск окна с именем myname
```

```ShellSession
$ tmux a #подключение к последнему открытому окну
$ tmux a -t myname # подключение к окну myname
```

```ShellSession
$ tmux ls
0: 1 windows (created Sat Jun 24 17:40:55 2017) [80x23] (attached)
myname: 1 windows (created Sat Jun 24 17:41:13 2017) [80x23] (attached)
$ tmux kill-session -t myname
0: 1 windows (created Sat Jun 24 17:40:55 2017) [80x23] (attached)

```

```ShellSession
<C-B>s
s: команда не найдена
<C-B>$
$: команда не найдена
```

```ShellSession
<C-B>c


<C-B>w
17:46:23 up  4:39,  2 users,  load average: 0,12, 0,10, 0,09
USER     TTY      FROM             LOGIN@   IDLE   JCPU   PCPU WHAT
user     tty7     :0               13:07    4:39m  3:49   0.21s /sbin/upstart -
user     pts/20   tmux(3292).%0    17:40    2.00s  0.07s  0.00s w
<C-B>n
n: команда не найдена
<C-B>p
p: команда не найдена
<C-B>f
f: команда не найдена
<C-B>, #пустой экран
<C-B>& # пустой экран
```

```ShellSession
<C-B>%
<C-B>" # открытие строки
<C-B>o
<C-B>q
<C-B>x
<C-B>+
<C-B>-
<C-B>⍽
```

## Report

```ShellSession
$ cd ~/workspace/labs/
$ export LAB_NUMBER=16
$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}
$ mkdir reports/lab${LAB_NUMBER}
$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
$ cd reports/lab${LAB_NUMBER}
$ edit REPORT.md
$ gistup -m"lab${LAB_NUMBER}"
```

## Links

- [Tmux](https://tmux.github.io)

```
Copyright (c) 2017 Братья Вершинины
```
