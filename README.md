### Ход выполнения Рабочей тетради №1

##### 1) Создание локального git-репозитория

```shell
cd frontend-backend-project
git init
```

##### 2) Создание папок и файлов

```shell
mkdir Folder1 Folder2 Folder3
echo "Initial file in Folder1" > Folder1/file.txt
echo "Initial file in Folder2" > Folder2/file.txt
echo "Initial file in Folder3" > Folder3/file.txt
```

##### 3) Создание веток и добавление файлов

```shell
git checkout -b Branch1
echo "New file in Folder1 for Branch1" > Folder1/new_file.txt
git add .
git commit -m "Добавлен новый файл в Folder1 из Branch1"

git checkout -b Branch2
echo "New file in Folder2 for Branch2" > Folder2/new_file.txt
git add .
git commit -m "Добавлен новый файл в Folder2 из Branch2"
```

##### 4) Создание и переход в `main`

```shell
git checkout -b main
```

##### 5) Объединить изменения из `Branch1` и `Branch2` в `main`

```shell
git merge Branch1 -m "Merged Branch1 into main"
git merge Branch2 -m "Merged Branch2 into main"
```

##### 6) Внесение изменений в Folder3

```shell
echo "Updated file in Folder3" > Folder3/updated_file.txt
git add .
git commit -m "Updated Folder3"
```

##### 7) Создание удаленного репозитория на GitHub

```shell
git remote add origin https://github.com/oreg0na/frontend-and-backend-first-basic-task
git branch -M main
git push -u origin main
```

##### 8) Создание приложения ReactJS

```shell
npx create-react-app test-app
cd test-app
npm run start
```

##### 9) Изменение логотипа в файле `src/App.js`

##### 10) Commit update in React App

```shell
git add .
git commit -m "Updated ReactJS"
git push origin main
```
