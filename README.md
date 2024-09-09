Overview

This SwiftUI application displays a random positive message along with a corresponding image. Users can toggle sound on or off and trigger the display of a new message and image by pressing a button. The app also supports playing sound effects associated with the displayed message.

Features

Randomized Messages:
Displays one of several predefined positive messages.
Image Display:
Shows a random image corresponding to the message.
Sound Effects:
Plays a sound effect when a new message is displayed if the sound is enabled.
Sound Toggle:
Allows the user to turn sound on or off.
Code Summary

State Variables

messageString: Stores the current message to be displayed.

imageName: Stores the name of the image to be displayed.

imageNumber: Keeps track of the current image index.

messageNumber: Tracks the index of the current message.

lastMessageNumber: Tracks the last displayed message index to avoid repetition.

lastImageNumber: Tracks the last displayed image index to avoid repetition.

lastSoundNumber: Tracks the last played sound index to avoid repetition.

audioPlayer: Manages audio playback.

soundIsOn: Boolean to toggle sound effects on or off.

UI Components
Message Display:

A Text view to display the current message, styled with a large font and red color.
The text animates when updated to make it more engaging.

Image Display:
An Image view to show the image corresponding to the current message.
The image is styled with rounded corners and a shadow for visual appeal.

Sound Toggle:
A Toggle switch allows the user to enable or disable sound effects.
The Toggle state affects whether sound effects play when a new message is shown.

Action Button:
A Button that triggers the display of a new random message, updates the displayed image, and plays a corresponding sound effect (if sound is enabled).

Functions

nonRepeatingRandom(lastNumber:upperBound:):

Generates a random number between 0 and upperBound, ensuring it is not the same as lastNumber.

playSound(soundName:):
Plays a sound effect using AVAudioPlayer. Retrieves the sound file from the app bundle and handles playback.


How to Use

Run the App:
Launch the app on a simulator or physical device.
Toggle Sound:
Use the Toggle switch to enable or disable sound effects.
Show Message:
Press the "Show Message" button to display a new random message and image, and play a sound effect if sound is enabled.
Future Enhancements

Additional Messages and Images:
Add more messages and images to diversify the content.
Custom Sound Effects:
Expand the sound library with custom sound effects for different messages or user interactions.
Enhanced User Interface:
Improve UI elements with additional styling and animations for a more polished look.
Accessibility Features:
Implement accessibility features to support users with different needs.
Settings and Preferences:
Add settings to allow users to customize their experience, such as choosing specific message categories or sound themes.
Setup and Running the App


Requirements:
Xcode with SwiftUI support.
iOS 17 or later for compatibility with SwiftUI features.
Running the App:
Open the project in Xcode.
Build and run the app on a simulator or a physical device.
