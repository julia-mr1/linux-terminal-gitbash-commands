# Gitbash commands homework №1
1) Посмотреть где я:
	pwd

2) Создать папку:
	mkdir group_26

3) Зайти в папку:
	cd group_26

4) Создать 3 папки:
	mkdir folder1 folder2 folder3


	$ ls -la
	total 0
	drwxr-xr-x 1 rus.andru 197609 0 Jan  4 11:52 ./
	drwxr-xr-x 1 rus.andru 197609 0 Jan  4 11:51 ../
	drwxr-xr-x 1 rus.andru 197609 0 Jan  4 11:52 folder1/
	drwxr-xr-x 1 rus.andru 197609 0 Jan  4 11:52 folder2/
	drwxr-xr-x 1 rus.andru 197609 0 Jan  4 11:52 folder3/


5) Зайти в любую папку:
	cd folder1

6) Создать 5 файлов (3 txt, 2 json):
	touch 1.txt 2.txt 3.txt 1.json 2.json

7) Создать 3 папки:
	mkdir folder_1.1 folder_1.2 folder_1.3


8) Вывести список содержимого папки:
	$ ls -la
	total 4
	drwxr-xr-x 1 rus.andru 197609 0 Jan  4 11:56 ./
	drwxr-xr-x 1 rus.andru 197609 0 Jan  4 11:52 ../
	-rw-r--r-- 1 rus.andru 197609 0 Jan  4 11:54 1.json
	-rw-r--r-- 1 rus.andru 197609 0 Jan  4 11:54 1.txt
	-rw-r--r-- 1 rus.andru 197609 0 Jan  4 11:54 2.json
	-rw-r--r-- 1 rus.andru 197609 0 Jan  4 11:54 2.txt
	-rw-r--r-- 1 rus.andru 197609 0 Jan  4 11:54 3.txt
	drwxr-xr-x 1 rus.andru 197609 0 Jan  4 11:56 folder_1.1/
	drwxr-xr-x 1 rus.andru 197609 0 Jan  4 11:56 folder_1.2/
	drwxr-xr-x 1 rus.andru 197609 0 Jan  4 11:56 folder_1.3/


9) Открыть любой txt файл:
	vim 1.txt

10) Написать туда что-нибудь, любой текст:
	i

11) Сохранить и выйти:
	:wq

$ cat 1.txt
	Hi. My name is Julia, and this is my first Git Bash homework!


12) Выйти из папки на уровень выше:
	cd ..
	$ pwd
	/c/Users/rus.andru/git/group_26

13) переместить любые 2 файла, которые вы создали, в любую другую папку:
	mv 2.txt 3.txt ../folder2


14) скопировать любые 2 файла, которые вы создали, в любую другую папку:
	cp 2.txt 3.txt ../folder1


15) Найти файл по имени:

	$ find -name 2.txt
	./group_26/folder1/2.txt
	./group_26/folder2/2.txt



16) просмотреть содержимое в реальном времени 

	tail -f 2.txt


17) вывести несколько первых строк из текстового файла

	head -3 2.txt

	id_01 Apple
	id_02 Apricot
	id_03 Avocado


18) вывести несколько последних строк из текстового файла


	tail -3 2.txt

	id_11 Nectarine
	id_12 Orange
	id_13 Papaya




19) просмотреть содержимое длинного файла (команда less)

	less 2.txt 

вывел в vim:
id_01 Apple
id_02 Apricot
id_03 Avocado
id_04 Banana
id_05 Coconut
id_06 Fig
id_07 Kiwi
id_08 Lemon
id_09 Lime
id_10 Mango
id_11 Nectarine
id_12 Orange
id_13 Papaya
~
~
~
~
~
~
~
~
~
~
(END)


20) вывести дату и время
	$ date
	Tue Jan  4 13:42:50 RTZ 2022

=========

Задание *
1) Отправить http запрос на сервер:
http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000



curl "http://162.55.220.72:5005/terminal-hw-request"
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   237  100   237    0     0   2570      0 --:--:-- --:--:-- --:--:--  2604{"Intro":"Hello!! This is your the first response from server","Tasks":{"Task_1":"Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)","result":["Your_String","Your_number"]}}


rus.andru@DESKTOP-OUO4U02 MINGW64 ~/git (master)
$ ^C

rus.andru@DESKTOP-OUO4U02 MINGW64 ~/git (master)
$ ^C

rus.andru@DESKTOP-OUO4U02 MINGW64 ~/git (master)
$ curl "http://162.55.220.72:5005/get_method?name=Julia&age=30"
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100    15  100    15    0     0    168      0 --:--:-- --:--:-- --:--:--   168["Julia","30"]



2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13


Файлик скрипта:
#!/bin/bash

pwd

# зайти в папку
cd folder1

# создать 3 папки  
mkdir f4 f5 f6

# зайти в любую папку, например, f4
cd f4

# создать 5 файлов
touch 11.txt 22.txt 33.txt 44.json 55.json

# создать 3 папки
mkdir fold_1 fold_2 fold_3

# вывести список содержимого папки
ls -la

# переместить любые 2 файла в другую папку
mv 11.txt 22.txt ../f5

Результат:

$ ./group_26
/c/Users/rus.andru/git/group_26
total 8
drwxr-xr-x 1 rus.andru 197609 0 Jan  4 14:20 .
drwxr-xr-x 1 rus.andru 197609 0 Jan  4 14:20 ..
-rw-r--r-- 1 rus.andru 197609 0 Jan  4 14:20 11.txt
-rw-r--r-- 1 rus.andru 197609 0 Jan  4 14:20 22.txt
-rw-r--r-- 1 rus.andru 197609 0 Jan  4 14:20 33.txt
-rw-r--r-- 1 rus.andru 197609 0 Jan  4 14:20 44.json
-rw-r--r-- 1 rus.andru 197609 0 Jan  4 14:20 55.json
drwxr-xr-x 1 rus.andru 197609 0 Jan  4 14:20 fold_1
drwxr-xr-x 1 rus.andru 197609 0 Jan  4 14:20 fold_2
drwxr-xr-x 1 rus.andru 197609 0 Jan  4 14:20 fold_3
 