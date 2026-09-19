# Practical-4

**Aim:** Develop an Android Alarm application using a `Service` and `BroadcastReceiver`.

## Project Overview

This application demonstrates how an alarm can be scheduled in Android using `AlarmManager`, while background operations are handled with a `BroadcastReceiver` and a `Service`.

### Main Components

- **MainActivity:** Provides the main screen where the user can select an alarm time using a `TimePickerDialog`. It calculates the required time and schedules the alarm.
- **AlarmManager:** Schedules the alarm to trigger at the selected time, even when the application is not currently running.
- **AlarmBroadcastReceiver:** Receives the broadcast when the scheduled alarm time is reached and starts the `AlarmService`.
- **AlarmService:** Controls the alarm ringtone using `MediaPlayer` and continues playing the sound until the alarm is cancelled.
- **Material Design UI:** Uses components such as `MaterialCardView`, `MaterialButton`, and `TextClock` to create a simple and responsive interface.

## Key Features

- Display current date and time.
- Select an alarm time using a time picker.
- Schedule an alarm using `AlarmManager`.
- Receive the alarm event using `BroadcastReceiver`.
- Play an alarm sound using a background `Service`.
- Cancel the scheduled alarm.
- Modern Material Design interface.

## Screenshots

<table>
<tr>
<td align="center">
<img src="./screenshots/ss1.png" width="250" alt="Main Alarm Screen">
<br><br>
<b>1. Main Alarm Screen</b>
</td>

<td align="center">
<img src="./screenshots/ss2.png" width="250" alt="Time Picker">
<br><br>
<b>2. Time Picker</b>
</td>

<td align="center">
<img src="./screenshots/ss3.png" width="250" alt="Alarm Created">
<br><br>
<b>3. Alarm Created</b>
</td>
</tr>
</table>

## Application Working

1. The application displays the current date and time on the main screen.
2. The user presses the **Create Alarm** button.
3. A **Time Picker** appears on the screen.
4. The user selects the required alarm time.
5. The selected time is scheduled using **AlarmManager**.
6. When the scheduled time is reached, **AlarmBroadcastReceiver** receives the alarm event.
7. The receiver starts the **AlarmService**.
8. The `AlarmService` plays the alarm ringtone using `MediaPlayer`.
9. The user can cancel the scheduled alarm using the **Cancel Alarm** button.

## Technologies Used

- Kotlin
- Android Studio
- Android SDK
- AlarmManager
- BroadcastReceiver
- Service
- MediaPlayer
- TimePickerDialog
- Material Design Components

---

# Student Details

**Enrollment No:** 24012011134

**Practical:** 04

**Subject:** Mobile Application Development (MAD)

---

## Project Structure

```text
Practical-4/
│
├── app/
│
├── screenshots/
│   ├── ss1.png
│   ├── ss2.png
│   └── ss3.png
│
├── README.md
│
└── ...
