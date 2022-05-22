# GitHub
<h1 align="center">GitHub.HW_2</h1>

**1. На локальном репозитории сделать ветки для:**

<h5>-Postman<br>
-Jmeter<br>
-CheckLists<br>
-Bag Reports<br>
-SQL<br>
-Charles<br>
-Mobile testing</h5><br>

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
		
**3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта**
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


**4. Запушить структуру багрепорта на внешний репозиторий**<br>
```
git add .; git commit -m "add BugReports_structure.txt"; git push
```
**5. Вмержить ветку Bag Reports в Main**<br>
```
git checkout main; git merge Bug_Reports
```
**6. Запушить main на внешний репозиторий.**
```
git push
```
**7. В ветке CheckLists набросать структуру чек листа.**<br>
```
git checkout CheckLists
vim CheckLists_structure.txt
```
<i>режим редактирования - i</i>
```
Порядковый номер
Формулировка задачи
Отметка о выполнении либо статусе проверки
```
<i>выйти из режима редактирования с сохранением - Esc :wq Enter</i>

**8. Запушить структуру на внешний репозиторий**
```
git add .; git commit -m "add CheckLists_structure.txt"; git push
```
**9. На внешнем репозитории сделать Pull Request ветки CheckLists в main**<br>
```
Pull requests
CheckLists
Compare & pull request
Create pull request
Merge pull request
Confirm merge
```
**10. Синхронизировать Внешнюю и Локальную ветки Main**<br>
```
git fetch
git pull
```
