# 🔔 Android Application to Display Notifications

## 📌 Project Title

**Create an Android Application to Display Notifications**

---

## 🎯 Aim

To develop an Android application that demonstrates how to create and display notifications using **Kotlin and Android Studio**.

---

## 🎯 Objective

The main objectives of this experiment are:

* To understand Android Notifications.
* To create a Notification Channel.
* To display a notification when a button is clicked.
* To handle notification permission on Android 13 and above.
* To understand the use of `NotificationCompat`.
* To test notification functionality in an Android application.

---

## 🛠️ Technologies Used

* **Android Studio**
* **Kotlin**
* **XML**
* **Android SDK**
* **NotificationCompat**
* **Notification Channel**

---

## 📖 Concept / Technology

### 🔔 Android Notifications

A notification is a message displayed by Android outside the application's normal user interface. It allows an application to provide information or alerts to the user.

In this application, clicking the **Show Notification** button creates a notification.

### 🔔 Notification Channel

Android 8.0 (API 26) and above requires notifications to be associated with a **Notification Channel**.

The application creates a channel named:

**Demo Notifications**

### 🔐 Notification Permission

Android 13 (API 33) and above requires the application to request the:

`POST_NOTIFICATIONS`

permission at runtime.

The application checks the Android version and requests permission when required.

---

## 💡 Scenario

This application demonstrates a simple student notification system.

When the user opens the application, the screen displays the student's name and USN. When the user clicks **Show Notification**, the application generates a notification.

### Student Details

* **Name:** SWARUPA S
* **USN:** 25MCAR0137

---

## 📱 Application Features

* Simple and user-friendly interface.
* Displays student name and USN.
* Button to generate a notification.
* Creates a notification channel.
* Supports Android notification permissions.
* Displays notification in the device notification panel.
* Notification can be dismissed automatically after it is tapped.

---

## 📂 Project Folder Structure

```text
NotificationDemo/
│
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           │   └── com/
│           │       └── example/
│           │           └── notificationdemo/
│           │               └── MainActivity.kt
│           │
│           ├── res/
│           │   ├── layout/
│           │   │   └── activity_main.xml
│           │   │
│           │   ├── drawable/
│           │   │
│           │   ├── mipmap/
│           │   │
│           │   └── values/
│           │
│           └── AndroidManifest.xml
│
├── screenshots/
│   ├── testcase1.png
│   ├── testcase2.png
│   └── testcase3.png
│
└── README.md
```

---

## 📄 Important Files

### 1. `MainActivity.kt`

This file contains the main application logic.

It:

* Creates the notification channel.
* Handles the **Show Notification** button.
* Requests notification permission on Android 13+.
* Creates and displays the notification.

### 2. `activity_main.xml`

This file defines the application's user interface.

It contains:

* Application title.
* Student name.
* USN.
* **Show Notification** button.

### 3. `AndroidManifest.xml`

The manifest declares the notification permission:

```xml
<uses-permission android:name="android.permission.POST_NOTIFICATIONS" />
```

---

## ▶️ How to Run the Application

1. Open **Android Studio**.
2. Open the `NotificationDemo` project.
3. Wait for Gradle synchronization to finish.
4. Connect an Android device or start an emulator.
5. Click **Run ▶**.
6. The application will open.
7. Verify the displayed name and USN.
8. Click **Show Notification**.
9. If Android asks for notification permission, select **Allow**.
10. Open the notification panel and verify the notification.

---

# 🧪 Test Cases

## Test Case 1 – Launch Application

| Field           | Details                                                                     |
| --------------- | --------------------------------------------------------------------------- |
| Test Case ID    | TC01                                                                        |
| Test            | Launch the application                                                      |
| Input           | Open the application                                                        |
| Expected Result | Application opens successfully and displays the title, name, USN and button |
| Status          | Pass                                                                        |

**Screenshot:**

```text
screenshots/testcase1.png
```

---

## Test Case 2 – Display Notification

| Field           | Details                                                                        |
| --------------- | ------------------------------------------------------------------------------ |
| Test Case ID    | TC02                                                                           |
| Test            | Click Show Notification                                                        |
| Input           | Tap the Show Notification button                                               |
| Expected Result | Notification permission is requested if required and notification is displayed |
| Status          | Pass                                                                           |

The notification should display:

**Title:** Notification Demo

**Message:** Hello SWARUPA! Your notification is working.

**Screenshot:**

```text
screenshots/testcase2.png
```

---

## Test Case 3 – Verify Notification

| Field           | Details                               |
| --------------- | ------------------------------------- |
| Test Case ID    | TC03                                  |
| Test            | Check notification panel              |
| Input           | Open the device notification panel    |
| Expected Result | The generated notification is visible |
| Status          | Pass                                  |

**Screenshot:**

```text
screenshots/testcase3.png
```

---

# 📸 Output

The application displays the following interface:

```text
--------------------------------
       Notification Demo

       Name:Devraath Joshi
      **USN:** 25MCAR0091

       [ Show Notification ]
--------------------------------




https://github.com/user-attachments/assets/7978bb78-d888-485d-8095-795a2f59530f



```

After clicking the button, a notification is displayed in the Android notification panel.

---

# 🎓 Learning Outcomes

After completing this experiment, the following concepts were understood:

* Creating notifications in Android.
* Creating and managing Notification Channels.
* Using `NotificationCompat.Builder`.
* Handling notification permissions.
* Using Android's `NotificationManager`.
* Understanding Android 13+ notification permission requirements.
* Testing notifications on an Android device/emulator.

---

# ⚙️ Requirements

### Software Requirements

* Android Studio
* Android SDK
* Kotlin
* Gradle

### Hardware Requirements

* Computer/Laptop
* Android Emulator or Android smartphone

---

# ✅ Conclusion

The Android Notification application was successfully developed using **Kotlin and Android Studio**. The application demonstrates how to create a notification channel, request notification permission, and display a notification when the user clicks a button.

This experiment provides a basic understanding of how notifications are implemented and tested in Android applications.

---

## 👩‍🎓 Student Details

**Name:** Devraath Joshi
**USN:** 25MCAR0091
**Experiment:** Create an Android Application to Display Notifications

---

## 📚 References

* Android Studio Documentation
* Android Developer Documentation
* Kotlin Documentation
