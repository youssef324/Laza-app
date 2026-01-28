# Laza - E-Commerce Flutter Application

Laza is a modern, fully-functional e-commerce mobile application built with Flutter and Firebase. It features a sleek design with support for both Light and Dark modes, a real-time cloud-synced database, and a comprehensive user flow from discovery to checkout.

## 🚀 Features

### 🔐 Authentication
*   **Sign Up**: Create an account with username, email, and password.
*   **Login**: Secure email and password authentication.
*   **Password Recovery**: Integrated Firebase password reset flow.
*   **Logout**: Securely clear user session.

### 🛍️ Shopping Experience
*   **Product Catalog**: Browse latest arrivals with real-time data.
*   **Product Details**: View high-quality images, dynamic descriptions, and select sizes (S, M, L, XL, 2XL).
*   **Dynamic Search**: Search for products by title or description.
*   **Wishlist**: Add/remove products from your personal wishlist, synced across devices.
*   **Shopping Bag (Cart)**: Manage items in your cart with real-time quantity adjustments and automated price calculations.

### 💳 Checkout & Payments
*   **Shipping Management**: Collect shipping details via a dedicated Address Page.
*   **Order Confirmation**: Preview purchased items and total costs on a detailed confirmation screen.
*   **Wallet**: Track your account balance and view recent financial activity.

### 💬 Social Proof
*   **Product Reviews**: View real reviews from other users.
*   **Add Review**: Submit your own feedback with a name, comment, and star rating.

### 🌓 Personalization
*   **Dark Mode**: A fully optimized dark theme accessible via the side drawer.
*   **Dynamic Profile**: The drawer and profile pages automatically display the logged-in user's name and order count.

## 📁 Project Structure

*   `lib/main.dart`: Entry point of the application. Handles Firebase initialization and global theme state.
*   `lib/app.dart`: Defines the root widget, authentication routing logic, and named routes.
*   `lib/theme.dart`: Centralized theme definitions for both Light and Dark modes.
*   `lib/services/`:
    *   `auth_service.dart`: Manages Firebase Authentication tasks.
    *   `firestore_service.dart`: Handles all cloud database operations (Cart, Wishlist, Reviews, User Data).
    *   `api.dart`: Fetches product data from external REST APIs.
*   `lib/pages/`: Contains all UI screens (Login, Signup, Home, Cart, Profile, etc.).
*   `lib/models/`: Data classes for Product, CartItem, and FavoriteItem.
*   `lib/ui/widgets.dart`: Reusable custom UI components like buttons and icons.

## 🛠️ How to Run

### Prerequisites
1.  **Flutter SDK**: Ensure you have Flutter installed (`flutter doctor`).
2.  **Firebase Project**: 
    *   Create a project in the [Firebase Console](https://console.firebase.google.com/).
    *   Enable **Email/Password** Authentication.
    *   Create a **Firestore Database**.

### Setup
1.  **Clone the repository**:
    ```bash
    git clone https://github.com/youssef324/Laza-app.git
    cd mobile_project
    ```
2.  **Install dependencies**:
    ```bash
    flutter pub get
    ```
3.  **Firebase Configuration**:
    *   Configure your Firebase options using the FlutterFire CLI or by manually updating `lib/services/firebase_options.dart` with your project credentials.
4.  **Run the app**:
    ```bash
    flutter run
    ```

## 📦 Key Dependencies
*   `firebase_core`: Fundamental Firebase plugin.
*   `firebase_auth`: User authentication.
*   `cloud_firestore`: Real-time cloud database.
*   `http`: Network requests for product data.
*   `cupertino_icons`: Standard iOS-style icons.

