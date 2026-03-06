# Інструкція для швидкого розгортання та базових налаштувань бекенду для фінального проєкту

## 1.
для розгортання проєкту потрібно створити `github` репозиторій з додаванням `.gitignore` оптимізований під `Node.js`.

## 2.
репозиторій клонувати до себе на комп'ютер.

## 3.
в терміналі виконати команди для швидкого розгортання базової структури проєкту, а також інсталяції `node_modules`

## 4.
для розгортання базових модулів, що потрібні для створення сервера `express` в терміналі потрібно виконати команду(за необхідності перелік пакетів можна змінити або доповнити):
```bash
npm init -y && npm i express mongoose cors dotenv http-errors celebrate bcrypt &&  npm i nodemon -D
``` 

## 5.
для наповнення базової структури потрібно в терміналі викликати команду:
```bash
mkdir src && cd src && mkdir controllers db middleware models routes services utils validations && touch controllers/index.js db/connectToMongDB.js middleware/index.js models/index.js routes/index.js services/index.js utils/index.js validations/index.js server.js ../readme.md && cd ..
```