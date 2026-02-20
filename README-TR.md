# 📡 Türkiye Amatör Telsiz Röle Listesi

[![Lisans: MIT](https://img.shields.io/badge/Lisans-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform](https://img.shields.io/badge/Platform-Android-green.svg)](https://www.android.com/)
[![API](https://img.shields.io/badge/API-24%2B-brightgreen.svg)](https://android-arsenal.com/api?level=24)
[![Versiyon](https://img.shields.io/badge/Versiyon-1.0.0-blue.svg)](https://github.com/cektor/AmateurRadioRepeatersList)

🇹🇷 Türkçe | [🇬🇧 English](README.md)

<p align="center">
  <img src="repeaters.png" alt="Uygulama Logosu" width="200"/>
</p>

## 📖 Hakkında

**Türkiye Amatör Telsiz Röle Listesi**, Türkiye'deki amatör telsiz operatörleri için tasarlanmış kapsamlı bir Android uygulamasıdır. Uygulama, Türkiye genelindeki röle istasyonlarının güncel listesini gelişmiş filtreleme, konum tabanlı özellikler ve çevrimdışı yeteneklerle sunar.

### 🎯 Temel Özellikler

- 📍 **Konum Bazlı Filtreleme** - Şehrinizi otomatik algılar ve röleleri filtreler
- 📏 **Mesafe Hesaplama** - Konumunuzdan her röleye olan mesafeyi gösterir
- 🗺️ **QTH Locator** - Maidenhead grid kare koordinatları oluşturur
- ⭐ **Favoriler** - Sık kullandığınız röleleri kaydedin
- 📶 **Çevrimdışı Mod** - İnternet bağlantısı olmadan röle verilerine erişin
- 🔄 **Aşağı Çekerek Yenile** - Basit bir kaydırma hareketiyle verileri güncelleyin
- 📊 **İstatistikler** - Bölgelere ve bantlara göre detaylı istatistikleri görüntüleyin
- 🔗 **Paylaş** - Röle bilgilerini herhangi bir uygulama ile paylaşın
- 🌙 **Karanlık Tema** - Göz dostu karanlık arayüz
- 📱 **Responsive Tasarım** - Tüm ekran boyutları için optimize edilmiş
- 🔔 **Bildirimler** - Yeni röleler eklendiğinde bildirim alın

### 🎨 Ekran Görüntüleri

<p align="center">
  <img src="screenshots/main.png" alt="Ana Ekran" width="200"/>
  <img src="screenshots/statistics.png" alt="İstatistikler" width="200"/>
  <img src="screenshots/about.png" alt="Hakkında" width="200"/>
</p>

## 🚀 Başlangıç

### Gereksinimler

- Android Studio Arctic Fox veya üzeri
- Android SDK 24 veya üzeri
- Kotlin 1.9+
- Gradle 8.0+

### Kurulum

1. Depoyu klonlayın
```bash
git clone https://github.com/cektor/AmateurRadioRepeatersList.git
cd AmateurRadioRepeatersList
```

2. Projeyi Android Studio'da açın

3. Gradle dosyalarını senkronize edin

4. Uygulamayı emülatör veya fiziksel cihazda çalıştırın

### APK Oluşturma

```bash
./gradlew assembleRelease
```

APK, `app/build/outputs/apk/release/` dizininde oluşturulacaktır.

## 🏗️ Mimari

Uygulama, modern Android geliştirme uygulamalarını takip eder:

- **Dil:** Kotlin
- **Mimari:** Yaşam döngüsü farkında bileşenlerle MVVM benzeri desen
- **UI:** Material Design 3 bileşenleri
- **Ağ:** Retrofit + OkHttp
- **Eşzamanlılık:** Kotlin Coroutines
- **Yerel Depolama:** SharedPreferences
- **Konum:** Google Play Services Location API
- **Bağımlılık Enjeksiyonu:** Manuel (hafif yaklaşım)

### Proje Yapısı

```
app/
├── src/
│   └── main/
│       ├── java/com/repeaters/
│       │   ├── MainActivity.kt          # Röle listesi ana ekran
│       │   ├── StatisticsActivity.kt    # İstatistikler ekranı
│       │   ├── AboutActivity.kt         # Hakkında ekranı
│       │   ├── ApiService.kt            # Retrofit API arayüzü
│       │   ├── LocationHelper.kt        # Konum ve QTH yardımcıları
│       │   ├── CacheManager.kt          # Yerel veri yönetimi
│       │   ├── NotificationHelper.kt    # Push bildirim işleyici
│       │   ├── Repeater.kt              # Veri modeli
│       │   └── RepeaterAdapter.kt       # RecyclerView adaptörü
│       ├── res/
│       │   ├── layout/                  # XML düzenler
│       │   ├── drawable/                # Resimler ve simgeler
│       │   ├── values/                  # String'ler, renkler, boyutlar
│       │   └── anim/                    # Animasyonlar
│       └── AndroidManifest.xml
└── build.gradle.kts
```

## 🔧 Yapılandırma

### API Uç Noktası

Uygulama verileri şuradan alır:
```
https://amatortelsizcilik.com.tr/api/role/androidapi
```

### İzinler

- `INTERNET` - Röle verilerini almak için gerekli
- `ACCESS_NETWORK_STATE` - İnternet bağlantısını kontrol et
- `ACCESS_FINE_LOCATION` - Mesafe hesaplama için kesin konum
- `ACCESS_COARSE_LOCATION` - Yaklaşık konum
- `POST_NOTIFICATIONS` - Yeni röleler hakkında bildirim (Android 13+)

Veri toplama ve gizlilik hakkında detaylı bilgi için [Gizlilik Politikamızı](PRIVACY_POLICY.md) inceleyin.

## 📊 Özellikler Detaylı

### 1. Röle Listesi
- Türkiye'deki tüm röle istasyonlarını görüntüleyin
- Şehir, bölge (TA1-TA9) ve bant (VHF, UHF, Cross, APRS, Echolink) ile filtreleyin
- Favorilere ve şehre göre sıralayın
- Sayfalama (sayfa başına 50 öğe)

### 2. Konum Özellikleri
- Otomatik şehir algılama
- Konumunuzdan mesafe hesaplama
- QTH Locator (Maidenhead grid kare)
- QTH Locator uygulaması ile entegrasyon

### 3. Çevrimdışı Mod
- Önbelleğe alınmış röle verileri
- Son güncelleme zaman damgası
- İnternet bağlantısı olmadan çalışır

### 4. İstatistikler
- Toplam röle sayısı
- Dijital ve ruhsatlı röle sayıları
- Bölgelere göre dağılım (TA0-TA9)
- Bantlara göre dağılım
- En çok röleye sahip ilk 10 şehir

### 5. Paylaşım
- Röle detaylarını herhangi bir uygulama ile paylaşın
- Tüm teknik bilgileri içerir
- Koordinatlar için Google Maps bağlantısı

## 🌍 TA Bölgeleri

| Bölge | Kapsam |
|-------|--------|
| TA0 | Adalar |
| TA1 | Çanakkale, Edirne, İstanbul, Kırklareli, Tekirdağ |
| TA2 | Ankara, Bartın, Bilecik, Bolu, Düzce, Eskişehir, İstanbul Asya, Karabük, Kırıkkale, Kocaeli, Sakarya, Yalova, Zonguldak |
| TA3 | Balıkesir, Bursa, Çanakkale Asya, İzmir, Manisa |
| TA4 | Afyon, Antalya, Aydın, Burdur, Denizli, Isparta, Kütahya, Muğla, Uşak |
| TA5 | Adana, Hatay, Aksaray, Karaman, Konya, Mersin, Nevşehir, Niğde, Osmaniye |
| TA6 | Amasya, Çankırı, Çorum, Kastamonu, Kırşehir, Samsun, Sinop, Tokat, Yozgat |
| TA7 | Bayburt, Erzincan, Giresun, Gümüşhane, Kayseri, Ordu, Sivas, Trabzon, Tunceli |
| TA8 | Adıyaman, Bingöl, Diyarbakır, Elazığ, Gaziantep, Kahramanmaraş, Kilis, Malatya, Mardin, Şanlıurfa, Şırnak |
| TA9 | Ağrı, Ardahan, Artvin, Batman, Bitlis, Erzurum, Hakkari, Iğdır, Kars, Muş, Rize, Siirt, Van |

## 🛠️ Kullanılan Teknolojiler

- **Kotlin** - Birincil programlama dili
- **Android SDK** - Android geliştirme çerçevesi
- **Material Design 3** - UI bileşenleri
- **Retrofit** - REST API istemcisi
- **OkHttp** - HTTP istemcisi
- **Gson** - JSON serileştirme
- **Coroutines** - Asenkron programlama
- **Google Play Services** - Konum hizmetleri
- **SwipeRefreshLayout** - Aşağı çekerek yenileme işlevi

## 🔒 Gizlilik

Gizliliğinizi ciddiye alıyoruz. Bu uygulama:
- Hiçbir kişisel bilgi TOPLAMAZ
- Konum verilerini TOPLAMAZ veya İLETMEZ (yalnızca yerel olarak işler)
- Konum geçmişinizi TAKİP ETMEZ
- Tüm verileri cihazınızda yerel olarak işler
- Verileri üçüncü taraflarla PAYLAŞMAZ
- Sunucularımızda kullanıcı verisi SAKLAMAZ

Detaylar için [Gizlilik Politikamızı](PRIVACY_POLICY.md) okuyun.

## 📝 Lisans

Bu proje MIT Lisansı altında lisanslanmıştır - detaylar için [LICENSE](LICENSE) dosyasına bakın.

```
MIT Lisansı

Telif Hakkı (c) 2026 ALG Yazılım & Elektronik Inc.

İşbu belge ile, bu yazılımın ve ilgili dokümantasyon dosyalarının ("Yazılım")
bir kopyasını edinen herhangi bir kişiye, Yazılım'ı kullanma, kopyalama,
değiştirme, birleştirme, yayınlama, dağıtma, alt lisanslama ve/veya satma
hakları da dahil olmak üzere, Yazılım'da herhangi bir kısıtlama olmaksızın
işlem yapma izni ücretsiz olarak verilir ve Yazılım'ın sağlandığı kişilere
aşağıdaki koşullara tabi olarak izin verilir:

Yukarıdaki telif hakkı bildirimi ve bu izin bildirimi, Yazılım'ın tüm
kopyalarına veya önemli bölümlerine dahil edilecektir.

YAZILIM "OLDUĞU GİBİ" SAĞLANIR, TİCARİ ELVERİŞLİLİK, BELİRLİ BİR AMACA
UYGUNLUK VE İHLAL ETMEME GARANTİLERİ DE DAHİL OLMAK ÜZERE AÇIK VEYA ZIMNİ
HİÇBİR GARANTİ OLMAKSIZIN. HİÇBİR DURUMDA YAZARLAR VEYA TELİF HAKKI SAHİPLERİ,
YAZILIM'DAN VEYA YAZILIM'IN KULLANIMI VEYA DİĞER İŞLEMLERİNDEN KAYNAKLANAN,
BUNLARLA BAĞLANTILI VEYA BUNLARDAN DOĞAN HERHANGİ BİR İDDİA, HASAR VEYA DİĞER
YÜKÜMLÜLÜKLERDEN SORUMLU TUTULAMAZ.
```

## 👨💻 Geliştirici

**ALG Yazılım & Elektronik Inc.** © 2026

- **Geliştirici:** Fatih ÖNDER (TB1TFO - CekToR)
- **E-posta:** info@algyazilim.com
- **Web Sitesi:** [https://algyazilim.com](https://algyazilim.com)

## ⚡ Destekleyen

<p align="center">
  <a href="https://qrv73.com">
    <img src="qrv73.png" alt="QRV73" width="150"/>
  </a>
</p>

**QRV73.com** - Online Amatör Telsiz Platformu

## 🤝 Katkıda Bulunma

Katkılar memnuniyetle karşılanır! Lütfen bir Pull Request göndermekten çekinmeyin.

1. Projeyi fork edin
2. Özellik dalınızı oluşturun (`git checkout -b feature/HarikaBirOzellik`)
3. Değişikliklerinizi commit edin (`git commit -m 'Harika bir özellik ekle'`)
4. Dalınıza push yapın (`git push origin feature/HarikaBirOzellik`)
5. Bir Pull Request açın

## 🐛 Hata Raporları

Bir hata bulursanız, lütfen şunları içeren bir issue açın:
- Cihaz modeli ve Android sürümü
- Hatayı yeniden oluşturma adımları
- Beklenen davranış
- Gerçekleşen davranış
- Ekran görüntüleri (varsa)

## 📮 İletişim

Sorular, öneriler veya destek için:
- **E-posta:** info@algyazilim.com
- **Web Sitesi:** [https://algyazilim.com](https://algyazilim.com)

## 🙏 Teşekkürler

- Veriler [amatortelsizcilik.com.tr](https://amatortelsizcilik.com.tr) tarafından sağlanmaktadır
- [QRV73.com](https://qrv73.com) tarafından desteklenmektedir
- Türk Amatör Telsiz Topluluğu

## 📱 İndir

Yakında Google Play Store'da!

---

**73!** 🎙️

*Türk Amatör Telsiz Topluluğu için ❤️ ile yapılmıştır*
