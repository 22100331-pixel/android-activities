## Summary

This PR implements the two Android lab activities:

### Part 1: Hello Campus (MainActivity)
- Displays "Department of Computer Science" in a TextView
- Button click reveals chairwoman name "Dr. Sarah Johnson"
- Action Bar title set to `ID: 22100331`
- Second button navigates to CounterActivity

### Part 2: The Interrupted Counter (CounterActivity)
- Counter increments on button press
- Survives screen rotation using `onSaveInstanceState` / `onRestoreInstanceState`
- Includes commented sabotage code with NullPointerException explanation

### Files Added
- `app/src/main/java/com/example/androidlab/MainActivity.java`
- `app/src/main/java/com/example/androidlab/CounterActivity.java`
- `app/src/main/res/layout/activity_main.xml`
- `app/src/main/res/layout/activity_counter.xml`
- `app/src/main/AndroidManifest.xml`
- `app/src/main/res/values/strings.xml`
- `app/src/main/res/values/colors.xml`
- `app/src/main/res/values/themes.xml`
- `app/build.gradle`
- `build.gradle`
- `settings.gradle`
- `gradle.properties`
- `README.md`