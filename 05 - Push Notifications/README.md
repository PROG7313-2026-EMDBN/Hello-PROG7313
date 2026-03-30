# 🚀 PROG7313 Practical Activity: Adding Local and Push Notifications to the Digital Detox App

## 📝 Objective

In this activity, you will extend your Digital Detox app by adding two different types of notifications:

- a local notification that reminds the user to log their detox session  
- a Firebase Cloud Messaging (FCM) push notification that informs users that an app update is pending  

By the end of this activity, you should be able to understand and implement:
- notifications triggered inside the app on the device
- notifications triggered remotely through Firebase

## 🛠️ Your Task

You will need to implement both:

### 🔹 Part A: Local Notification

Add a feature to schedule a reminder:

```
Title: Digital Detox Reminder
Message: Don’t forget to log your detox session today.
```

You can extend it later to remind user in 10 seconds, remind user every evening, or remind user to add details after a focus session  

### 🔹 Part B: Firebase Push Notification

Enable FCM to receive update notifications:

```
Title: Update Pending
Message: A new Digital Detox update is available soon.
```

You can extend it later to announce update announcements; announce feature releases, and broadcast messages to users  

## 📚 Resources to research before you start coding

Research the following concepts:
- Android notification basics
- Notification channels
- Runtime notification permission
- WorkManager
- Firebase Cloud Messaging (FCM)
- FirebaseMessagingService

You should understand:
- what a notification is  
- why Android uses channels
- the difference between local and remote triggers
- how FCM delivers messages

You can also refer to the Sandbox, if needed.