# Gemini API Compose Starter 🌐📱

An advanced Android starter template engineered with **Jetpack Compose** that integrates Google's **Gemini API** for real-time generative conversational experiences. Built following modern Android development practices, it features secure local API key management, reactive UI states, and a clean architecture layout.

---

## 🌟 Key Features

* **Declarative Jetpack Compose UI**: Built entirely with modern Compose layouts, supporting reactive state collection, custom chat bubbles, smooth scrolling, and dynamic input fields.
* **Gemini Generative AI Integration**: Pre-configured client setup connecting directly to Google's generative models (`gemini-pro` / `gemini-1.5-flash`) for streaming text and multi-turn conversations.
* **Secure Key Management (`local.properties`)**: Protects your sensitive credentials by injecting API keys safely at compile-time via `BuildConfig`, preventing accidental leakage into public version control.
* **Reactive Coroutine Architecture**: Leverages Kotlin Coroutines and Flows for non-blocking asynchronous network requests and fluid conversational UI updates.
* **Extensible Boilerplate**: Designed to serve as a solid foundation for building custom AI assistants, study partners, or productivity chatbots.

---

## 🏗️ Project Architecture & Structure

The project follows a clean, feature-based modular structure to keep UI logic decoupled from network operations:

```text
com.example.geminiapicomposestarter/
│
├── data/                  # API clients, network data sources, and DTO models
├── ui/
│   ├── components/        # Reusable UI widgets (chat bubbles, input bars, loaders)
│   ├── screens/           # Main chat screen and navigation destinations
│   └── theme/             # Material 3 color schemes, typography, and shapes
│
├── viewmodel/             # ViewModel managing UI state and generative request flows
└── MainActivity.kt        # Entry point initializing Compose content
