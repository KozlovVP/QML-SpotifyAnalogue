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

![change](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/b6bd5b48-6964-4f5a-a6fd-8adfffb3a6ac)

Плейлист с функцией скроллинга

![playlist](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/28a1142a-ad54-4363-a444-32568d095951)

Возможность добавлять новые треки

![find](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/41695fff-a2d5-4601-a010-36e1745858f8)


## Как установить мое приложение
1) Удостоверьтесь, что у вас установлены Qt Creator и Git CMD 
2) Создайте папку "Git" на рабочем столе

![image](https://github.com/KozlovVP/Qt-EmployeeMonitoring/assets/114473389/45e6e0d7-e09b-4fd8-9c74-55246530dcb9)

3) Откройте Git CMD и введите "git clone https://github.com/KozlovVP/QML-SpotifyAnalogue"

![image](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/8b8be92c-5520-4c5d-b48d-0103a2cae538)

4) Скопируйте PATH к папке "git", которую вы создали, и введите "cd \<PATH\>"

![image](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/c396cf61-4554-460c-93c0-344b10681a81)

5) Введите "git clone https://github.com/KozlovVP/QML-SpotifyAnalogue" повторно

![image](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/ed70ef1f-4ffa-4372-85c6-62d7faef2258)

6) Теперь все файлы программы находятся в папке "git"

7) Откройте Qt Creator, нажмите на "Open project"->C:\Users\\..\Desktop\git\QML-SpotifyAnalogue\MusicPlayer\CMakeLists.txt
Вы увидите исходные файлы приложения

![image](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/a39b6521-b89f-4d81-ad6c-6cca81de2536)

Спасибо за установку!
