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
```
ziyixie@ZIYIdeMacBook-Pro exercises % git start commit-one-file
Preparing the exercise environment, hold on...
Exercise commit-one-file started!
Read the README.md for instructions or view them in browser:
http://gitexercises.fracz.com/e/commit-one-file

ziyixie@ZIYIdeMacBook-Pro exercises % ls
A.txt		B.txt		README.md	start.sh

ziyixie@ZIYIdeMacBook-Pro exercises % cat README.md 
## Commit one file
There are two files created in the root project directory - `A.txt` and `B.txt`.

The goal is to commit only one of them.

NOTE: Remember that you can submit your solutions with `git verify` command instead of `git push`.

ziyixie@ZIYIdeMacBook-Pro exercises % git status
位于分支 commit-one-file
您的分支与上游分支 'origin/commit-one-file' 一致。

未跟踪的文件:
  （使用 "git add <文件>..." 以包含要提交的内容）
	A.txt
	B.txt

提交为空，但是存在尚未跟踪的文件（使用 "git add" 建立跟踪）

ziyixie@ZIYIdeMacBook-Pro exercises % git add A.txt

ziyixie@ZIYIdeMacBook-Pro exercises % git status
位于分支 commit-one-file
您的分支与上游分支 'origin/commit-one-file' 一致。

要提交的变更：
  （使用 "git restore --staged <文件>..." 以取消暂存）
	新文件：   A.txt

未跟踪的文件:
  （使用 "git add <文件>..." 以包含要提交的内容）
	B.txt

ziyixie@ZIYIdeMacBook-Pro exercises % git commit -m "commit A.txt"
[commit-one-file df257d0] commit A.txt
 1 file changed, 1 insertion(+)
 create mode 100644 A.txt

ziyixie@ZIYIdeMacBook-Pro exercises % git verify                  
Verifying the commit-one-file exercise. Hold on...
Exercise: commit-one-file        
Status: PASSED        
You can see the easiest known solution and further info at:        
https://gitexercises.fracz.com/e/commit-one-file/mqla        

Next task: merge-conflict        
In order to start, execute: git start next        

See your progress and instructions at:        
https://gitexercises.fracz.com/c/mqla 
```
```
ziyixie@ZIYIdeMacBook-Pro exercises % git start commit-one-file-staged
Preparing the exercise environment, hold on...
Exercise commit-one-file-staged started!
Read the README.md for instructions or view them in browser:
http://gitexercises.fracz.com/e/commit-one-file-staged

ziyixie@ZIYIdeMacBook-Pro exercises % ls
A.txt		B.txt		README.md	start.sh

ziyixie@ZIYIdeMacBook-Pro exercises % git status
位于分支 commit-one-file-staged
您的分支与上游分支 'origin/commit-one-file-staged' 一致。

要提交的变更：
  （使用 "git restore --staged <文件>..." 以取消暂存）
	新文件：   A.txt
	新文件：   B.txt

ziyixie@ZIYIdeMacBook-Pro exercises % git reset A.txt

ziyixie@ZIYIdeMacBook-Pro exercises % git status
位于分支 commit-one-file-staged
您的分支与上游分支 'origin/commit-one-file-staged' 一致。

要提交的变更：
  （使用 "git restore --staged <文件>..." 以取消暂存）
	新文件：   B.txt

未跟踪的文件:
  （使用 "git add <文件>..." 以包含要提交的内容）
	A.txt

ziyixie@ZIYIdeMacBook-Pro exercises % git commit -m "Commit B.txt file"
[commit-one-file-staged 8508780] Commit B.txt file
 1 file changed, 1 insertion(+)
 create mode 100644 B.txt

ziyixie@ZIYIdeMacBook-Pro exercises % git verify
Verifying the commit-one-file-staged exercise. Hold on...
Exercise: commit-one-file-staged        
Status: PASSED        
You can see the easiest known solution and further info at:        
https://gitexercises.fracz.com/e/commit-one-file-staged/mqla        

Next task: merge-conflict        
In order to start, execute: git start next        

See your progress and instructions at:        
https://gitexercises.fracz.com/c/mqla 
```
```
ziyixie@ZIYIdeMacBook-Pro exercises % git start ignore-them
Preparing the exercise environment, hold on...
Exercise ignore-them started!
Read the README.md for instructions or view them in browser:
http://gitexercises.fracz.com/e/ignore-them

ziyixie@ZIYIdeMacBook-Pro exercises % git branch
  another-piece-of-work
  commit-one-file
  commit-one-file-staged
* ignore-them
  master
  merge-conflict

ziyixie@ZIYIdeMacBook-Pro exercises % git status
位于分支 ignore-them
您的分支与上游分支 'origin/ignore-them' 一致。

未跟踪的文件:
  （使用 "git add <文件>..." 以包含要提交的内容）
	file.txt
	libraries/
	output.o
	program.exe

提交为空，但是存在尚未跟踪的文件（使用 "git add" 建立跟踪）


```

