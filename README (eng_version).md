# QML-SpotifyAnalogue
SpotifyAnalogue app allows one to:
* Listen to tracks and switch between them
* Add songs via search function
* Remove tracks from a playlist
* See the song title, author and picture

All windows slide out smoothly, the scrolling function works

## Tech performance
1) The user enters the name of the song he wants to listen to
2) The program sends a GET request to the Jamendo API and receives a JSON file
3) After parsing the JSON file, we get an array of songs, display them as a QListView
4) The user selects a song and it is added to the playlist

Model-View concept is used

## Demonstration of the application
Listening and switching between tracks

![change](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/b6bd5b48-6964-4f5a-a6fd-8adfffb3a6ac)

Playlist with scrolling function

![playlist](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/28a1142a-ad54-4363-a444-32568d095951)

Adding new tracks

![find](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/41695fff-a2d5-4601-a010-36e1745858f8)


## How to install my app
1) Make sure you have Qt Creator and Git CMD installed
2) Create a "git" folder on your Dekstop

![image](https://github.com/KozlovVP/Qt-EmployeeMonitoring/assets/114473389/45e6e0d7-e09b-4fd8-9c74-55246530dcb9)

3) Open Git CMD and type "git clone https://github.com/KozlovVP/QML-SpotifyAnalogue"

![image](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/8b8be92c-5520-4c5d-b48d-0103a2cae538)

4) Copy PATH to the "git" folder on your Dekstop and type "cd \<PATH\>"

![image](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/c396cf61-4554-460c-93c0-344b10681a81)

5) Type "git clone https://github.com/KozlovVP/QML-SpotifyAnalogue" one more time

![image](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/ed70ef1f-4ffa-4372-85c6-62d7faef2258)

6) Congrats! Now you have all src files in your "git" folder

7) Open Qt Creator and go to "Open project"->C:\Users\\..\Desktop\git\QML-SpotifyAnalogue\MusicPlayer\CMakeLists.txt
You will see the src files

![image](https://github.com/KozlovVP/QML-SpotifyAnalogue/assets/114473389/a39b6521-b89f-4d81-ad6c-6cca81de2536)

Thanks for installation!
