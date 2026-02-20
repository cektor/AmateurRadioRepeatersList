# Privacy Policy | Gizlilik Politikası

**Last Updated | Son Güncelleme:** January 2025

---

## 🇬🇧 English

### Introduction

ALG Yazılım & Elektronik Inc. ("we", "our", or "us") operates the **Türkiye Amatör Telsiz Röle Listesi** mobile application (the "App"). This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you use our App.

By using the App, you agree to the collection and use of information in accordance with this policy. If you do not agree with the terms of this Privacy Policy, please do not use the App.

### Information We Collect

#### 1. Location Data

**What we process (NOT collect):**
- GPS coordinates (latitude and longitude)
- City and region information
- QTH Locator (Maidenhead grid square)

**Why we process it:**
- To calculate distances between your location and repeater stations
- To automatically filter repeaters by your current city
- To generate QTH Locator coordinates for amateur radio operations
- To provide location-based features and improve user experience

**How we use it:**
- Location data is processed **ONLY on your device**
- We do **NOT collect or store** your location data on our servers
- We do **NOT transmit** your location data anywhere
- We do **NOT track** your movements or location history
- Location data is used in real-time and immediately discarded
- No location data leaves your device

**Permissions required:**
- `ACCESS_FINE_LOCATION` - For precise distance calculations
- `ACCESS_COARSE_LOCATION` - For city-level filtering

#### 2. Internet/Network Access

**What we collect:**
- Network connectivity status
- API request logs (temporary, for debugging purposes only)

**Why we collect it:**
- To fetch updated repeater data from our API
- To check if offline mode should be activated
- To ensure data synchronization

**How we use it:**
- Network access is used only to download repeater information
- We do NOT collect browsing history or other network activities
- Connection data is not stored permanently

**Permissions required:**
- `INTERNET` - To fetch repeater data from our API
- `ACCESS_NETWORK_STATE` - To detect online/offline status

#### 3. Notification Data

**What we collect:**
- Notification preferences (enabled/disabled)
- Device push notification token (if notifications are enabled)

**Why we collect it:**
- To notify you when new repeaters are added to the database
- To send important updates about the App

**How we use it:**
- Notification tokens are stored securely
- We only send notifications related to repeater updates
- You can disable notifications at any time in your device settings

**Permissions required:**
- `POST_NOTIFICATIONS` (Android 13+) - To send push notifications

#### 4. Local Storage Data

**What we store locally:**
- Cached repeater data (for offline mode)
- Your favorite repeaters list
- App preferences and settings
- Last data update timestamp

**Why we store it:**
- To enable offline access to repeater information
- To remember your favorite repeaters
- To improve app performance and reduce data usage

**How we use it:**
- All data is stored locally on your device using SharedPreferences
- This data never leaves your device
- You can clear this data by uninstalling the App

### Data We Do NOT Collect

We want to be transparent about what we **DO NOT** collect:

- ❌ Personal identification information (name, email, phone number)
- ❌ Amateur radio call signs or license information
- ❌ Payment or financial information
- ❌ Device identifiers (IMEI, MAC address, etc.)
- ❌ Contacts or phonebook data
- ❌ Photos, videos, or media files
- ❌ Microphone or camera access
- ❌ SMS or call logs
- ❌ Location data (we process it locally but DO NOT collect it)
- ❌ Location history or tracking data
- ❌ Browsing history or search queries
- ❌ Any personally identifiable information (PII)

**IMPORTANT:** We do NOT collect, store, or transmit ANY user data to our servers. All data processing happens locally on your device.

### Third-Party Services

#### API Data Source

The App fetches repeater data from:
```
https://amatortelsizcilik.com.tr/api/role/androidapi
```

This API provides public information about amateur radio repeater stations in Turkey. No personal data is sent to this API.

#### Google Play Services

