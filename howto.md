cd C:\Users\user\IdeaProjects
git clone https://github.com/Fr0ntal/KotlinAsFirst2020
cd KotlinAsFirst2020
git remote add upstream-my https://github.com/Fr0ntal/KotlinAsFirst2021
git fetch upstream-my
git checkout -b backport
git cherry-pick d535f3592006b8f2593c9f881d72c05164aadc13...FETCH_HEAD
git remote add upstream-theirs https://github.com/Sevdat/KotlinAsFirst2021
git fetch upstream-theirs
git checkout master
git merge upstream-theirs/master backport
git remote -v
git remote -v > remotes
git commit -m "ура победа"
git add remotes
git commit -m "ура победа"
git push
git update-git-for-windows
git push
doskey /history > howto.md
