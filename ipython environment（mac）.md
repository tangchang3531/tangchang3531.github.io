##Ipython 环境搭建
###1. 软件准备
1. Download boot2docker
2. Open mac shell， and type“boot2docker ssh”
3. In docker shell, clone the repo. Eg:"bigdata-mindstorms/ipython-playground"

  $ git clone https://github.com/bigdata-mindstorms/ipython-playground
4. Find the folder

  cd /Users/changtang/ipython-playground

    if cant find the folder:

    1. In mac shell, type: pwd
    2. type: ls
    3. type: cd ipython-playground
    4. type: ls
    5. type: ./docker-ipython       (until you see [1])
    6. type: % run hello.py(hello.py is an example)
    7. you will see "hello"

5. In mac shell
    1. type: cd
    2. clone the repo again
    3. type: cd ipython-playground
    4. type: pwd(you will see absolute path of the repo)

6. In docker shell
    1. type: cd /Users/changtang/ipython-playground

    //Mac shell has your folder-/Users/changtang/ipython-playground,but it only runs BSD Unix.Docker only runs in linux(a version of UNIX).boot2docker gives you a virtual linux machine. They share the same folder. But you can only run "./docker-ipython" in the Linux VM

    2. % run hello.py (until you see[1])
7. Find the repo in Atom, and edit hello.py in the folder home.
8. Commit the change in Mac shell:
    1. type: cd /User/changtang/ipython-playground
    2. type: git status
    3. type: git add .
    4. type: git commit -m "your comment"
    5. type: git push

9. Now you can add plain.py in the home folder,using atom to edit it. Find the ipython-playground, and

Notice:

1. If computer crashed, you still need to type: boot2docker ssh,.

2. If you have "Conflict".
    1. In docker shell,type: docker ps
    2. In Mac shell, type: docker ps -a
    3. In mac shell, type: docker rm e73("e73" is just an example)
    4. Now the dead container has gone
3. oNCE YOU HAVE RAN "./build-image", you will see "image.id" and "image.log", that means you dont need to build image again.


Two ways to run the script:
1. REPL
2. bATCH MODE
