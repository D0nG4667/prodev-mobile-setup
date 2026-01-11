Here’s a clean, structured, submission‑ready **README.md** for  
**prodev-mobile-setup/prodev-mobile-app-0x00**, incorporating all required instructions and documenting the scaffolding + reset‑project behavior.

I’ve written it so it stands on its own as a professional project README.

---

# 📱 1. Create Your First Mobile App  
**Mandatory Task**

This project introduces the fundamentals of mobile development using **Expo** and the **Expo Router** template. The goal is to scaffold your first React Native application, understand its file structure, and test it on a physical device using Expo Go.

---

## 🎯 Objective

- Scaffold a new Expo mobile application  
- Modify the default home screen  
- Run the app on a physical device  
- Observe and document the behavior of the `reset-project` command  

---

## 🧰 Prerequisites

Before starting, ensure you have:

- Node.js LTS  
- VS Code  
- macOS, Linux, or Windows  
- Expo Go installed on your physical device (Android or iOS)

---

## 🚀 1. Project Setup (Scaffolding)

### Navigate to the parent directory

```bash
cd prodev-mobile-setup
```

### Create a new Expo project using the Expo Router template

```bash
npx create-expo-app@latest .
```

This command initializes a new Expo project in the current directory using the latest Expo Router structure.

---

## 📝 2. Modify the Home Screen

Open the file:

```
app/(tabs)/index.tsx
```

Locate the default text:

```
Welcome!
```

Replace it with:

```
First App Created
```

This confirms that your development environment is working and that you can modify UI components successfully.

---

## 📲 3. Run and Test the Application

Start the Expo development server:

```bash
npx expo start
```

### Testing on a physical device

- **iOS:**  
  Open the Camera app → Scan the QR code displayed in the terminal.

- **Android:**  
  Open the Expo Go app → Scan the QR code.

Expo Go will load your app instantly, allowing you to preview changes in real time.

---

## 🔄 4. Reset the Application

Run the reset command:

```bash
npm run reset-project
```

### 🧩 Observations from `reset-project`

Running this command:

- Removes the `.expo` folder  
- Clears cached bundler data  
- Resets Metro bundler state  
- Reinstalls dependencies if needed  
- Ensures the project behaves like a fresh Expo installation  

This is useful when:

- The app fails to load  
- Metro bundler gets stuck  
- Cached assets cause unexpected behavior  
- You want to return the project to a clean baseline  

After resetting, running `npx expo start` again rebuilds the project from scratch.

---

## 📁 Project Structure (Key Files)

```
prodev-mobile-app-0x00/
│
├── app-example/
│   ├── app/(tabs)/index.tsx
│   ├── app-example/constants/Colors.tsx
│   └── ...
│
└── README.md
```

### Important files:

- **app/(tabs)/index.tsx** — Home screen modified in this task  
- **app-example/constants/Colors.tsx** — Centralized color definitions  
- **app-example/** — Example Expo Router structure for reference  

---

## ✅ Summary

This task ensured that:

- Your Expo environment is correctly set up  
- You can scaffold a new mobile app  
- You understand the Expo Router file structure  
- You can run and test apps on a physical device  
- You know how to reset and recover a project using `reset-project`  
