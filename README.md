# Crono: Smart Notifications
#AndroidDevChallenge
![](https://github.com/batraabhishek/crono/raw/master/cr.jpg)

## Overview
An average user receives 150 notifications in a day. These notifications contain promotions, spam which a user might not even look at. Crono is designed to cut through the clutter and provide a notifications experience that surfaces only useful information in the notification drawer. With Crono, we want to make phone notifications smart. 

## Notification Classifier

We will build a **TensorFlow Lite** model, by manually training notifications (tens of thousands of notifications). Tensorflow model will be integrated into Crono Android app. 

- The model will identify similar types of notifications and group them under categories.
- This model will work offline, as it will be integrated into android app.


Notification classifier will be a model that will predict the type of notification. Based on the content of notification the model will categorize the notification into the following four categories.
1. Primary
2. Messages
3. Transactions
4. Promotions

![](https://github.com/batraabhishek/crono/raw/master/crono_framed.png)

## Timeline
1. **December-January:** Generate training dataset from notifications.
2. **February:** Training TensorFlow model and integration into Android App
3. **March - April:** App logic + UI + UX work
4. **May:** App launch

## Cover letter
https://github.com/batraabhishek/crono/blob/master/Android%20Dev%20Challenge%20-%20Cover%20Letter.pdf
