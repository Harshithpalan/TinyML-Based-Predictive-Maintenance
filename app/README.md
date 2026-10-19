# TinyML-Based Predictive Maintenance Flutter App

A Flutter mobile application for predictive maintenance using TinyML technology. This app monitors industrial equipment in real-time, predicts failures, and provides actionable insights to prevent downtime.

## Features

### Home Tab
- **System Status Overview**: Real-time display of overall system health
- **Quick Actions**: Access to common tasks like diagnosis, reports, and maintenance scheduling
- **Recent Alerts**: View the latest maintenance alerts and warnings
- **Key Metrics**: Active devices count, daily alerts, and system efficiency

### Monitoring Tab
- **Real-time Sensor Data**: Live monitoring of critical parameters
  - Vibration (mm/s)
  - Temperature (°C)
  - Pressure (PSI)
  - Current (A)
- **Visual Indicators**: Progress bars showing current readings vs thresholds
- **Color-coded Alerts**: Visual warnings when values exceed normal ranges

### Analytics Tab
- **Failure Prediction Chart**: Historical trend analysis using fl_chart
- **Maintenance History**: Log of past maintenance activities
- **Predictive Insights**: AI-powered failure probability predictions

### Settings Tab
- **Push Notifications**: Toggle maintenance alerts
- **Auto Diagnostics**: Configure automatic diagnostic runs
- **Dark Mode**: Theme preference
- **Bluetooth Settings**: Configure sensor connectivity
- **Data Sync**: Cloud synchronization options

## Tech Stack

- **Flutter**: 3.41.2
- **Dart**: 3.11.0
- **fl_chart**: 0.68.0 (for data visualization)
- **Material Design 3**: Modern UI components

## Getting Started

### Prerequisites
- Flutter SDK (3.41.2 or higher)
- Dart SDK (3.11.0 or higher)
- Android Studio / Xcode (for mobile development)
- VS Code or Android Studio (recommended IDE)

### Installation

1. Clone the repository:
```bash
cd "D:\TinyML-Based Predictive Maintenance\app"
```

2. Install dependencies:
```bash
flutter pub get
```

3. Run the app:
```bash
flutter run
```

### Building for Production

**Android:**
```bash
flutter build apk --release
```

**iOS:**
```bash
flutter build ios --release
```

**Web:**
```bash
flutter build web --release
```

## Project Structure

```
lib/
├── main.dart                 # App entry point
└── screens/
    └── dashboard_screen.dart # Main dashboard with 4 tabs
        ├── HomeTab
        ├── MonitoringTab
        ├── AnalyticsTab
        └── SettingsTab
```

## Future Enhancements

- [ ] Integrate TinyML models for on-device inference
- [ ] Add Bluetooth connectivity for real sensor data
- [ ] Implement cloud backend for data storage
- [ ] Add user authentication
- [ ] Export reports as PDF
- [ ] Push notification integration
- [ ] Machine learning model updates via OTA
- [ ] Multi-device support

## Architecture

The app follows a clean architecture pattern with:
- **Separation of Concerns**: UI separated from business logic
- **State Management**: StatefulWidget for local state
- **Material Design 3**: Modern, responsive UI components
- **Modular Design**: Each tab is a separate widget for maintainability

## License

This project is part of the TinyML-Based Predictive Maintenance initiative.

## Support

For issues or questions, please contact the development team.
