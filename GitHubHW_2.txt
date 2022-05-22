
GitHub. HW_2
1. На локальном репозитории сделать ветки для:
- Postman
> git branch Postman
- Jmeter
> git branch Jmeter
- CheckLists
> git branch CheckLists
- Bag Reports
> git branch Bag_Reports
- SQL
> git branch SQL
- Charles
> git branch Charles
- Mobile testing
> git branch Mobile_testing

2. Запушить все ветки на внешний репозиторий
> git push origin Postman Jmeter CheckLists Bag_Reports SQL Charles Mobile_testing
or
> git push origin --all
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
> git checkout Bag_Reports 
> cat >>Bugreport_structure.txt
4. Запушить структуру багрепорта на внешний репозиторий
> git add .
> git commit -m "create Bugreport_structure"
> git push --set-upstream origin Bag_Reports
5. Вмержить ветку Bag Reports в Main
> git checkout main
> git merge Bag_Reports -m "add BugReports"
6. Запушить main на внешний репозиторий.
> git pull
> git push
7. В ветке CheckLists набросать структуру чек листа.
> git checkout CheckLists 
> cat >> Checklist_structure
8. Запушить структуру на внешний репозиторий
> git add .
> git commit -am "add txt file"
> git push -u origin CheckLists
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
10. Синхронизировать Внешнюю и Локальную ветки Main
> git checkout main
> git pull
