# GitHub
<h1 align="center">GitHub.HW_2</h1>

** 1. На локальном репозитории сделать ветки для:**
-Postman
-Jmeter
-CheckLists
-Bag Reports
-SQL
-Charles
-Mobile testing
```
git clone https://github.com/marg0sh/GitHub.git
cd GitHub

git branch Postman; git branch Jmeter; git branch CheckLists; git branch Bug_Reports; git branch SQL; git branch Charles; git branch Mobile_testing
```

**2. Запушить все ветки на внешний репозиторий**
```
git push -u origin Postman; git push -u origin Jmeter; git push -u origin CheckLists; git push -u origin Bug_Reports; git push -u origin SQL; git push -u origin Charles; git push -u origin Mobile_testing;
```
или

    git push -u origin --all
		
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
````
git checkout BugReports
vim BugReports_structure.txt
````
<i>режим редактирования - i </i>
````
ID
Краткое описание проблемы
Продукт
Платформа
Статус
Приоритет
Серьезность
Предусловия
Шаги воспроизведения
Фактический результат
Ожидаемый результат
Прикрепленные файлы
````
<i>выйти из режима редактирования с сохранением - Esc :wq Enter </i>


Запушить структуру багрепорта на внешний репозиторий
git add .; git commit -m "add BugReports_structure.txt"; git push

Вмержить ветку Bag Reports в Main
git checkout main; git merge Bug_Reports

Запушить main на внешний репозиторий.
git push

В ветке CheckLists набросать структуру чек листа.
git checkout CheckLists
vim CheckLists_structure.txt
режим редактирования - i

Порядковый номер
Формулировка задачи
Отметка о выполнении либо статусе проверки

выйти из режима редактирования с сохранением - Esc :wq Enter

Запушить структуру на внешний репозиторий
git add .; git commit -m "add CheckLists_structure.txt"; git push

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
Pull requests
CheckLists
Compare & pull request
Create pull request
Merge pull request
Confirm merge

10. Синхронизировать Внешнюю и Локальную ветки Main
git fetch
git pull
