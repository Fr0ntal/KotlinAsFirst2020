клонируем
```
git clone https://github.com/Fr0ntal/KotlinAsFirst2020
cd KotlinAsFirst2020
```
добавляем upstream
```
git remote add upstream-my https://github.com/Fr0ntal/KotlinAsFirst2021
git fetch upstream-my
```
создаем ветку backport и заодно переходим в нее
```
git checkout -b backport
```
берем все коммиты с того что указан по конечный и перекидываем в текущую ветку


```
git cherry-pick d535f3592006b8f2593c9f881d72c05164aadc13...FETCH_HEAD
```
доабвляем второй upstream
```
git remote add upstream-theirs https://github.com/Sevdat/KotlinAsFirst2021
git fetch upstream-theirs
```
переход в ветку мастер
```
git checkout master
```
мерgym
```
git merge upstream-theirs/master backport
```
смотрим что выдает данное сочитатание символов
```
git remote -v
```
заливаем все что нам выдает git remote -v в файл remotes
```
git remote -v > remotes
```
добавляем remotes в гит чтобы он за ним следил
```
git add remotes
```
коммит и пуш
```
git commit -m "�� ������"
git push
```
было произведено обновление гита
```
git update-git-for-windows
```
опять пуш
```
git push
```
выгружаем историю команды 
```
doskey /history > howto.md
```
