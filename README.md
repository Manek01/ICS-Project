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
*  Simple GUI interface (Windows API)



##  Technologies Used

* C Programming Language
* cJSON Library
* Weather API
* Windows API (for GUI)

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
│── weather.c          # Main logic (API call + parsing)
│── gui_weather.c      # GUI implementation
│── cJSON.c / cJSON.h  # JSON parsing library
│── weather.json       # API response file
│── weather.exe        # Executable (optional)
```

---

##  How to Run

1. Compile the code:

```
gcc weather.c gui_weather.c cJSON.c -o weather.exe
```

2. Run:

```
./weather.exe
```

3. Enter city name when prompted

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

* Add better GUI design
* Auto-detect location
* Add forecast feature
* Cross-platform support

