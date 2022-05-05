13.
```sh
PS C:\Users\Janis\Documents\Macibas DevOps\git_repos\module_1> git cat-file -p 'main^{tree}'
040000 tree cb4a85320c63c791759312a23af050fec336baa0    module_1
040000 tree 770f173bc251c9ce6cffb81d327205041a6f7cc7    module_2
PS C:\Users\Janis\Documents\Macibas DevOps\git_repos\module_1> git cat-file -p cb4a85320c63c791759312a23af050fec336baa0
100644 blob 393302525a4720cb278e5611c6d1572224897f8f    README.md
040000 tree b8d46a7a17066d0c0ff341a64a2b1a3fd4544633    img
PS C:\Users\Janis\Documents\Macibas DevOps\git_repos\module_1> git cat-file -p b8d46a7a17066d0c0ff341a64a2b1a3fd4544633
100644 blob 0e6779476ae751a8b26773c9d3b39b56b69efc2a    Git_Screenshot.png
100644 blob b1d324bd94cb9439d6ace19f3eed638b271c8c3a    VS Code_ScreenShot.png
PS C:\Users\Janis\Documents\Macibas DevOps\git_repos\module_1> git cat-file -p 770f173bc251c9ce6cffb81d327205041a6f7cc7
100644 blob e69de29bb2d1d6434b8b29ae775ad8c2e48c5391    README.md
040000 tree b8d46a7a17066d0c0ff341a64a2b1a3fd4544633    img
PS C:\Users\Janis\Documents\Macibas DevOps\git_repos\module_1> git cat-file -p b8d46a7a17066d0c0ff341a64a2b1a3fd4544633
100644 blob 0e6779476ae751a8b26773c9d3b39b56b69efc2a    Git_Screenshot.png
100644 blob b1d324bd94cb9439d6ace19f3eed638b271c8c3a    VS Code_ScreenShot.png
```
Git neredz atšķirību starp dažādiem vienādiem failiem dažādās mapēs.

16.
Izmaiņas Terraform repozitārijā pagājušajā nedēļā
git log --since=25.04.2022 --before=01.05.2022
Otrs variants - 
git log --since="last week"
Šis gan parāda par pēdējām 7 dienām no šodienas

17.
git log --author="Laura Pacilio"

18.
git log --since=01.09.2021 --before=01.10.2021 --author="Laura Pacilio"

19.
git log --author="Laura Pacilio" --since="Yesterday"

*. - 
git log --since=20.04.2021 --before=21.04.2021 --pretty=fuller
commit f8493bf5cd78bc2a723f5ddc6f6bceb0e08813ea
Author:     James Bardin <j.bardin@gmail.com>
AuthorDate: Fri Apr 16 17:11:27 2021 -0400
Commit:     James Bardin <j.bardin@gmail.com>
CommitDate: Tue Apr 20 17:04:56 2021 -0400

Visticamāk izmantots parametrs --date=<date>  kas "pārraksta" autora datumu veicot commit.