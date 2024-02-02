https://gitexercises.fracz.com/
```sh
ziyixie@ZIYIdeMacBook-Pro ~ % git clone https://gitexercises.fracz.com/git/exercises.git
正克隆到 'exercises'...
remote: Enumerating objects: 150, done.
remote: Counting objects: 100% (150/150), done.
remote: Compressing objects: 100% (112/112), done.
remote: Total 150 (delta 35), reused 150 (delta 35)
接收对象中: 100% (150/150), 33.85 KiB | 173.00 KiB/s, 完成.
处理 delta 中: 100% (35/35), 完成.

ziyixie@ZIYIdeMacBook-Pro ~ % ls
Applications			Downloads			Music				Public				go
Desktop				Library				OneDrive			exercises			iCloud云盘（归档）
Documents			Movies				Pictures			github-learning-xie		许可.pdf

ziyixie@ZIYIdeMacBook-Pro ~ % cd exercises

ziyixie@ZIYIdeMacBook-Pro exercises % git config user.name "myname"

ziyixie@ZIYIdeMacBook-Pro exercises % git config user.email "myemail@example.com"

ziyixie@ZIYIdeMacBook-Pro exercises % ./configure.sh
OK

ziyixie@ZIYIdeMacBook-Pro exercises % git start
Preparing the exercise environment, hold on...
Exercise master started!
Read the README.md for instructions or view them in browser:
http://gitexercises.fracz.com/e/master

ziyixie@ZIYIdeMacBook-Pro exercises % ls
README.md	configure.sh	start.sh	test.txt

ziyixie@ZIYIdeMacBook-Pro exercises % cat README.md 
## Push a commit you have made

The first exercise is to push a commit that is created when you run the `git start` command.

Just try `git verify` after you have initialized the exercises and be proud of passing the first one :-)
```
```sh
ziyixie@ZIYIdeMacBook-Pro exercises % git start
Preparing the exercise environment, hold on...
Exercise master started!
Read the README.md for instructions or view them in browser:
http://gitexercises.fracz.com/e/master

ziyixie@ZIYIdeMacBook-Pro exercises % git verify
Verifying the master exercise. Hold on...
Exercise: master        
Status: PASSED        
You can see the easiest known solution and further info at:        
https://gitexercises.fracz.com/e/master/mqla        

Next task: merge-conflict        
In order to start, execute: git start next        

See your progress and instructions at:        
https://gitexercises.fracz.com/c/mqla 
```
