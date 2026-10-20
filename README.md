# SafeHer

SafeHer is a mobile safety and route-awareness platform designed for women and vulnerable travelers. It combines real-time location tracking, risk-aware route suggestions, emergency contact management, and SOS alerting.

## Features
- Safe route planning using lighting and crowd data
- Journey monitoring and route deviation detection
- Emergency contact management
- SOS alerts with offline queue support

## Tech Stack
- Android: Kotlin + Jetpack Compose + Firebase + Google Maps
- Backend: Python + FastAPI + Postgres + PostGIS

## Project Structure
```text
SafeHer/
├── app/
├── lighting_backend/
├── build.gradle.kts
├── settings.gradle.kts
├── gradlew
├── README.md
└── ...
```

## Getting Started
### Android app
1. Open the project in Android Studio.
2. Add your Google Maps key in `local.properties`:
   ```properties
   MAPS_API_KEY=your_google_maps_api_key_here
   ```
3. Add Firebase configuration in `app/google-services.json`.
4. Run the app with Android Studio or:
   ```bash
   ./gradlew assembleDebug
   ```

### Backend
```bash
cd lighting_backend
pip install -r requirements.txt
python -m uvicorn app.main:app --host 0.0.0.0 --port 8000 --reload
```
