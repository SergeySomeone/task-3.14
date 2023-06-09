## Первый git add и git commit!

В предыдущей главе мы с вами создали клон удаленного репозитория у себя на ПК. В созданной папке находится один файл - readme.md. Так дело не пойдет! Давайте добавим файлы нашего будущего проекта в папку, а заодно и в удаленный репозиторий.
Первая команда, которая нам понадобится - **`git add`**.
Что же она делает? Эта команда добавляет изменение из рабочего каталога в раздел проиндексированных файлов. Она сообщает Git, что вы хотите включить изменения в конкретном файле или все изменения в следующий commit (про него позже).
Создайте в вашем локальном репозитории файл project.md.
Здесь же открываем GitBash как это было указано ранее и прописываем:
``` bash=
git add . (для добавления всех созданных илит измененных файлов)
git add project.md (для добавления конкретного файла)
```
Готово? Отлично! Только что вы добавили ваш файл в раздел проиндексированных файлов. 
Дальше необходимо как бы зафиксировать ваше действие. Для этого существует команда **`git commit`**. Для начала давайте разберемся что же такое commit в Git.
Простыми словами, commit это фиксация изменений в файле(-ах) вашего репозитория. Как бы контрольные точки (точки сохранения) вашего проекта. Благодаря этим точкам вы всегда сможете найти и откатить версию вашего проекта на необходимую вам стадию. Ошибка в программе? Не надо пролистывать весь код и тратить уйму времени на поиск конфликта. Достаточно просто откатить программу на верситю назад - на commit назад. 
И так, в том же окне GitBash пропишем:
```bash=
git commit -m "add file project.md"
```
***-m "add file project.md"** в данном случае является сообщением для разработчиков из вашей команды о том, что вы добавили файл с соответствующим названием. Ну или напоминалка для себя самого, чтобы вспомнить суть внесенных изменений*

Вот вы и создали свой первый `commit`! Но это еще не все! Теперь необходимо отправить ваш подготовленный файл в удаленный репозиторий. Как? [Листай дальше и узнаешь!](./push.md)
#
*[< к содержанию](/readme.md)*