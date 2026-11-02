# LR6
Лабораторная работа №6
## Ход работы

1. Делаем fork [fork](screenshots/fork.png)

2. Клонируем репозиторий [clone](screenshots/git%20clone.png)

3. Добавляем новый файл [add new_file.txt](screenshots/add%20new%20file.png)

4. Коммитим добавление файла [commit new file](screenshots/commit%20adding%20a%20new%20file.png)

5. Подтягиваем изменения локально [pull to local](screenshots/git%20pull%20changes%20to%20local%20repo.png)

6. Создаем и изменяем файлы в новой ветке [new branch work](screenshots/new%20branch%20changes.png)

7. Получаем историю и последние изменения в ветках [changes in branches](screenshots/get%20history%20and%20last%20changes%20for%20branches.png)

8. Мёрджим ветку feature в мастер и удаляем feature [merge feature into master, then delete](screenshots/merge%20feature%20into%20master,%20delete%20feature.png)

9. Создаем файл [create file](screenshots/extra%20file%20created.png)

10. Коммитим создание файла [commit file creation](screenshots/extra%20file%20committed.png)

11. Удаляем файл [delete file](screenshots/extra%20file%20deleted.png)

12. Коммитим удаление файла [commit file deletion](screenshots/extra%20file%20deletion%20committed.png)

13. Откат коммита [revert commit](screenshots/commit%20revert.png)


## Лог комманд

git config --global user.name "4541vRanevskayaAD"
git config --global user.email "donniedarko2018@mail.ru"
git clone https://github.com/4541vRanevskayaAD/LR6.git
cd LR6

git pull origin master

git checkout -b feature
git add.
git commit -m "changed new_file.txt"
git push -u origin feature

git log --oneline master
git log --oneline feature
git log -5 HEAD
git show HEAD
git checkout master
git log -5 HEAD
git show HEAD

git merge feature
git add.
git commit -m "merge feature"
git branch -d feature
git push origin --delete feature

git revert HEAD

git checkout -b report
git add.
git commit -m "screenshots folder created"
git push -u origin report

git add.
git commit -m "report started"
git push -u origin report

git add.
git commit -m "report command log added"
git push -u origin report

git log --pretty=format:"%h | %ad | %an | %s" --date=short

git add.
git commit -m "all screenshots added"
git push -u origin report