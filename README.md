# Android Lab Activities

**Student ID:** 22100331

## Project Structure

- **MainActivity** - Hands-on 1: Hello Campus
- **CounterActivity** - Hands-on 2: The Interrupted Counter

## Part 1: Hello Campus

Displays "Department of Computer Science" in a TextView. Clicking "Show Chairwoman" updates the text to "Dr. Sarah Johnson". The Action Bar shows ID: 22100331.

## Part 2: The Interrupted Counter

A counter that increments on button press and survives screen rotation using onSaveInstanceState and onRestoreInstanceState.

### The Sabotage Bug: NullPointerException Explained

The sabotage code was:
TextView counterDisplay = null;
counterDisplay.setText("0");

Why it crashed: counterDisplay is explicitly set to null. When setText("0") is called, the JVM throws a NullPointerException because there is no object to call the method on.

The Fix: Use findViewById(R.id.tvCounter) to get a real reference to the TextView before calling any methods on it.

### State Preservation on Rotation

Android destroys and recreates the Activity on screen rotation. We fix counter reset using onSaveInstanceState to save the counter value and onRestoreInstanceState to restore it after recreation.

## How to Run

1. Open in Android Studio
2. Wait for Gradle sync
3. Run on emulator API 24+
4. Test rotation on Counter screen with Ctrl+Left or Ctrl+Right
