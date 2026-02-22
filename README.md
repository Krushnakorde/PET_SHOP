# 🐾 Pet Shop - Mobile App Challenge

A simple, robust Pet Shop mobile application built with React Native (Expo) and TypeScript. This app allows users to list pets, upload images, and manage a shopping cart with global state.

## 🚀 Features
- **Pet Image Upload:** Support for both Camera and Gallery using `expo-image-picker`.
- **API Integration:**
  - Random pet images fetched from `dog.ceo` API.
  - Form data submitted to `reqres.in` mock API.
- **State Management:** Lightweight and fast global state using `Zustand`.
- **Form Validation:** Strict schema validation with `Zod` and `react-hook-form`.
- **UI/UX:** Clean, card-based listing with real-time cart updates and toast notifications.

## 🛠️ Tech Stack & Libraries
- **Framework:** Expo (React Native)
- **Language:** TypeScript (for type safety and better DX)
- **State:** Zustand
- **Forms:** React Hook Form + @hookform/resolvers/zod
- **Networking:** Axios
- **Feedback:** react-native-toast-message

## 🏗️ Architecture Overview
I followed a **Feature-based/Layered Architecture** to ensure the code is maintainable and scalable:
- `/src/components`: Reusable UI elements (PetCard, CartItem) to keep screens lean.
- `/src/store`: Centralized logic for the shopping cart and pet listing.
- `/src/utils`: Validation schemas separated from UI logic.
- `/src/screens`: High-level views orchestrating data flow.

**Why Zustand?** I chose Zustand over Redux or Context API because it provides a much simpler boilerplate while maintaining high performance for global state like a shopping cart.

## 📥 Setup Instructions
1. Clone the repository:
   ```bash
   git clone <your-repo-link>