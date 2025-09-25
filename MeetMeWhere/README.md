# MeetMeWhere

Android event management and social meetup app.  
Users can register, create events, RSVP, view events in list/map views, and share photos.  

![Cover](../docs/screenshots/MeetMeWhere-cover.png)

## ✨ Features
- Secure user registration + login with Firebase Auth
- Create, update, delete events
- RSVP functionality with attendee counts
- Event list (RecyclerView) + map view integration
- Photo sharing for events
- Gamification elements to encourage engagement
- Offline support via Room database (sync with Firestore)

## 🧱 Tech Stack
- Android (Kotlin)
- Firebase Authentication + Firestore
- Room Database
- RecyclerView + ViewBinding
- Google Maps SDK (for map view)

## 🚀 Quick Start
### Prerequisites
- Android Studio installed
- Emulator or Android device
- Firebase project (update google-services.json)

### Run
1. Open folder in Android Studio  
2. Sync Gradle  
3. Run on emulator or device  

## 🔐 Environment / Secrets
- Place your `google-services.json` in `/app`  
- Configure Firebase project in the console (Auth + Firestore)  

## 📐 Architecture Notes
- MVVM with ViewModel + LiveData
- Firestore for real-time sync
- Room for local persistence
- Adapter pattern for RecyclerView
- Lambdas for update/delete callbacks

## 🧪 Tests
- Unit tests for ViewModels
- Instrumented tests with Espresso (optional)

## 📸 Screenshots
Add images to `../docs/screenshots` and name one:
- `MeetMeWhere-cover.png` (home screen or event list)
- `MeetMeWhere-event.png` (event detail page)
