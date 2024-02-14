eng_version of REAMDE.md is located above

# QML-SpotifyAnalogue
Приложение SpotifyAnalogue позволяет:
* Возможность прослушивать треки, переключаться между ними
* Добавлять песни через функцию поиска
* Удалять треки из плейлиста
* Видеть название песни, автора и картинку

Все окна выдвигаются плавно, работает функция скроллинга

## Техническое исполнение
1) Пользователь вводит название песни, которую хочет прослушать
2) Программа отправляет GET запрос на Jamendo API и получает JSON файл
3) Поссле парсинга JSON-файла получим массив песен, показываем их в виде QListView
4) Пользователь выбирает песню и она добавляется в плейлист

Используется концепция Model-View 

## Демонстрация работы приложения
Возможность прослушивать и переключать треки
![change](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/a2fda8f7-55df-467f-b313-5b03405d6096)

