# FlowPDF Legacy 📄🌊

FlowPDF Legacy is a React Native and Expo-based app for browsing, organizing, and viewing PDF files stored on your device. It focuses on Android file-system access, local folder scanning, and a fast, lightweight PDF viewing experience without requiring cloud storage.

This project is built for local-first document access and is optimized for mobile workflows where you need quick access to PDFs from folders on-device.

## ✨ Features

- Local PDF discovery from user-selected folders
- Android Storage Access Framework integration for folder browsing
- Fast PDF rendering using `react-native-pdf-jsi`
- Smooth mobile UI with Expo Router and React Native
- Persistent folder preferences via Zustand + Async Storage
- Large file list support using `@shopify/flash-list`
- Cross-platform mobile development with Expo

## 🛠️ Tech Stack

- Framework: [React Native](https://reactnative.dev/) + [Expo](https://expo.dev/)
- Routing: [Expo Router](https://docs.expo.dev/router/introduction/)
- PDF Rendering: [`react-native-pdf-jsi`](https://github.com/react-native-pdf-jsi/react-native-pdf-jsi)
- State Management: [Zustand](https://github.com/pmndrs/zustand)
- Storage: `@react-native-async-storage/async-storage`, `expo-file-system`
- UI & Icons: `@expo/vector-icons`, `@react-native-vector-icons/material-design-icons`
- List Rendering: `@shopify/flash-list`

## 🚀 Getting Started

### Prerequisites

Before running the app, make sure you have:

- [Node.js](https://nodejs.org/) installed
- [Expo CLI](https://docs.expo.dev/get-started/installation/) available via `npx expo`
- Android Studio and Android SDK for Android development, or Xcode for iOS development
- A physical device or emulator for running the app

This project uses native dependencies for PDF rendering and file access, so a native build is typically required.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/tej-sh/FlowPDF-Legacy.git
   cd FlowPDF-Legacy
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the app:

   ```bash
   npx expo start
   ```

### Running on Android

```bash
npx expo run:android
```

### Running on iOS

```bash
npx expo run:ios
```

## 📂 Project Structure

```text
.
├── app/                  # Expo Router screens and navigation
├── assets/              # Static assets, fonts, and images
├── components/          # Reusable UI and feature components
│   ├── Folders/         # Folder selection and file-system UI
│   └── Pdf/            # PDF viewer and related UI
├── store/               # Zustand state stores
├── .gitignore
├── app.json             # Expo app configuration
├── eas.json             # EAS build configuration
├── eslint.config.js    # ESLint configuration
├── LICENSE              # MIT license
├── package.json         # Project dependencies and scripts
├── README.md            # Project documentation
├── tsconfig.json        # TypeScript configuration
└── ...
```

## 🔐 Notes

- Folder access is designed around local file browsing and Android document access flows.
- On Android, you may need to grant the app permissions and choose a root folder before PDFs are discovered.
- Because this app relies on native modules, the recommended workflow is to run it through a device/emulator build rather than a simple browser preview.

## 🤝 Contributing

Contributions, bug reports, and feature suggestions are welcome.

- Open an issue: https://github.com/tej-sh/FlowPDF-Legacy/issues
- Submit a pull request with a clear description of the change

## 📝 License

This project is licensed under the [MIT License](LICENSE).
