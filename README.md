# 📡 Türkiye Amatör Telsiz Röle Listesi

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform](https://img.shields.io/badge/Platform-Android-green.svg)](https://www.android.com/)
[![API](https://img.shields.io/badge/API-24%2B-brightgreen.svg)](https://android-arsenal.com/api?level=24)
[![Version](https://img.shields.io/badge/Version-1.0.0-blue.svg)](https://github.com/cektor/AmateurRadioRepeatersList)

[🇹🇷 Türkçe](README-TR.md) | 🇬🇧 English

<p align="center">
  <img src="repeaters.png" alt="App Logo" width="200"/>
</p>

## 📖 About

**Türkiye Amatör Telsiz Röle Listesi** is a comprehensive Android application designed for amateur radio operators in Turkey. The app provides an up-to-date list of repeater stations across Turkey with advanced filtering, location-based features, and offline capabilities.

### 🎯 Key Features

- 📍 **Location-Based Filtering** - Automatically detects your city and filters repeaters
- 📏 **Distance Calculation** - Shows distance from your location to each repeater
- 🗺️ **QTH Locator** - Generates Maidenhead grid square coordinates
- ⭐ **Favorites** - Save your frequently used repeaters
- 📶 **Offline Mode** - Access repeater data without internet connection
- 🔄 **Pull to Refresh** - Update data with a simple swipe gesture
- 📊 **Statistics** - View detailed statistics by regions and bands
- 🔗 **Share** - Share repeater information via any app
- 🌙 **Dark Theme** - Eye-friendly dark interface
- 📱 **Responsive Design** - Optimized for all screen sizes
- 🔔 **Notifications** - Get notified when new repeaters are added

### 🎨 Screenshots

<p align="center">
  <img src="screenshots/main.png" alt="Main Screen" width="200"/>
  <img src="screenshots/statistics.png" alt="Statistics" width="200"/>
  <img src="screenshots/about.png" alt="About" width="200"/>
</p>

## 🚀 Getting Started

### Prerequisites

- Android Studio Arctic Fox or later
- Android SDK 24 or higher
- Kotlin 1.9+
- Gradle 8.0+

### Installation

1. Clone the repository
```bash
git clone https://github.com/cektor/AmateurRadioRepeatersList.git
cd AmateurRadioRepeatersList
```

2. Open the project in Android Studio

3. Sync Gradle files

4. Run the app on an emulator or physical device

### Building APK

```bash
./gradlew assembleRelease
```

The APK will be generated in `app/build/outputs/apk/release/`

## 🏗️ Architecture

The app follows modern Android development practices:

- **Language:** Kotlin
- **Architecture:** MVVM-like pattern with lifecycle-aware components
- **UI:** Material Design 3 components
- **Networking:** Retrofit + OkHttp
- **Concurrency:** Kotlin Coroutines
- **Local Storage:** SharedPreferences
- **Location:** Google Play Services Location API
- **Dependency Injection:** Manual (lightweight approach)

### Project Structure

```
app/
├── src/
│   └── main/
│       ├── java/com/repeaters/
│       │   ├── MainActivity.kt          # Main screen with repeater list
│       │   ├── StatisticsActivity.kt    # Statistics screen
│       │   ├── AboutActivity.kt         # About screen
│       │   ├── ApiService.kt            # Retrofit API interface
│       │   ├── LocationHelper.kt        # Location and QTH utilities
│       │   ├── CacheManager.kt          # Local data management
│       │   ├── NotificationHelper.kt    # Push notification handler
│       │   ├── Repeater.kt              # Data model
│       │   └── RepeaterAdapter.kt       # RecyclerView adapter
│       ├── res/
│       │   ├── layout/                  # XML layouts
│       │   ├── drawable/                # Images and icons
│       │   ├── values/                  # Strings, colors, dimensions
│       │   └── anim/                    # Animations
│       └── AndroidManifest.xml
└── build.gradle.kts
```

## 🔧 Configuration

### API Endpoint

The app fetches data from:
```
https://amatortelsizcilik.com.tr/api/role/androidapi
```

### Permissions

- `INTERNET` - Required for fetching repeater data
- `ACCESS_NETWORK_STATE` - Check internet connectivity
- `ACCESS_FINE_LOCATION` - Precise location for distance calculation
- `ACCESS_COARSE_LOCATION` - Approximate location
- `POST_NOTIFICATIONS` - Notify about new repeaters (Android 13+)

For detailed information about data collection and privacy, see our [Privacy Policy](PRIVACY_POLICY.md).

## 📊 Features in Detail

### 1. Repeater List
- View all repeater stations in Turkey
- Filter by city, region (TA1-TA9), and band (VHF, UHF, Cross, APRS, Echolink)
- Sort by favorites and city
- Pagination (50 items per page)

### 2. Location Features
- Automatic city detection
- Distance calculation from your location
- QTH Locator (Maidenhead grid square)
- Integration with QTH Locator app

### 3. Offline Mode
- Cached repeater data
- Last update timestamp
- Works without internet connection

### 4. Statistics
- Total repeater count
- Digital and licensed repeater counts
- Distribution by regions (TA0-TA9)
- Distribution by bands
- Top 10 cities with most repeaters

### 5. Sharing
- Share repeater details via any app
- Includes all technical information
- Google Maps link for coordinates

## 🌍 TA Regions

| Region | Coverage |
|--------|----------|
| TA0 | Islands (Adalar) |
| TA1 | Çanakkale, Edirne, İstanbul, Kırklareli, Tekirdağ |
| TA2 | Ankara, Bartın, Bilecik, Bolu, Düzce, Eskişehir, İstanbul Asya, Karabük, Kırıkkale, Kocaeli, Sakarya, Yalova, Zonguldak |
| TA3 | Balıkesir, Bursa, Çanakkale Asya, İzmir, Manisa |
| TA4 | Afyon, Antalya, Aydın, Burdur, Denizli, Isparta, Kütahya, Muğla, Uşak |
| TA5 | Adana, Hatay, Aksaray, Karaman, Konya, Mersin, Nevşehir, Niğde, Osmaniye |
| TA6 | Amasya, Çankırı, Çorum, Kastamonu, Kırşehir, Samsun, Sinop, Tokat, Yozgat |
| TA7 | Bayburt, Erzincan, Giresun, Gümüşhane, Kayseri, Ordu, Sivas, Trabzon, Tunceli |
| TA8 | Adıyaman, Bingöl, Diyarbakır, Elazığ, Gaziantep, Kahramanmaraş, Kilis, Malatya, Mardin, Şanlıurfa, Şırnak |
| TA9 | Ağrı, Ardahan, Artvin, Batman, Bitlis, Erzurum, Hakkari, Iğdır, Kars, Muş, Rize, Siirt, Van |

## 🛠️ Technologies Used

- **Kotlin** - Primary programming language
- **Android SDK** - Android development framework
- **Material Design 3** - UI components
- **Retrofit** - REST API client
- **OkHttp** - HTTP client
- **Gson** - JSON serialization
- **Coroutines** - Asynchronous programming
- **Google Play Services** - Location services
- **SwipeRefreshLayout** - Pull-to-refresh functionality

## 🔒 Privacy

We take your privacy seriously. This app:
- Does NOT collect any personal information
- Does NOT collect or transmit location data (processes locally only)
- Does NOT track your location history
- Processes all data locally on your device
- Does NOT share any data with third parties
- Does NOT store user data on our servers

Read our full [Privacy Policy](PRIVACY_POLICY.md) for details.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2026 ALG Yazılım & Elektronik Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 👨‍💻 Developer

**ALG Yazılım & Elektronik Inc.** © 2026

- **Developer:** Fatih ÖNDER (TB1TFO - CekToR)
- **Email:** info@algyazilim.com
- **Website:** [https://algyazilim.com](https://algyazilim.com)

## ⚡ Powered By

<p align="center">
  <a href="https://qrv73.com">
    <img src="qrv73.png" alt="QRV73" width="150"/>
  </a>
</p>

**QRV73.com** - Online Amateur Radio Platform

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🐛 Bug Reports

If you find a bug, please open an issue with:
- Device model and Android version
- Steps to reproduce
- Expected behavior
- Actual behavior
- Screenshots (if applicable)

## 📮 Contact

For questions, suggestions, or support:
- **Email:** info@algyazilim.com
- **Website:** [https://algyazilim.com](https://algyazilim.com)

## 🙏 Acknowledgments

- Data provided by [amatortelsizcilik.com.tr](https://amatortelsizcilik.com.tr)
- Powered by [QRV73.com](https://qrv73.com)
- Turkish Amateur Radio Community

## 📱 Download

Coming soon on Google Play Store!

---

**73!** 🎙️

*Made with ❤️ for the Turkish Amateur Radio Community*
