# 💊 Smart Medicine Reminder

An Arduino-based **Smart Medicine Reminder System** designed to remind users to take their medicines at the scheduled time. The system uses a real-time clock, LCD display, buzzer, LEDs, and buttons to provide visual and audio reminders.

## 📌 Project Overview

The **Smart Medicine Reminder** is an embedded-system project developed using an **Arduino Uno**. It displays the current time and medicine reminder information on a 16×2 LCD. When the scheduled medicine time is reached, the system activates a buzzer and LED notification to remind the user.

The system is designed to provide a simple and low-cost solution for improving medication adherence.

## 🎯 Objectives

* Provide timely medicine reminders.
* Display time and reminder information on an LCD.
* Generate an audio alert using a buzzer.
* Provide visual alerts using LEDs.
* Allow the user to interact with the system using buttons.
* Develop a simple and affordable embedded healthcare solution.

## ⚙️ Features

* ⏰ Real-time time tracking
* 💊 Medicine reminder system
* 📺 16×2 LCD display
* 🔊 Buzzer notification
* 🔴 Red LED warning indicator
* 🟢 Green LED status indicator
* 🔘 Button-based user interaction
* 🔋 Arduino-based embedded system
* 🕐 Scheduled medicine alerts

## 🛠️ Hardware Components

| Component           | Purpose                                |
| ------------------- | -------------------------------------- |
| Arduino Uno         | Main microcontroller                   |
| DS3231 / DS1307 RTC | Keeps accurate date and time           |
| 16×2 LCD            | Displays time and medicine information |
| Buzzer              | Provides audible medicine reminder     |
| Red LED             | Indicates medicine alert               |
| Green LED           | Indicates normal/status condition      |
| Push Buttons        | User input and control                 |
| Resistors           | Current limiting/protection            |
| Jumper Wires        | Circuit connections                    |
| Acrylic Sheet       | Physical project structure             |

## 💻 Software & Tools

* Arduino IDE
* Embedded C / Arduino C++
* Arduino Uno
* RTC Library
* LiquidCrystal Library

## 🔌 System Working

The system works according to the following process:

```text
        ┌─────────────────┐
        │   Arduino Uno   │
        └────────┬────────┘
                 │
       ┌─────────┼─────────┐
       │         │         │
       ▼         ▼         ▼
    RTC Module  LCD     Buttons
       │         │         │
       │         │         │
       ▼         ▼         ▼
   Current Time  Display  User Input
                 │
                 ▼
          Medicine Schedule
                 │
                 ▼
          ┌─────────────┐
          │ Reminder    │
          │ Time Reached│
          └──────┬──────┘
                 │
          ┌──────┴──────┐
          ▼             ▼
       Buzzer        Red LED
       Alert         Warning
```

## 🔄 How It Works

1. The Arduino initializes all connected components.
2. The RTC module provides the current time.
3. The current time is displayed on the LCD.
4. The system continuously compares the current time with the programmed medicine time.
5. When the scheduled time is reached:

   * The buzzer starts producing an alert.
   * The red LED starts blinking.
   * The LCD displays the medicine reminder.
6. The user can interact with the system using the buttons.
7. After the reminder is acknowledged, the system returns to its normal monitoring state.

## 🔘 User Interaction

The push buttons are used to control and interact with the reminder system. Depending on the programmed functionality, buttons can be used for:

* Setting reminder time
* Selecting options
* Confirming a reminder
* Navigating between settings

## 📺 LCD Display

The LCD can display information such as:

```text
Time: 08:00 AM
Medicine Time
Take Medicine!
```

During normal operation, it can display the current time and system status.

## 🚨 Medicine Alert

When the medicine schedule matches the current RTC time, the system generates a reminder.

```text
Medicine Time Reached
        ↓
   Buzzer ON
        ↓
   Red LED Blink
        ↓
LCD: Take Medicine!
        ↓
 User Acknowledges
        ↓
    Alert Stops
```

## 🧪 Testing

The system can be tested by setting different medicine reminder times and checking whether:

* The RTC displays the correct time.
* The LCD displays the expected information.
* The buzzer activates at the scheduled time.
* The red LED blinks during the reminder.
* The user buttons respond correctly.
* The reminder stops after user acknowledgement.

## 🔮 Future Improvements

Future versions of the project could include:

* Multiple medicine schedules
* Automatic medicine dispensing
* Mobile application integration
* Bluetooth/Wi-Fi connectivity
* Notification through a smartphone
* Medicine stock monitoring
* Voice reminders
* Cloud-based medication history
* Rechargeable battery support

## 📚 Project Type

**Embedded Systems / IoT / Healthcare Automation**

## 👨‍💻 Author

**Syed Muhammad Khizer Rizvi**

Computer Science Student
Iqra University, North Campus, Karachi

📧 Email: [syedkhizer405@gmail.com](mailto:syedkhizer405@gmail.com)

---

⭐ If you find this project useful, consider giving the repository a star!
