# Number System Converter  
A cross-platform mobile application for converting numbers between Binary, Octal, Decimal, and Hexadecimal.  

---

## Table of Contents
1. Introduction  
2. Features  
3. System Requirements  
4. Project Structure  
5. How It Works  
6. Installation and Setup  
7. Usage  
8. Test Cases  
9. Error Handling  
10. Deployment    
11. Conclusion  

---

## Introduction
This project automates number system conversions between Binary, Octal, Decimal, and Hexadecimal.  
It was developed using React Native, ensuring compatibility with both Android and iOS.  

The app takes an input number, the base system of that number, and outputs the equivalent value in all supported number systems.  

---

## Features
- Convert numbers between Binary, Octal, Decimal, and Hexadecimal.  
- Interactive and user-friendly interface.  
- Error handling for invalid inputs.  
- Works on Android and iOS with one codebase.  
- Open-source and easy to extend.  

---

## System Requirements
**Software:**  
- Node.js (LTS)  
- React Native CLI or Expo  
- Android Studio (for Android build)  
- Xcode (for iOS build, on Mac)  
- GitHub (for collaboration and version control)  

**Hardware:**  
- Smartphone (Android 8.0+ / iOS 13+) or Emulator  
- Minimum 4GB RAM  
- Internet connection  

---

## Project Structure
```
NumberSystemConverter/
│── App.js                 # Main application file
│── package.json           # Dependencies and scripts
│── /components            # Reusable components
│     └── Converter.js
│── /screens               # App screens
│     └── HomeScreen.js
│── /assets                # Images/icons
```

---

## How It Works
1. User enters a number in the input field.  
2. User selects the base system (Binary, Octal, Decimal, Hexadecimal).  
3. The app validates the input based on the selected base.  
4. The app converts the input to Decimal (intermediate format).  
5. From Decimal, the app generates equivalent values in all other systems.  
6. Results are displayed in a clean format.  

**Flowchart:**  

```
   ┌─────────────┐
   │   Start     │
   └─────┬───────┘
         │
  Enter number + base
         │
 Validate input
         │
   Convert → Decimal
         │
 Convert Decimal → Other systems
         │
 Display all results
         │
   ┌─────▼──────┐
   │    End     │
   └────────────┘
```

---

## Installation and Setup

### 1. Clone Repository
```bash
git clone https://github.com/your-username/number-system-converter.git
cd number-system-converter
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Run on Android
```bash
npx react-native run-android
```

### 4. Run on iOS (Mac required)
```bash
npx react-native run-ios
```

---

## Usage
1. Enter a number in the input box.  
2. Select the base system (Binary, Octal, Decimal, Hexadecimal).  
3. Press Convert.  
4. View the results in all number systems.  

---

## Test Cases

| Input Number | Base Selected | Decimal | Binary  | Octal | Hexadecimal |
|--------------|--------------|---------|---------|-------|-------------|
| `1010`       | Binary       | 10      | 1010    | 12    | A           |
| `25`         | Decimal      | 25      | 11001   | 31    | 19          |
| `77`         | Octal        | 63      | 111111  | 77    | 3F          |
| `1A`         | Hexadecimal  | 26      | 11010   | 32    | 1A          |

---


## Error Handling
- If the user enters an invalid number (for example, `2` in Binary), the app displays:  
  ```
  Invalid input for Binary system.
  ```

---

## Deployment
**Android:**  
```bash
npx react-native run-android
```
Generate APK or AAB for production:  
```bash
cd android
./gradlew assembleRelease
```

**iOS (Mac only):**  
```bash
npx react-native run-ios
```
Build via Xcode for IPA file.  

**Collaboration:**  
- Project hosted on GitHub.  
- Lecturer added as collaborator.  

---


---

## Conclusion
The Number System Converter app demonstrates how React Native can be used to build a cross-platform mobile application with practical use in computer science and digital systems. It successfully automates number system conversions between Binary, Octal, Decimal, and Hexadecimal, while maintaining a simple and intuitive interface.  

---
