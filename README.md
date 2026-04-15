#  Weather App (C Language)

##  Overview

This is a simple Weather Application built in **C language** that fetches real-time weather data using an API and displays it in a user-friendly format.
The project demonstrates API handling, JSON parsing, and basic GUI integration in C.

---

##  Features

*  Get weather data by city name
*  Displays temperature
*  Shows humidity
*  Parses JSON data using cJSON library
*  Cross-platform animated GUI (SDL2)



##  Technologies Used

* C Programming Language
* cJSON Library
* Weather API
* SDL2 + SDL2_ttf (for GUI)

---

##  How It Works

1. User enters a city name
2. Program sends an API request using `curl`
3. Weather data is received in JSON format
4. Data is parsed using **cJSON**
5. Output is displayed on screen (GUI/Text)

---

##  Project Structure

```
WeatherApp/
│── weather.c          # Console app (API call + parsing)
│── gui_weather.c      # Cross-platform SDL2 GUI
│── cJSON.c / cJSON.h  # JSON parsing library
│── weather.json       # API response file
│── weather.exe        # Executable (optional)
```

---

##  How to Run

1. Install dependencies:

Linux (Debian/Ubuntu):

```
sudo apt update
sudo apt install -y build-essential curl libsdl2-dev libsdl2-ttf-dev fonts-dejavu-core
```

Windows (MSYS2 MinGW64):

```
pacman -Syu
pacman -S --needed mingw-w64-x86_64-gcc mingw-w64-x86_64-SDL2 mingw-w64-x86_64-SDL2_ttf curl
```

2. Compile the console app:

```
gcc weather.c cJSON.c -o weather_console
```

3. Compile the GUI app:

Linux:

```
gcc gui_weather.c cJSON.c -o weather_gui $(sdl2-config --cflags --libs) -lSDL2_ttf -lm
```

Windows (MSYS2 MinGW64 shell):

```
gcc gui_weather.c cJSON.c -o weather_gui.exe -IC:/msys64/mingw64/include/SDL2 -LC:/msys64/mingw64/lib -lmingw32 -lSDL2main -lSDL2 -lSDL2_ttf -lm
```

4. Run:

```
./weather_gui
```

5. Enter city name and press Enter or click **Fetch**

---

##  Note:-

* Make sure `curl` is installed on your system
* Replace API key with your own (if required)

---

##  Output

Displays:

* Temperature 
* Humidity 
* Weather condition 

---

##  Learning Outcomes

* API integration in C
* JSON parsing using cJSON
* Basic GUI programming
* Working with system commands

---

##  Author

**Manek Yadav**

---

##  Future Improvements

* Add weekly forecast cards
* Auto-detect location
* Add hourly timeline animation

