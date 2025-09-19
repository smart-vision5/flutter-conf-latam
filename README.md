# FlutterConf LATAM 2025 App

The official mobile application for FlutterConf LATAM 2025, taking place at Universidad de las Américas in Quito, Ecuador on September 9-10, 2025.

## 🚀 Features

### 📱 Core Functionality
- **Event Overview**: Interactive home screen with countdown timer and venue information
- **Agenda Management**: Complete conference schedule with session details and filtering
- **Speaker Profiles**: Detailed speaker information with social media links and language preferences
- **Sponsor Directory**: Comprehensive sponsor showcase with tier-based organization
- **Venue Information**: Detailed venue details, directions, and accessibility information

### 🎨 User Experience
- **Bilingual Support**: Full English and Spanish localization
- **Dark Mode**: Complete dark theme support with Material 3 design
- **Accessibility**: Comprehensive accessibility features and semantic labels
- **Responsive Design**: Optimized for various screen sizes and orientations
- **Modern UI**: Clean, modern interface with Flutter's Material 3 design system

### 🏗️ Technical Features
- **Modular Architecture**: Clean separation of concerns with custom packages
- **State Management**: BLoC pattern for predictable state management
- **Offline Support**: Cached data for offline conference information
- **Firebase Integration**: Cloud functions for data synchronization
- **External Links**: Seamless integration with maps and social media

## 📱 Screenshots

### Home
<img src="assets/screenshots/home/home.png" alt="Home Screen" width="300"/>  
<img src="assets/screenshots/home/home_1.png" alt="Home Screen - Scroll" width="300"/>  
<img src="assets/screenshots/home/home_dark_mode.png" alt="Home Screen - Dark Mode" width="300"/>  
<img src="assets/screenshots/home/home_english.png" alt="Home Screen - English" width="300"/>

### Agenda
<img src="assets/screenshots/agenda/agenda.png" alt="Agenda Screen" width="300"/>  

### Details
**Session Details**  
<img src="assets/screenshots/details/session_details.png" alt="Session Details Screen" width="300"/>  

**Speaker Details**  
<img src="assets/screenshots/details/speaker_details.png" alt="Speaker Details Screen" width="300"/>  

### Venue
<img src="assets/screenshots/venue/venue.png" alt="Venue Screen" width="300"/>  
<img src="assets/screenshots/venue/venue_1.png" alt="Venue Screen - Additional View" width="300"/>  

### More
<img src="assets/screenshots/more/more.png" alt="More Screen" width="300"/>  

## 🏗️ Architecture

This project follows a clean, modular architecture with the following structure:

### Core Packages
- **`conf_shared_models`**: Data models and business logic
- **`conf_ui_kit`**: Reusable UI components and theming
- **`conf_core`**: Core functionality and utilities
- **`conf_cache`**: Local data caching and storage
- **`conf_data_source`**: Data source abstraction layer
- **`conf_cloud_functions_data_source`**: Firebase Cloud Functions integration

### Feature Packages
- **`agenda_repository`**: Agenda and session management
- **`speakers_repository`**: Speaker data management
- **`sponsors_repository`**: Sponsor information management

### App Structure
```
lib/
├── agenda/           # Agenda feature with BLoC pattern
├── speakers/         # Speaker management
├── sponsors/         # Sponsor showcase
├── venue/           # Venue information
├── session_details/ # Session detail views
├── speaker_details/ # Speaker profile views
├── home/            # Home screen and navigation
├── app/             # App configuration and localization
└── l10n/            # Internationalization files
```

## 🛠️ Tech Stack

- **Framework**: Flutter 3.7.0+
- **State Management**: BLoC (flutter_bloc)
- **Architecture**: Clean Architecture with Repository Pattern
- **UI**: Material 3 with custom theming
- **Localization**: Flutter Intl with ARB files
- **Backend**: Firebase Cloud Functions
- **Caching**: Local storage with conf_cache package
- **External Links**: url_launcher for maps and social media

## 🚀 Getting Started

### Prerequisites
- Flutter SDK 3.7.0 or higher
- Dart SDK 3.7.0 or higher
- Android Studio / VS Code with Flutter extensions
- Firebase project (for backend functionality)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/flutter-conf-latam-2025.git
   cd flutter-conf-latam-2025
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Configure Firebase** (Optional)
   - Copy `firebase_options_template.dart` to `firebase_options.dart`
   - Add your Firebase configuration

4. **Run the app**
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

## 🌍 Localization

The app supports multiple languages:
- English (en)
- Spanish (es)

Localization files are located in `lib/l10n/arb/` and generated automatically.

## 🎨 Theming

The app includes a comprehensive theming system with:
- Light and dark themes
- Custom Flutter brand colors
- Material 3 design system
- Consistent spacing and typography
- Custom UI components

## 📦 Dependencies

### Core Dependencies
- `flutter_bloc`: State management
- `equatable`: Value equality
- `firebase_core`: Firebase integration
- `url_launcher`: External link handling
- `intl`: Internationalization

### Development Dependencies
- `very_good_analysis`: Linting rules
- `flutter_launcher_icons`: App icon generation
- `flutter_test`: Testing framework

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🏢 Event Information

**FlutterConf LATAM 2025**
- **Date**: September 9-10, 2025
- **Venue**: Universidad de las Américas, Quito, Ecuador
- **Capacity**: 600 attendees
- **Languages**: English and Spanish

## 📞 Support

For support or questions about the app, please contact the FlutterConf LATAM team or open an issue in this repository.

---

Built with ❤️ for the Flutter community in Latin America