We use Google Play Services Location API for location features. Google's privacy policy applies to their services:
- [Google Privacy Policy](https://policies.google.com/privacy)

### Data Security

We take data security seriously:

- 🔒 All API communications use HTTPS encryption
- 🔒 Location data is processed locally and never transmitted
- 🔒 No user accounts or authentication required
- 🔒 No personal data is stored on our servers
- 🔒 Local data is protected by Android's security model

### Data Retention

- **Location Data:** NOT retained - processed in real-time only and immediately discarded
- **Cached Repeater Data:** Stored locally until you clear app data or uninstall
- **Favorites:** Stored locally until you clear app data or uninstall
- **Notification Tokens:** Deleted when you uninstall the App

**IMPORTANT:** No user data is stored on our servers. Everything is local to your device.

### Your Rights and Choices

You have the following rights:

#### Location Permissions
- You can revoke location permissions at any time in Android Settings
- The App will continue to work without location features
- Distance calculations and city filtering will be disabled

#### Notifications
- You can disable notifications in Android Settings
- You will still receive app updates through the Play Store

#### Data Deletion
- Uninstalling the App removes all locally stored data
- No data remains on our servers (we don't store user data)

### Children's Privacy

The App does not knowingly collect information from children under 13. The App is designed for amateur radio operators who typically hold licenses requiring minimum age requirements.

### Changes to This Privacy Policy

We may update this Privacy Policy from time to time. We will notify you of any changes by:
- Posting the new Privacy Policy in the App
- Updating the "Last Updated" date
- Sending a notification (if significant changes occur)

### Open Source and Transparency

This App's source code is available on GitHub, allowing full transparency of our data practices. You can review exactly how your data is handled by examining the code.

### Contact Us

If you have questions about this Privacy Policy, please contact us:

- **Email:** info@algyazilim.com
- **Website:** [https://algyazilim.com](https://algyazilim.com)
- **Developer:** ALG Yazılım & Elektronik Inc.

### Legal Compliance

This Privacy Policy complies with:
- Google Play Store Developer Policies
- Android App Privacy Requirements
- General Data Protection Regulation (GDPR) principles
- Turkish Personal Data Protection Law (KVKK)

---

## 🇹🇷 Türkçe

### Giriş

ALG Yazılım & Elektronik Inc. ("biz", "bizim" veya "bize") **Türkiye Amatör Telsiz Röle Listesi** mobil uygulamasını ("Uygulama") işletmektedir. Bu Gizlilik Politikası, Uygulamamızı kullandığınızda bilgilerinizi nasıl topladığımızı, kullandığımızı, ifşa ettiğimizi ve koruduğumuzu açıklar.

Uygulamayı kullanarak, bu politikaya uygun olarak bilgilerin toplanmasını ve kullanılmasını kabul etmiş olursunuz. Bu Gizlilik Politikası şartlarını kabul etmiyorsanız, lütfen Uygulamayı kullanmayın.

### Topladığımız Bilgiler

#### 1. Konum Verileri

**Ne işliyoruz (TOPLAMIYORUZ):**
- GPS koordinatları (enlem ve boylam)
- Şehir ve bölge bilgileri
- QTH Locator (Maidenhead grid karesi)

**Neden işliyoruz:**
- Konumunuz ile röle istasyonları arasındaki mesafeyi hesaplamak için
- Röleleri bulunduğunuz şehre göre otomatik filtrelemek için
- Amatör telsiz operasyonları için QTH Locator koordinatları oluşturmak için
- Konum tabanlı özellikler sağlamak ve kullanıcı deneyimini iyileştirmek için

**Nasıl kullanıyoruz:**
- Konum verileri **YALNIZCA cihazınızda** işlenir
- Konum verilerinizi sunucularımızda **TOPLAMIYORUZ veya SAKLAMIYORUZ**
- Konum verilerinizi hiçbir yere **İLETMİYORUZ**
- Hareketlerinizi veya konum geçmişinizi **TAKİP ETMİYORUZ**
- Konum verileri gerçek zamanlı kullanılır ve hemen silinir
- Hiçbir konum verisi cihazınızdan ayrılmaz

**Gerekli izinler:**
- `ACCESS_FINE_LOCATION` - Hassas mesafe hesaplamaları için
- `ACCESS_COARSE_LOCATION` - Şehir düzeyinde filtreleme için

#### 2. İnternet/Ağ Erişimi

**Ne topluyoruz:**
- Ağ bağlantı durumu
- API istek kayıtları (geçici, yalnızca hata ayıklama amaçlı)

**Neden topluyoruz:**
- API'mizden güncellenmiş röle verilerini almak için
- Çevrimdışı modun etkinleştirilip etkinleştirilmeyeceğini kontrol etmek için
- Veri senkronizasyonunu sağlamak için

**Nasıl kullanıyoruz:**
- Ağ erişimi yalnızca röle bilgilerini indirmek için kullanılır
- Tarayıcı geçmişi veya diğer ağ etkinliklerini TOPLAMIYORUZ
- Bağlantı verileri kalıcı olarak saklanmaz

**Gerekli izinler:**
- `INTERNET` - API'mizden röle verilerini almak için
- `ACCESS_NETWORK_STATE` - Çevrimiçi/çevrimdışı durumu tespit etmek için

#### 3. Bildirim Verileri

**Ne topluyoruz:**
- Bildirim tercihleri (etkin/devre dışı)
- Cihaz push bildirim token'ı (bildirimler etkinse)

**Neden topluyoruz:**
- Veritabanına yeni röleler eklendiğinde sizi bilgilendirmek için
- Uygulama hakkında önemli güncellemeler göndermek için

**Nasıl kullanıyoruz:**
- Bildirim token'ları güvenli bir şekilde saklanır
- Yalnızca röle güncellemeleriyle ilgili bildirimler gönderiyoruz
- Bildirimleri istediğiniz zaman cihaz ayarlarından devre dışı bırakabilirsiniz

**Gerekli izinler:**
- `POST_NOTIFICATIONS` (Android 13+) - Push bildirimleri göndermek için

#### 4. Yerel Depolama Verileri

**Yerel olarak ne saklıyoruz:**
- Önbelleğe alınmış röle verileri (çevrimdışı mod için)
- Favori röleler listeniz
- Uygulama tercihleri ve ayarları
- Son veri güncelleme zaman damgası

**Neden saklıyoruz:**
- Röle bilgilerine çevrimdışı erişimi etkinleştirmek için
- Favori rölelerinizi hatırlamak için
- Uygulama performansını artırmak ve veri kullanımını azaltmak için

**Nasıl kullanıyoruz:**
- Tüm veriler SharedPreferences kullanılarak cihazınızda yerel olarak saklanır
- Bu veriler asla cihazınızdan ayrılmaz
- Uygulamayı kaldırarak bu verileri temizleyebilirsiniz

### Toplamadığımız Veriler

**TOPLAMADIKLERIMIZ** konusunda şeffaf olmak istiyoruz:

- ❌ Kişisel kimlik bilgileri (ad, e-posta, telefon numarası)
- ❌ Amatör telsiz çağrı işaretleri veya lisans bilgileri
- ❌ Ödeme veya finansal bilgiler
- ❌ Cihaz tanımlayıcıları (IMEI, MAC adresi, vb.)
- ❌ Kişiler veya telefon rehberi verileri
- ❌ Fotoğraflar, videolar veya medya dosyaları
- ❌ Mikrofon veya kamera erişimi
- ❌ SMS veya arama kayıtları
- ❌ Konum verileri (yerel olarak işliyoruz ama TOPLAMIYORUZ)
- ❌ Konum geçmişi veya takip verileri
- ❌ Tarayıcı geçmişi veya arama sorguları
- ❌ Herhangi bir kişisel tanımlanabilir bilgi (KTB)

**ÖNEMLİ:** Sunucularımıza HİÇBİR kullanıcı verisi toplamıyor, saklamıyor veya iletmiyoruz. Tüm veri işleme cihazınızda yerel olarak gerçekleşir.

### Üçüncü Taraf Hizmetler

#### API Veri Kaynağı

Uygulama, röle verilerini şu adresten alır:
```
https://amatortelsizcilik.com.tr/api/role/androidapi
```

Bu API, Türkiye'deki amatör telsiz röle istasyonları hakkında kamuya açık bilgiler sağlar. Bu API'ye hiçbir kişisel veri gönderilmez.

#### Google Play Hizmetleri

Konum özellikleri için Google Play Services Location API kullanıyoruz. Google'ın gizlilik politikası hizmetleri için geçerlidir:
- [Google Gizlilik Politikası](https://policies.google.com/privacy)

### Veri Güvenliği

Veri güvenliğini ciddiye alıyoruz:

- 🔒 Tüm API iletişimleri HTTPS şifrelemesi kullanır
- 🔒 Konum verileri yerel olarak işlenir ve asla iletilmez
- 🔒 Kullanıcı hesabı veya kimlik doğrulama gerekmez
- 🔒 Sunucularımızda hiçbir kişisel veri saklanmaz
- 🔒 Yerel veriler Android'in güvenlik modeli tarafından korunur

### Veri Saklama

- **Konum Verileri:** Saklanmaz - yalnızca gerçek zamanlı işlenir ve hemen silinir
- **Önbelleğe Alınmış Röle Verileri:** Uygulama verilerini temizleyene veya kaldırana kadar yerel olarak saklanır
- **Favoriler:** Uygulama verilerini temizleyene veya kaldırana kadar yerel olarak saklanır
- **Bildirim Token'ları:** Uygulamayı kaldırdığınızda silinir

**ÖNEMLİ:** Sunucularımızda hiçbir kullanıcı verisi saklanmaz. Her şey cihazınızda yereldir.

### Haklarınız ve Seçimleriniz

Aşağıdaki haklara sahipsiniz:

#### Konum İzinleri
- Konum izinlerini istediğiniz zaman Android Ayarları'ndan iptal edebilirsiniz
- Uygulama, konum özellikleri olmadan çalışmaya devam edecektir
- Mesafe hesaplamaları ve şehir filtreleme devre dışı kalacaktır

#### Bildirimler
- Bildirimleri Android Ayarları'ndan devre dışı bırakabilirsiniz
- Play Store üzerinden uygulama güncellemelerini almaya devam edeceksiniz

#### Veri Silme
- Uygulamayı kaldırmak, yerel olarak saklanan tüm verileri kaldırır
- Sunucularımızda hiçbir veri kalmaz (kullanıcı verisi saklamıyoruz)

### Çocukların Gizliliği

Uygulama, 13 yaşın altındaki çocuklardan bilerek bilgi toplamaz. Uygulama, genellikle minimum yaş gereksinimleri olan lisanslara sahip amatör telsiz operatörleri için tasarlanmıştır.

### Bu Gizlilik Politikasındaki Değişiklikler

Bu Gizlilik Politikasını zaman zaman güncelleyebiliriz. Değişiklikleri şu yollarla size bildireceğiz:
- Yeni Gizlilik Politikasını Uygulama içinde yayınlayarak
- "Son Güncelleme" tarihini güncelleyerek
- Bildirim göndererek (önemli değişiklikler olursa)

### Açık Kaynak ve Şeffaflık

Bu Uygulamanın kaynak kodu GitHub'da mevcuttur ve veri uygulamalarımızın tam şeffaflığını sağlar. Kodu inceleyerek verilerinizin tam olarak nasıl işlendiğini görebilirsiniz.

### Bize Ulaşın

Bu Gizlilik Politikası hakkında sorularınız varsa, lütfen bizimle iletişime geçin:

- **E-posta:** info@algyazilim.com
- **Web Sitesi:** [https://algyazilim.com](https://algyazilim.com)
- **Geliştirici:** ALG Yazılım & Elektronik Inc.

### Yasal Uyumluluk

Bu Gizlilik Politikası şunlara uygundur:
- Google Play Store Geliştirici Politikaları
- Android Uygulama Gizlilik Gereksinimleri
- Genel Veri Koruma Yönetmeliği (GDPR) ilkeleri
- Türkiye Kişisel Verilerin Korunması Kanunu (KVKK)

---

## 📋 Permission Summary | İzin Özeti

| Permission | Purpose (EN) | Amaç (TR) |
|------------|--------------|-----------|
| `INTERNET` | Fetch repeater data from API | API'den röle verilerini almak |
| `ACCESS_NETWORK_STATE` | Check online/offline status | Çevrimiçi/çevrimdışı durumu kontrol etmek |
| `ACCESS_FINE_LOCATION` | Calculate precise distances | Hassas mesafeleri hesaplamak |
| `ACCESS_COARSE_LOCATION` | Filter by city | Şehre göre filtrelemek |
| `POST_NOTIFICATIONS` | Notify about new repeaters | Yeni röleler hakkında bildirim göndermek |

---

## 🔒 Data Protection Principles | Veri Koruma İlkeleri

### English
- **Minimization:** We only collect data necessary for app functionality
- **Purpose Limitation:** Data is used only for stated purposes
- **Transparency:** This policy clearly explains our practices
- **Security:** We implement appropriate security measures
- **User Control:** You control your data and permissions
- **No Selling:** We never sell or share your data with third parties

### Türkçe
- **Minimizasyon:** Yalnızca uygulama işlevselliği için gerekli verileri topluyoruz
- **Amaç Sınırlaması:** Veriler yalnızca belirtilen amaçlar için kullanılır
- **Şeffaflık:** Bu politika uygulamalarımızı açıkça açıklar
- **Güvenlik:** Uygun güvenlik önlemlerini uyguluyoruz
- **Kullanıcı Kontrolü:** Verilerinizi ve izinlerinizi siz kontrol edersiniz
- **Satış Yok:** Verilerinizi asla üçüncü taraflara satmaz veya paylaşmayız

---

**73!** 🎙️

*Made with ❤️ for the Turkish Amateur Radio Community*

*Türk Amatör Telsiz Topluluğu için ❤️ ile yapılmıştır*
