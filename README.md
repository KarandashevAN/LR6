# LR6
Лабораторная работа №6


***Порядок выполнения работы***
1. Создать аккаунт на сайте GitHub.

![Рисунок 1](screenshots/1.png)

2. Сделать копию в личное хранилище из 
https://github.com/Kurtyanik/LR6/ (Fork).

![Рисунок 2](screenshots/2.png)

![Рисунок 3](screenshots/3.png)

![Рисунок 4](screenshots/4.png)

3. Установить Git (https://git-scm.com/).

4. После установки настроить клиент git, введя имя пользователя (Группа 
Фамилия И.О.) и email.

![Рисунок 5](screenshots/5.png)

5. Клонировать свой личный удалённый репозиторий на компьютер.

![Рисунок 6](screenshots/6.png)

![Рисунок 7](screenshots/7.png)

6. Добавить файл через интерфейс GitHub. Подтянуть изменения в 
локальный репозиторий.

![Рисунок 8](screenshots/8.png)

![Рисунок 9](screenshots/9.png)

![Рисунок 10](screenshots/10.png)

![Рисунок 11](screenshots/11.png)

![Рисунок 12](screenshots/12.png)

7. Получить историю операций для каждой из веток.

![Рисунок 13](screenshots/13.png)

![Рисунок 14](screenshots/14.png)

![Рисунок 15](screenshots/15.png)

8. Просмотреть последние изменения.

![Рисунок 16](screenshots/16.png)

9. Выполнить слияние в ветку master, разрешив конфликт (можно 
использовать специальные редакторы или графический интерфейс git).

![Рисунок 17](screenshots/17.png)

![Рисунок 18](screenshots/18.png)

![Рисунок 19](screenshots/19.png)

![Рисунок 20](screenshots/20.png)

![Рисунок 21](screenshots/21.png)

![Рисунок 22](screenshots/22.png)

10. Удалить побочную ветку после успешного слияния.

Удаление в локальном репозитории.

![Рисунок 23](screenshots/23.png)

![Рисунок 24](screenshots/24.png)

Удаление в удаленном репозитории.

![Рисунок 25](screenshots/25.png)

![Рисунок 26](screenshots/26.png)

11. Сделать изменения и зафиксировать их, оставляя комментарии, 
несколько раз.

![Рисунок 27](screenshots/27.png)

![Рисунок 28](screenshots/28.png)

12. Сделать откат коммита.

![Рисунок 29](screenshots/29.png)

![Рисунок 30](screenshots/30.png)

13. Создать ветку для отчёта.

![Рисунок 31](screenshots/31.png)

![Рисунок 32](screenshots/32.png)

# Лог команд
```
git config --global user.name "B3441 Karandashev A N"
git config --global user.email karandashevaleksey.guap@gmail.com
git clone https://github.com/KarandashevAN/LR6.git
git pull origin master
git log master
git checkout -b branch1 origin/branch1
git log branch1
git log -p
git checkout master
git merge branch1
git diff
git commit -m "Merged after resolving conflict"
git branch -d branch1
git push -d origin branch1
git add file1.txt
git commit -m "Create file1.txt"
git add file2.txt
git commit -m "Create file2.txt"
git reset --hard HEAD~1
git push
git checkout -b report
git push --set-upstream origin report
```

# История операций
```
commit 1f1ab82a4c8dc16c96c774c2bcc4c88b6e54f948 (HEAD -> master, origin/master, origin/HEAD)
Author: B3441 Karandashev A N <karandashevaleksey.guap@gmail.com>
Date:   Tue Nov 5 15:36:06 2024 +0300

    Create file1.txt

commit 913d6afacc4a5561356f16e482c6ab3d18fe8ad5
Merge: 041d00c 0f9f50d
Author: B3441 Karandashev A N <karandashevaleksey.guap@gmail.com>
Date:   Tue Nov 5 15:29:13 2024 +0300

    Merged after resolving conflict

commit 041d00ca390e5cf13f7116b4afa05074a78e6e27
Author: KarandashevAN <karandashevaleksey.guap@gmail.com>
Date:   Tue Nov 5 15:06:01 2024 +0300

    Create file.txt

commit 921f53b8d0cebf542c791cf31f04e9b792f385a4
Author: Kurtyanik <45309985+Kurtyanik@users.noreply.github.com>
Date:   Sat Nov 21 20:09:49 2020 +0300

    Обновление информации

commit 0f9f50db68a6983b47398017545532cd0f992846
Author: Kurtyanik <45309985+Kurtyanik@users.noreply.github.com>
Date:   Sat Nov 21 20:08:33 2020 +0300

    Заполнил файл

commit c08a654a63cfc3a7146b2b7015884d9020f5cbf5
Author: Kurtyanik <45309985+Kurtyanik@users.noreply.github.com>
Date:   Sat Nov 21 20:02:16 2020 +0300

    Файл создан пустым

commit 3c6e9131bb47ed6009c28226afb0535c7f6d5964
Author: Kurtyanik <45309985+Kurtyanik@users.noreply.github.com>
Date:   Sat Nov 21 19:58:20 2020 +0300

    Initial commit
```
