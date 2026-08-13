# LAB 1

**Linux commands workflow:**

```text
➜ StudentLab git:(main) mkdir Programs Assignments Notes
➜ StudentLab git:(main) ls
Assignments Notes Programs
➜ StudentLab git:(main) pwd
/home/.../StudentLab
➜ StudentLab git:(main) cd Assignments
➜ Assignments git:(main) touch assignment1.txt
➜ Assignments git:(main) touch assignment2.txt
➜ Assignments git:(main) touch assignment3.txt
➜ Assignments git:(main) ls
assignment1.txt assignment2.txt assignment3.txt
➜ Assignments git:(main) mv assignment3.txt lab3.txt
➜ Assignments git:(main) ls
assignment1.txt assignment2.txt lab3.txt
➜ Assignments git:(main) rm assignment2.txt
➜ Assignments git:(main) ls
assignment1.txt lab3.txt
➜ Assignments git:(main) touch profile.txt
➜ Assignments git:(main) nano profile.txt
➜ Assignments git:(main) cat profile.txt
Name: Student
Enrollment Number: 202612074
Department: MSc IT
Favourite Programming Language: C++

➜ Assignments git:(main) touch report.txt
➜ Assignments git:(main) cp report.txt report_backup.txt
➜ Assignments git:(main) nano report_backup.txt
➜ Assignments git:(main) cat report.txt
➜ Assignments git:(main) cat report_backup.txt
hello this is demo report.

➜ Assignments git:(main) mkdir LinuxLab
➜ Assignments git:(main) cd LinuxLab
➜ LinuxLab git:(main) mkdir C C++ Python Java
➜ LinuxLab git:(main) cd C
➜ C git:(main) touch program1.txt
➜ C git:(main) cd ..
➜ LinuxLab git:(main) cd C++
➜ C++ git:(main) touch program1.txt
➜ C++ git:(main) cd ..
➜ LinuxLab git:(main) cd Python
➜ Python git:(main) touch program1.txt
➜ Python git:(main) cd ..
➜ LinuxLab git:(main) cd Java
➜ Java git:(main) touch program1.txt
➜ Java git:(main) cd ..
➜ LinuxLab git:(main) ls
C C++ Java Python

➜ LinuxLab git:(main) cd ..
➜ Assignments git:(main) mkdir Projects
➜ Assignments git:(main) cd Projects
➜ Projects git:(main) mkdir AI ML DL
➜ Projects git:(main) rmdir ML
➜ Projects git:(main) mv DL DeepLearning
➜ Projects git:(main) ls
AI DeepLearning

➜ Projects git:(main) cd ..
➜ Assignments git:(main) nano isPalindrome.cpp
➜ Assignments git:(main) g++ isPalindrome.cpp -0 isPalindrome
g++: error: unrecognized command-line option ‘-0’
➜ Assignments git:(main) g++ isPalindrome.cpp -o isPalindrome
➜ Assignments git:(main) ./isPalindrome
Enter a string: 121
Palindrome
➜ Assignments git:(main) ./isPalindrome
Enter a string: 122
Not Palindrome

➜ Assignments git:(main) cd ..
➜ StudentLab git:(main) mkdir GitPractice
➜ StudentLab git:(main) cd GitPractice
➜ GitPractice git:(main) git init
Initialized empty Git repository in .../StudentLab/GitPractice/.git/
➜ GitPractice git:(main) touch readme.md
➜ GitPractice git:(main) git add readme.md
➜ GitPractice git:(main) git commit -m "First Commit"
Author identity unknown
fatal: empty ident name not allowed
➜ GitPractice git:(main) git config --global user.name "Student"
➜ GitPractice git:(main) git config --global user.email "student@example.com"
➜ GitPractice git:(main) git commit -m "First Commit"
[main (root-commit)] First Commit
1 file changed, 0 insertions(+), 0 deletions(-)
➜ GitPractice git:(main) git status
On branch main
nothing to commit, working tree clean
➜ GitPractice git:(main) git log

➜ GitPractice git:(main) cd ..
➜ StudentLab git:(main) mkdir Library
➜ StudentLab git:(main) cd Library
➜ Library git:(main) mkdir Books Notes Assignments
➜ Library git:(main) touch Books/booklist.txt
➜ Library git:(main) touch Notes/notes.txt
➜ Library git:(main) touch Assignments/assignment.txt
➜ Library git:(main) cp Books/booklist.txt Notes/
➜ Library git:(main) mv Notes/booklist.txt "Notes/library books.txt"
➜ Library git:(main) rm Assignments/assignment.txt
➜ Library git:(main) cd Books
➜ Books git:(main) ls
booklist.txt
➜ Books git:(main) cd ../Notes
➜ Notes git:(main) ls
library books.txt notes.txt
➜ Notes git:(main) cd ../Assignments
➜ Assignments git:(main) ls

➜ Assignments git:(main) cd ../..
➜ StudentLab git:(main) mkdir Student
➜ StudentLab git:(main) cd Student
➜ Student git:(main) mkdir Programs Documents
➜ Student git:(main) mkdir Documents/Backup
➜ Student git:(main) touch Programs/cpp.cpp
➜ Student git:(main) touch Programs/python.py
➜ Student git:(main) touch Documents/resume.txt
➜ Student git:(main) nano Documents/resume.txt
➜ Student git:(main) cp Documents/resume.txt Documents/Backup/
➜ Student git:(main) mv Documents/Backup/resume.txt "Documents/Backup/resume backup.txt"
➜ Student git:(main) ls
Documents Programs
➜ Student git:(main) cd Documents
➜ Documents git:(main) ls
Backup resume.txt
➜ Documents git:(main) cd Backup
➜ Backup git:(main) ls
resume backup.txt
➜ Backup git:(main) cd ../..
➜ Student git:(main) ls
Documents Programs
➜ Student git:(main) pwd
/home/.../StudentLab/Student
```
