# Introduction-to-programming-IT603-Lab1-Assignment1
# LINUX PROGRAMMING LABORATORY MINI DEMONSTRATION

## AB 1

**Linux commands workflow:**

### 1. Create Your Personal Workspace

```text
narayan@Asus:~/Sem1/Programming$ mkdir StudentLab
narayan@Asus:~/Sem1/Programming$ cd StudentLab
narayan@Asus:~/Sem1/Programming/StudentLab$ mkdir Programs Assignments Notes
narayan@Asus:~/Sem1/Programming/StudentLab$ ls
Assignments  Notes  Programs
narayan@Asus:~/Sem1/Programming/StudentLab$ pwd
/home/narayan/Sem1/Programming/StudentLab
```

---

### 2. File Management Practice

```text
narayan@Asus:~/Sem1/Programming/StudentLab$ cd Assignments
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ touch assignment1.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ touch assignment2.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ touch assignment3.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ ls
assignment1.txt  assignment2.txt  assignment3.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ mv assignment3.txt lab3.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ rm assignment2.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ ls
assignment1.txt  lab3.txt
```

---

### 3. Creating and Editing Files

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ nano profile.txt
```

**Contents entered in `profile.txt`:**

```text
Name: Narayan
Enrollment Number: __________
Department: MSc IT
Favourite Programming Language: C++
```

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ cat profile.txt
Name: Narayan
Enrollment Number: __________
Department: MSc IT
Favourite Programming Language: C++
```

**Screenshot:**
*Paste screenshot of `profile.txt` / terminal output here.*

---

### 4. File Copy and Backup

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ touch report.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ cp report.txt report_backup.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ nano report_backup.txt
```

**Additional line added to `report_backup.txt`:**

```text
This is just one additional line.
```

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ cat report.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ cat report_backup.txt
This is just one additional line.
```

**Screenshot:**
*Paste screenshot showing both files and their contents here.*

---

### 5. Directory Tree Creation

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ mkdir LinuxLab
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ cd LinuxLab
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments/LinuxLab$ mkdir C C++ Python Java
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments/LinuxLab$ touch C/program1.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments/LinuxLab$ touch C++/program1.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments/LinuxLab$ touch Python/program1.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments/LinuxLab$ touch Java/program1.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments/LinuxLab$ tree .
.
├── C
│   └── program1.txt
├── C++
│   └── program1.txt
├── Java
│   └── program1.txt
└── Python
    └── program1.txt

5 directories, 4 files
```

**Screenshot:**
*Paste screenshot of the `tree` output here.*

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments/LinuxLab$ cd ..
```

---

### 6. Directory Management

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ mkdir Projects
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ mkdir Projects/AI Projects/ML Projects/DL
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ rmdir Projects/ML
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ mv Projects/DL Projects/DeepLearning
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ tree Projects
Projects
├── AI
└── DeepLearning

2 directories, 0 files
```

---

### 7. Compile and Execute a C++ Program

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ nano isPalindrome.cpp
```

**C++ Program Screenshot:**

*Paste screenshot of the complete `isPalindrome.cpp` program here.*

**Compilation:**

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ g++ isPalindrome.cpp -o isPalindrome
```

**Compilation Screenshot:**

*Paste screenshot here.*

**Execution:**

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ ./isPalindrome
Enter a string: git
No git is not palindrome
```

**Output Screenshot:**

*Paste screenshot here.*

**Second Test:**

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Assignments$ ./isPalindrome
Enter a string: ababa
Yes ababa is palindrome
```

**Output Screenshot:**

*Paste screenshot here.*

---

### 8. Git Repository Basics

```text
narayan@Asus:~/Sem1/Programming/StudentLab$ mkdir GitPractice
narayan@Asus:~/Sem1/Programming/StudentLab$ cd GitPractice
narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ git init
Initialized empty Git repository in /home/narayan/Sem1/Programming/StudentLab/GitPractice/.git/
narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ touch readme.md
narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ git add readme.md
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
```

**Screenshot:**
*Paste screenshot of Git initialization, commit, status and log here.*

---

### 9. Mini Linux Project

```text
narayan@Asus:~/Sem1/Programming/StudentLab/GitPractice$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab$ mkdir Library
narayan@Asus:~/Sem1/Programming/StudentLab$ cd Library
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ mkdir Books Notes Assignments
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ touch Books/booklist.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ touch Notes/notes.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ touch Assignments/assignment.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ cp Books/booklist.txt Notes/
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ mv Notes/booklist.txt "Notes/library books.txt"
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ rm Assignments/assignment.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ tree .
.
├── Assignments
├── Books
│   └── booklist.txt
└── Notes
    ├── library books.txt
    └── notes.txt

4 directories, 3 files
```

**Screenshot:**
*Paste screenshot of the final Library structure here.*

---

### 10. Linux Command Challenge

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Library$ cd ..
narayan@Asus:~/Sem1/Programming/StudentLab$ mkdir Student
narayan@Asus:~/Sem1/Programming/StudentLab$ cd Student
narayan@Asus:~/Sem1/Programming/StudentLab/Student$ mkdir Programs Documents
narayan@Asus:~/Sem1/Programming/StudentLab/Student$ mkdir Documents/Backup
narayan@Asus:~/Sem1/Programming/StudentLab/Student$ touch Programs/cpp.cpp
narayan@Asus:~/Sem1/Programming/StudentLab/Student$ touch Programs/python.py
narayan@Asus:~/Sem1/Programming/StudentLab/Student$ touch Documents/resume.txt
narayan@Asus:~/Sem1/Programming/StudentLab/Student$ nano Documents/resume.txt
```

**Contents added to `resume.txt`:**

```text
Name: Narayan
Department: MSc IT
Skills: C++, Linux, Git
```

```text
narayan@Asus:~/Sem1/Programming/StudentLab/Student$ cp Documents/resume.txt Documents/Backup/
narayan@Asus:~/Sem1/Programming/StudentLab/Student$ mv Documents/Backup/resume.txt "Documents/Backup/resume backup.txt"
narayan@Asus:~/Sem1/Programming/StudentLab/Student$ tree .
.
├── Documents
│   ├── Backup
│   │   └── resume backup.txt
│   └── resume.txt
└── Programs
    ├── cpp.cpp
    └── python.py

4 directories, 4 files
narayan@Asus:~/Sem1/Programming/StudentLab/Student$ pwd
/home/narayan/Sem1/Programming/StudentLab/Student
```

**Final Directory Screenshot:**
*Paste screenshot here.*

---

# END OF LINUX PROGRAMMING LABORATORY MINI DEMONSTRATION
