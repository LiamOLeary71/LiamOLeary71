## Lab 01

- Name: Liam O'Leary
- Email: Oleary.23@wright.edu

## Part 1 - GitHub Profile

1. [ LiamOLeary71 Profile](https://github.com/LiamOLeary71)

## Part 2 - Research

| Windows | Linux / Mac | Action |
| ---     | ---         | ---    |
| help    | man         |   displays help     |
| Get-Location |  cmd  |    gets path for SYS 32  |
| Get-ChildItem | ls    |    tons of files i honestly don't know looks like windows files   |
|  mkdir  |    mkdir    |    makes a directory    |
| Set-Location | cd     |     sets where directory is located   |
| New-Item | touch      |    new item like a directory  or file |
| Move-Item | mv        |    moving item within or outside directory    |
| Copy-Item | cp        |     copying item within directory   |
| Remove-Item | rm      |     removing an item   |
| notepad.exe | vim     |   notepad     |

## Part 3 - Command Line Navigation

My OS is:
- [x] Windows
- [] Linux
- [] Mac

My Command Line Shell is: power-shell

### Navigating My OS on the Command Line

1. Create a directory named `DirA`: New-Item -Path . -Name "DirA" -ItemType Directory
2. Create a directory named `Dir B`: New-Item -Path . -Name "DirB" -ItemType Directory
3. Go into `DirA`: Set-Location -Path ".\DirA"
4. Go into `Dir B` from `DirA`: Set-Location -Path "..\DirB"
5. Return to your user's home directory: Set-Location -Path Olear
6. Create a file named `test.txt`: New-Item -Path . -Name "test.txt" -ItemType File
7. Move the file named `test.txt` into `DirA`: Move-Item -Path ".\test.txt" -Destination ".\DirA"
8. Contents of `test.txt`: Set-Content -Path ".\DirA\test.txt"
```
Lots of words just huge amount of words enough words that it is a lot more words than the word words lots of words though in this words word word teehee
```
9. Make a copy of `test.txt` named `copy.txt` in `DirA`: Copy-Item -Path ".\DirA\test.txt" -Destination ".\DirA\copy.txt"
10. View the contents of `DirA`: Get-ChildItem -Path ".\DirA"
11. Make a copy of `test.txt` in `Dir B` named `fodder.txt`: Copy-Item -Path ".\DirA\test.txt" -Destination ".\Dir B\fodder.txt"
12. Delete / remove both `fodder.txt` AND `Dir B`: Remove-Item -Path ".\Dir B\fodder.txt" -Force
Remove-Item -Path ".\Dir B" -Recurse -Force

## Citations

To add citations, provide the cite and a summary of what it assisted you with.  If generative AI was used, include which generative AI system was used and what prompt(s) you fed it.



