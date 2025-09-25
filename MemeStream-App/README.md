# MemeStream-App

Android client for a simple social app.  
Users can sign in, view a feed, and create posts. Pairs with the **MemeStream-API** backend.

![Cover](../docs/screenshots/MemeStream-App-cover.png)

## ✨ Features
- Login & JWT token storage (from API)
- View posts feed (RecyclerView)
- Create new post (text + optional image)
- Edit/Delete own posts (optional)
- Error handling & loading states

## 🧱 Tech Stack
- Android (Kotlin)
- Retrofit + OkHttp (API calls)
- ViewBinding / Jetpack components
- Glide or Coil (image loading)

## 🚀 Quick Start
### Prerequisites
- Android Studio
- Running **MemeStream-API** (see `../MemeStream-API` README)
- API base URL configured in app (e.g., `BuildConfig.API_BASE_URL`)

### Run
1. Open the project in Android Studio  
2. Update API base URL if needed  
3. Sync Gradle and Run on emulator/device

## 🔐 Environment
- Store API base URL in `local.properties` or a `BuildConfig` field
- Do **not** commit secrets/keys

## 📐 Architecture Notes
- MVVM or simple MVC (depending on your implementation)
- Repository class wraps Retrofit service
- RecyclerView Adapter for feed
- Token stored in SharedPreferences (or DataStore)

## 🧪 Tests
- Unit tests for repository/viewmodel (optional)

## 📸 Screenshots
Add images to `../docs/screenshots`:
- `MemeStream-App-cover.png` (feed screen)
- `MemeStream-App-compose.png` (create post)
