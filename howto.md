1.Форкаем репозиторий https://github.com/Kotlin-Polytech/KotlinAsFirst2020 и клонируем git clone
2.Добавляем upstream git remote add upstream-my https://github.com/tokci4/KotlinAsFirst2021
3.Фетчим из апстрима git fetch upstream-my
4.Создаем ветку backport и переходим в нее git checkout -b backport
5.Переносим коммиты в backport git cherry-pick d535f359...FETCH_HEAD
6.Добавляем второй апстрим: git remote add upstream-theirs https://github.com/Nikikikson/KotlinAsFirst2021
7.git fetch upstream-theirs
8.Возвращемся в master: git checkout master
9.Мерджим: git merge backport upstream-theirs/master
10.Разрешаем конфликты
11.git commit
12.git remote -v
13.git commit
14.Создаём howto.md и пишем ход решения 
15.git commit + git push 
