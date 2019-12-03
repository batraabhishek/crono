# Crono: Smart Notifications
#AndroidDevChallenge
![](https://github.com/batraabhishek/crono/raw/master/cr.jpg)

## Overview
An average user receives 150 notifications in a day. These notifications contain promotions, spam which a user might not even look at. Crono is designed to cut through the clutter and provide a notifications experience that surfaces only useful information in the notification drawer. With Crono, we want to make phone notifications smart. 

Currently, Crono acts as a bridge between android device and pc. Notifications are synced between browser and android device. User can share files and clipboard data etc. Crono has about 15000 active users, growing daily. Crono is available at https://play.google.com/store/apps/details?id=com.getcrono

But that's not all. 


## Notification Classifier

We will build a **TensorFlow Lite** model, by manually training notifications (tens of thousands of notifications). Tensorflow model will be integrated into Crono Android app. 

- The model will identify similar types of notifications and group them under categories.
- This model will work offline, as it will be integrated into android app.


Notification classifier will be a model that will predict the type of notification. Based on the content of notification the model will categorize the notification into the following five categories.
1. **Primary** will contains notifications that are categorised as high priority notifications. These notifications will be displayed in the Notification drawer. 
2. **Messages**: All the notifications that are categorized as conversations by the Tensorflow model will fall under this category. These notifications will leverage Android Notification grouping and will form a single group in the Notification Drawer.
3. **Transactions**: Any notification that contains sensitive financial information like bank statements, credit card transactions will fall under this category.
4. **Promotions**: Notifications that are categorised as spam will come in this category. Crono will auto remove these notifications from the Notification Drawer. User can still access these notifications from Crono app. 
5. **Reminders**: Tensorflow Lite model will also detect time-sensitive + important notifications. Crono will show these notifications under Reminder group. Also, Crono will make sure to remind the user about the notification context at the appropriate time.


![](https://github.com/batraabhishek/crono/raw/master/crono_framed.png)

## Timeline
1. **December-January:** Generate training dataset from notifications.
2. **February:** Training TensorFlow model and integration into Android App
3. **March - April:** App logic + UI + UX work
4. **May:** App launch

## Required Google Services 
1. Firebase
2. TensorFlow Lite
3. Google Cloud Functions


## Cover letter
https://github.com/batraabhishek/crono/blob/master/Android%20Dev%20Challenge%20-%20Cover%20Letter.pdf
