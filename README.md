This is an educational repository that contains homeworks, completed as part of Vadim Ksendzov's training course on software testing. Here I am learning how to work in GitHub. Below is my homework and solution
# GitHub. HW_2
## 1. На локальном репозитории сделать ветки для:
### - Postman
### - Jmeter
### - CheckLists
### - Bug Reports
### - SQL
### - Charles
### - Mobile testing
```
$ git branch Postman
$ git branch Jmeter
$ git branch CheckLists
$ git branch Bug_Reports
$ git branch SQL
$ git branch Charles
$ git branch Mobile_testing
```
## 2. Запушить все ветки на внешний репозиторий
```
$ git push origin --all

Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/demiurgusnen9/Homework_Gitbranch_Masalskaya.git
 * [new branch]      Bug_Reports -> Bug_Reports
 * [new branch]      Charles -> Charles
 * [new branch]      CheckLists -> CheckLists
 * [new branch]      Jmeter -> Jmeter
 * [new branch]      Mobile_testing -> Mobile_testing
 * [new branch]      Postman -> Postman
 * [new branch]      SQL -> SQL
```
## 3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта
```
$ git checkout Bug_Reports
Switched to branch 'Bug_Reports'
```
```
$ vim bug_report.txt
 ID:ID 
 Summary:Короткое описание
 Steps to Reproduce: Шаги воспроизведения
 Expected Result:Ожидаемый результат
 Actual Result:Фактический результат
 Severity:Серьезность
```
## 4. Запушить структуру багрепорта на внешний репозиторий
```
$ git add . && git commit -m "add bug_report.txt"
 warning: LF will be replaced by CRLF in bug_report.txt.
 The file will have its original line endings in your working directory
 [Bag_Reports 3471c3e] add bug_report.txt
 1 file changed, 6 insertions(+)
 create mode 100644 bug_report.txt
```
```
$ git push --set-upstream origin Bug_Reports
 Enumerating objects: 4, done.
 Counting objects: 100% (4/4), done.
 Delta compression using up to 2 threads
 Compressing objects: 100% (3/3), done.
 Writing objects: 100% (3/3), 481 bytes | 481.00 KiB/s, done.
 Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
 To https://github.com/demiurgusnen9/Homework_Gitbranch_Masalskaya.git
 725d855..3471c3e  Bug_Reports -> Bug_Reports
 branch 'Bug_Reports' set up to track 'origin/Bug_Reports'.
```
## 5. Вмержить ветку Bug Reports в Main
```
$ git checkout main
  Switched to branch 'main'
  Your branch is up to date with 'origin/main'.
$ git merge Bag_Reports
  Updating 725d855..3471c3e
  Fast-forward
  bug_report.txt | 6 ++++++
  1 file changed, 6 insertions(+)
  create mode 100644 bug_report.txt
```
## 6. Запушить main на внешний репозиторий.
```
$ git push
 Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
 To https://github.com/demiurgusnen9/Homework_Gitbranch_Masalskaya.git
 725d855..3471c3e  main -> main
```
## 7. В ветке CheckLists набросать структуру чек листа.
```
$ git checkout CheckLists
 Switched to branch 'CheckLists'

```
## 8. Запушить структуру на внешний репозиторий
```
$ git add . && git commit -m "add checkList.txt"
$  git push --set-upstream origin CheckLists
 Enumerating objects: 4, done.
 Counting objects: 100% (4/4), done.
 Delta compression using up to 2 threads
 Compressing objects: 100% (3/3), done.
 Writing objects: 100% (3/3), 506 bytes | 506.00 KiB/s, done.
 Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
 To https://github.com/demiurgusnen9/Homework_Gitbranch_Masalskaya.git
 725d855..56b161b  CheckLists -> CheckLists
 branch 'CheckLists' set up to track 'origin/CheckLists'.
```
## 9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
```
done
```
## 10. Синхронизировать Внешнюю и Локальную ветки Main
```
$ git pull
 remote: Enumerating objects: 4, done.
 remote: Counting objects: 100% (4/4), done.
 remote: Compressing objects: 100% (2/2), done.
 remote: Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
 Unpacking objects: 100% (2/2), 748 bytes | 149.00 KiB/s, done.
 From https://github.com/demiurgusnen9/Homework_Gitbranch_Masalskaya
 3471c3e..ecea53d  main       -> origin/main
 Updating 3471c3e..ecea53d
 Fast-forward
 checkList.txt | 2 ++
 1 file changed, 2 insertions(+)
 create mode 100644 checkList.txt
```
