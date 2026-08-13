LAB 1

Linux commands workflow:

narayan@Asus:~$ pwd
/home/narayan

narayan@Asus:~$ mkdir StudentLab
narayan@Asus:~/Sem1/Programming$ cd StudentLab/
narayan@Asus:~/Sem1/Programming/StudentLab$ mkdir Programs Assignments Notes
narayan@Asus:~/Sem1/Programming/StudentLab$ ls
Assignments Notes Programs
narayan@Asus:~/Sem1/Programming/StudentLab$ pwd
/home/narayan/Sem1/Programming/StudentLab

narayan@Asus:~/Sem1/Programming/StudentLab$ cd Assignments/
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ touch assignment1.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ touch assignment2.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ touch assignment3.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ ls
assignment1.txt  assignment2.txt  assignment3.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ mv assignment3.txt lab3.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ ls
assignment1.txt  assignment2.txt  lab3.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ rm assignment2.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ ls
assignment1.txt  lab3.txt

narayan@Asus:~/Sem1/Programming/StudentLab$ ls
Assignments Notes Programs
narayan@Asus:~/Sem1/Programming/StudentLab$ cd Notes/
narayan@Asus:~/Sem1/Programming/StudentLab/Notes$ nano profile.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Notes$ cat profile.txt
hello there, this is demo text.

narayan@Asus:~/Sem1/Programming/StudentLab/Notes$ touch report.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Notes$ nano report.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Notes$ cat report.txt
hello this is demo report.
narayan@Asus:~/Sem1/Programming/StudentLab/Notes$ cp report.txt report_backup.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Notes$ cat report_backup.txt
hello this is demo report.

narayan@Asus:~/Sem1/Programming/StudentLab$ mkdir LinuxLab
narayan@Asus:~/Sem1/Programming/StudentLab$ cd LinuxLab/
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab$ mkdir C C++ Python Java
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab$ cd C
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab/C$ touch program1.txt
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab/C$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab$ cd C++/
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab/C++$ touch program1.txt
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab/C++$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab$ cd Python/
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab/Python$ touch program1.txt
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab/Python$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab$ cd Java/
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab/Java$ touch program1.txt
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab/Java$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab/LinuxLab$ ls
C  C++  Java  Python

narayan@Asus:~/Sem1/Programming/StudentLab$ mkdir Projects
narayan@Asus:~/Sem1/Programming/StudentLab$ cd Projects/
narayan@Asus:~/Sem1/Programming/StudentLab/Projects$ mkdir AI ML DL
narayan@Asus:~/Sem1/Programming/StudentLab/Projects$ rmdir ML
narayan@Asus:~/Sem1/Programming/StudentLab/Projects$ ls
AI DL ML
narayan@Asus:~/Sem1/Programming/StudentLab/Projects$ mv DL DeepLearning
narayan@Asus:~/Sem1/Programming/StudentLab/Projects$ ls
AI DeepLearning

narayan@Asus:~/Sem1/Programming/StudentLab/Projects$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab$ cd Programs/
narayan@Asus:~/Sem1/Programming/StudentLab/Programs$ nano Palindrome.cpp
narayan@Asus:~/Sem1/Programming/StudentLab/Programs$ g++ -o output Palindrome.cpp
narayan@Asus:~/Sem1/Programming/StudentLab/Programs$ ./output

Enter a string: 121
Palindrome

narayan@Asus:~/Sem1/Programming/StudentLab/Programs$ ./output
Enter a string: 122
Not Palindrome

narayan@Asus:~/Sem1/Programming/StudentLab$ mkdir GitPractice
narayan@Asus:~/Sem1/Programming/StudentLab$ cd GitPractice/
narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ git init

Initialized empty Git repository in /home/narayan/Sem1/Programming/StudentLab/GitPractice/.git/

narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ touch readme.md
narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ git add readme.md
narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ git commit -m "First Commit"

Author identity unknown

*** Please tell me who you are.
Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.

fatal: empty ident name (for <narayan@Asus.localdomain>) not allowed

narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ git config --global user.name "Narayan"
narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ git config --global user.email "narayandarbar73@gmail.com"
narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ git commit -m "First Commit"
[master (root-commit) b52a3b4] First Commit
1 file changed, 0 insertions(+), 0 deletions(-)
create mode 100644 readme.md

narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ git status
On branch master
nothing to commit, working tree clean
narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ git log
commit b52a3b4d0c8de509ab281e2b58ea3b1914a14958 (HEAD -> master)
Author: Narayan <narayandarbar73@gmail.com>
Date:   Wed Aug 12 11:28:22 2026 +0000

First Commit

narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ 

narayan@Asus:~/Sem1/Programming/StudentLab$ mkdir Library
narayan@Asus:~/Sem1/Programming/StudentLab$ cd Library/
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ mkdir Books Notes Assignments
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ touch Books/booklist.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ touch Notes/notes.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ touch Assignments/assignment.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ cp Books/booklist.txt Notes/
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ mv Notes/booklist.txt "Notes/library books.txt"
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ rm Assignments/assignment.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ cd Books/
narayan@Asus:~/Sem1/Programming/StudentLab/Library/Books$ ls
booklist.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Library/Books$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ cd Notes/
narayan@Asus:~/Sem1/Programming/StudentLab/Library/Notes$ ls
library books.txt  notes.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Library/Notes$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ cd Assignments/
narayan@Asus:~/Sem1/Programming/StudentLab/Library/Assignments$ ls

narayan@Asus:~/Sem1/Programming/StudentLab/Library/Assignments$ 

narayan@Asus:~/Sem1/Programming/StudentLab$ cd Programs/
narayan@Asus:~/Sem1/Programming/StudentLab/Programs$ mkdir Student
narayan@Asus:~/Sem1/Programming/StudentLab/Programs$ cd Student/
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ mkdir Documents
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ mkdir Documents/Backup
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ mkdir Programs
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ ls
Documents Programs
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ touch Programs/cpp.cpp
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ touch Programs/python.py
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ touch Documents/resume.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ nano Documents/resume.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ cp Documents/resume.txt Documents/Backup/
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ mv Documents/Backup/resume.txt "Documents/Backup/resume backup.txt"
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ ls
Documents Programs
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ cd Documents/
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student/Documents$ ls
Backup resume.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student/Documents$ cd Backup/
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student/Documents/Backup$ ls
resume backup.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student/Documents/Backup$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student/Documents$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ cd Programs/
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student/Programs$ ls
cpp.cpp  python.py
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student/Programs$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ ls
Documents Programs
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$ pwd
/home/narayan/Sem1/Programming/StudentLab/Programs/Student
narayan@Asus:~/Sem1/Programming/StudentLab/Programs/Student$
