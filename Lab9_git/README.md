# C-Programming

### Оценка 3

**1. Смотрим на какой ветке находимся через `git status`**

![](./misc/gitStatus.png)

**2. Выводим `git log`**

![](./misc/gitLog.png)

**3. Создаем файл `sort.c` и вставляем туда функцию сортировки пузырьком**

![](./misc/gitSort.png)

**4. Выводим `git status`**

![](./misc/gitStatus2.png)

**5. Добавим файл `sort.c` в stage**

![](./misc/gitStage.png)

**6. Выводим `git status`**

![](./misc/gitStatus3.png)


**7. Коммитим файл `sort.c` в репозиторий**

![](./misc/gitCommitSort.png)

**8. Выводим `git status`**

![](./misc/gitStatus4.png)

**9. Добавляем любой комментарий в файл `sort.c` ("Bubble Sort")**

![](./misc/gitAddLine.png)

**10. Выводим `git status`**

![](./misc/gitStatus5.png)

**11-12. Добавляем файл `sort.c` и выводим `git status`**

![](./misc/gitAdd&Status.png)

**13. Уберем добавленный ранее комментарий в файле `sort.c`**

![](./misc/gitAdd&Status.png)

**14. Делаем коммит**

![](./misc/gitCommitUnchangedSort.png)

**15. Выводим `git status` и смотрим журнал**

![](./misc/gitStatus6.png)

**16. Добавим в stage и закоммитим последнее изменение**

![](./misc/gitCommitAdd&Remove.png)

**17. Запушим на удаленный репозиторий через `git push`**

![](./misc/gitPush.png)

#### Branches

**1. Cоздадим новую ветку `mybranch` и перейдем на нее через `git checkout -b`**

![](./misc/gitBranch1.png)

**2. Используя `git branch`, увидем на какой ветке находимся**

![](./misc/gitBranch2.png)

**3. На основе предыдущего шага убедимся, что находимся на нужной ветке**

**4. При выводе `git status` заменяется название ветки на текущую (вместо main становится mybranch). Также это изменение видно в терминале VSCode и интерфейсе Git Bash**

![](./misc/gitBranch4.png)

**5-6. Создадим файл `file1.txt` и запишем туда одну строку с именем**

![](./misc/gitBranch6.png)

**7. Добавим файл `file1.txt` и закоммитем это изменение**

![](./misc/gitBranch7.png)

**8. Используя `git log --oneline --graph`, увидем, что ветка указывает на новый коммит**

![](./misc/gitBranch8.png)

**9. Вернемся на ветку `main`**

![](./misc/gitBranch9.png)

**10. Используя `git log --oneline --graph`, увидем, что теперь коммит `dabc0cb` не отображается в последних коммитах ветки main**

![](./misc/gitBranch10.png)

**11. Создадим новый файл `file2.txt` и закоммитем его**

![](./misc/gitBranch11.png)

**12. Используя `git log --oneline --graph --all`, увидем, что ветка указывает на новый коммит, и что теперь у двух веток разные коммиты**

![](./misc/gitBranch12.png)

**13. Переключимся на ветку mybranch**

![](./misc/gitBranch13.png)

**14. Увидим, что файл `file2.txt` пропал из рабочей директории. Это произошло по причине независимости изменений в каждой ветке (изменения, закоммиченные в одной ветке, не затрагивают состояние других веток до момента их слияния)**

![](./misc/gitBranch14.png)

**15. Используя `git diff mybranch master`, увидим разницу между двумя ветками**

![](./misc/gitBranch15.png)