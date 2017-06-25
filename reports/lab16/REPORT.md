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
<C-B>s # выбор сессии
<C-B>$ # переименование сессии
```

```ShellSession
<C-B>c # создать новое окно
<C-B>w # выбрать окно из списка
(0)  0: bash- "vershinin"                                                      
(1)  1: bash* "vershinin"    
<C-B>n # следующее окно
<C-B>p # предыдущее окно
<C-B>f # поиск окна
<C-B>, # смена названия окна
<C-B>& # удаление окна
```

```ShellSession
<C-B>% #разделение окон горизонтально
<C-B>" #разделение окна вертикально (получилось 3 окна)
<C-B>o #переход в первое окно
<C-B>q #краткое отображение номера окна
<C-B>x # kill окно 0
<C-B>+ #выбор панели
<C-B>- #удаление буфера
<C-B>⍽ #листаем слои
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
