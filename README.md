Practical 6 – Mobile Application Development
Submitted By: Reyan Prajapati
Enrollment Number: 24012011155
Department: Computer Engineering / Information Technology
Course: Mobile Application Development
Aim
To create an Android application with an alarm-setting screen and an animated splash screen, using XML drawable resources and Android animations.
Objectives
1. Create MainActivity according to the provided UI design.
2. Create a SplashActivity with an animated logo.
3. Create a rectangular gradient background for the splash screen using the <gradient> tag inside a <shape> drawable. The practical specifies a radial gradient with x = 0.9, y = 0.9, and radius 1500, starting with pink and ending with blue.
4. Demonstrate Android animation resources and tags:
   - <animation-list> and the oneShot attribute
   - <set> with android:startOffset and android:duration
   - <scale>, <translate>, <rotate>, and <alpha>
Main Features
- Splash screen with gradient background and animated logo.
- Alarm screen with an image, title, alarm-time display, explanatory text, and animated heart icon.
- Create Alarm button that opens a time picker.
- Cancel Alarm button to cancel the scheduled alarm.
- AlarmManager and PendingIntent for scheduling alarms.
- AlarmService with MediaPlayer to play the alarm sound.
- AlarmBroadcastReciver broadcast receiver to start or stop the alarm service.
Project Components
File	Purpose
MainActivity.kt	Displays the alarm UI, opens the time picker, and schedules or cancels alarms.
SplashActivity.kt	Displays the animated splash screen and opens MainActivity after the animation ends.
AlarmService.kt	Plays the alarm sound using MediaPlayer.
AlarmBroadcastReciver.kt	Receives alarm start/stop broadcasts and controls the service.
activity_main.xml	Defines the main alarm screen layout.
activity_splash.xml	Defines the splash screen layout.
activity_alarm_service.xml	Layout resource included in the practical.
rectangle_gradient.xml	Defines the splash screen's pink-to-blue gradient background.
uvpce_animation_list.xml	Defines the frame animation for the splash logo.
alarm_frame_anim.xml	Defines the alarm image frame animation.
heart_pulse.xml	Defines the pulsing heart scale animation.
twinanimation.xml	Defines splash-logo translate, rotate, and scale animations.
AndroidManifest.xml	Declares permissions, activities, service, and broadcast receiver.


Technologies Used
- Kotlin
- Android Studio
- XML layouts and drawable resources
- Android animation framework
- AlarmManager, PendingIntent, BroadcastReceiver, Service, and MediaPlayer
How to Run
1. Open the project in Android Studio.
2. Allow Gradle sync to finish.
3. Confirm that all drawable and animation resources referenced by XML and Kotlin files are present.
4. Run the application on an Android emulator or physical Android device.
5. The splash screen appears first, followed by the alarm screen.
6. Tap Create Alarm to select an alarm time. Tap Cancel Alarm to cancel it.
Notes
- On Android 12 and later, exact-alarm scheduling may require the user to grant special access.
- Ensure an alarm audio file exists at res/raw/alarm for AlarmService.
- The practical document uses the package name com.example.a24012011155_practical_6. Ensure package declarations and manifest entries match the actual project.
- The source names the receiver AlarmBroadcastReciver (spelling as provided in the practical). Keep this class name consistent across Kotlin and AndroidManifest.xml.
Author
Reyan Prajapati
Enrollment Number: 24012011155
