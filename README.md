# 🌦️ Weather Forecaster App

Welcome to the **Weather Forecaster App**! This is a simple Python-based command-line application that fetches and displays the weather report for any city using the **wttr.in** service. 🌍

---

## 🎯 Features
- **Interactive User Input**:
  - Simply enter the city name to get an instant weather report.
- **Instant Weather Report**:
  - Displays weather data fetched live from **wttr.in**.
- **Easy to Use**:
  - Minimal setup and intuitive functionality.

---

## 🛠️ Technologies Used
- **Python**: Core programming language.
- **Requests Library**: For making HTTP requests to fetch live weather data.

---

## 🚀 How to Run the Project
1. Clone this repository:  
   ```bash
   git clone https://github.com/your-username/weather-forecaster.git

Here's the complete, ready-to-copy README.md file for your Weather Forecaster App project:

markdown
Copy code
# 🌦️ Weather Forecaster App

Welcome to the **Weather Forecaster App**! This is a simple Python-based command-line application that fetches and displays the weather report for any city using the **wttr.in** service. 🌍

---

## 🎯 Features
- **Interactive User Input**:
  - Simply enter the city name to get an instant weather report.
- **Instant Weather Report**:
  - Displays weather data fetched live from **wttr.in**.
- **Easy to Use**:
  - Minimal setup and intuitive functionality.

---

## 🛠️ Technologies Used
- **Python**: Core programming language.
- **Requests Library**: For making HTTP requests to fetch live weather data.

---

## 🚀 How to Run the Project
1. Clone this repository:  
   ```bash
   git clone https://github.com/your-username/weather-forecaster.git
Install the required library:
bash
Copy code
pip install requests
Run the script:
bash
Copy code
python weather_forecaster.py
Enter the name of a city when prompted, and view the weather report in the console! ✅
📂 Repository Structure
weather_forecaster.py: The main script to fetch and display the weather report.
README.md: Documentation and project overview.
🌟 Example Usage
python
Copy code
import requests
 
print("\t\tWelcome to the Weather Forecaster!\n\n")
print("Just Enter the City you want the weather report for and click on the button! It's that simple!\n\n")
 
city_name = input("Enter the name of the City : ")
print("\n\n")
 
# Function to Generate Report
def Gen_report(C):
    url = 'https://wttr.in/{}'.format(C)
    try:
        data = requests.get(url)
        T = data.text
    except:
        T = "Error Occurred"
    print(T)
     
Gen_report(city_name)
🌟 Example Output
plaintext
Copy code
        Welcome to the Weather Forecaster!

Just Enter the City you want the weather report for and click on the button! It's that simple!


Enter the name of the City : New Delhi



Weather in New Delhi:
    Weather: Clear
    Temperature: 25°C
    Wind: 5 km/h from the NW
    ...

🤔 Notes
Ensure you have an active internet connection to fetch live weather data.
Feel free to fork this project, suggest improvements, or contribute! 🌈
This project uses wttr.in, which provides detailed weather information in a simple and readable format.
