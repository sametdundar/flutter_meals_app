# 🍽️ Meals App

Lezzetli yemek tariflerini keşfetmek için tasarlanmış modern bir Flutter uygulaması.

## 📱 Özellikler

- **Kategori Bazlı Tarifler**: İtalyan, Alman, Asya, Fransız ve daha fazla mutfak kategorisi
- **Detaylı Tarif Bilgileri**: Malzemeler, adımlar, pişirme süresi ve zorluk seviyesi
- **Favoriler Sistemi**: Beğendiğiniz tarifleri favorilere ekleyin
- **Çoklu Dil Desteği**: Türkçe ve İngilizce dil desteği
- **Tema Desteği**: Aydınlık, karanlık ve sistem teması seçenekleri
- **Responsive Tasarım**: Tüm cihaz boyutlarında mükemmel görünüm
- **Modern UI/UX**: Material Design 3 ile güncel tasarım

## 🏗️ Proje Yapısı

```
lib/
├── data/
│   ├── dummy_data.dart      # Örnek yemek ve kategori verileri
│   └── notifiers.dart       # State management
├── models/
│   ├── category.dart        # Kategori modeli
│   └── meal.dart           # Yemek modeli
├── providers/
│   └── theme_provider.dart  # Tema yönetimi
├── screens/
│   ├── category_screen.dart # Kategori listesi ekranı
│   ├── meals_screen.dart    # Yemek listesi ekranı
│   ├── meal_details_screen.dart # Yemek detay ekranı
│   └── settings_screen.dart # Ayarlar ekranı
├── widgets/
│   ├── category_grid_item.dart # Kategori grid öğesi
│   ├── meal_item.dart       # Yemek listesi öğesi
│   └── meal_item_meatadata.dart # Yemek meta verileri
├── main.dart               # Uygulama giriş noktası
└── widget_tree.dart        # Ana widget ağacı
```

## 🚀 Kurulum

### Gereksinimler

- Flutter SDK (3.8.1 veya üzeri)
- Dart SDK
- Android Studio / VS Code
- Git

### Adımlar

1. **Projeyi klonlayın**
   ```bash
   git clone [repository-url]
   cd Meals-App-main
   ```

2. **Bağımlılıkları yükleyin**
   ```bash
   flutter pub get
   ```

3. **Uygulamayı çalıştırın**
   ```bash
   flutter run
   ```

## 📦 Kullanılan Teknolojiler

- **Flutter**: Cross-platform mobil geliştirme framework'ü
- **Provider**: State management
- **Easy Localization**: Çoklu dil desteği
- **Google Fonts**: Özel font desteği
- **Shared Preferences**: Yerel veri saklama
- **Material Design 3**: Modern UI bileşenleri

## 🎨 Ekran Görüntüleri

### Ana Ekranlar
- **Kategori Ekranı**: Farklı mutfak kategorilerini grid görünümünde listeler
- **Yemek Listesi**: Seçilen kategoriye ait tarifleri gösterir
- **Tarif Detayı**: Malzemeler, adımlar ve beslenme bilgileri
- **Favoriler**: Kaydedilen tariflerin listesi
- **Ayarlar**: Tema ve dil seçenekleri

## 🔧 Özelleştirme

### Yeni Kategori Ekleme
`lib/data/dummy_data.dart` dosyasındaki `availableCategories` listesine yeni kategori ekleyin:

```dart
Category(id: 'c11', title: 'Yeni Kategori', color: Colors.blue),
```

### Yeni Tarif Ekleme
`dummyMeals` listesine yeni tarif ekleyin:

```dart
Meal(
  id: 'm20',
  categories: ['c1', 'c2'],
  title: 'Yeni Tarif',
  // ... diğer özellikler
),
```

### Yeni Dil Ekleme
1. `assets/translations/` klasörüne yeni dil dosyası ekleyin
2. `lib/main.dart` dosyasında `supportedLocales` listesine ekleyin

## 🌐 Desteklenen Diller

- 🇹🇷 Türkçe (varsayılan)
- 🇺🇸 İngilizce

## 🎯 Özellikler Detayı

### Yemek Kategorileri
- İtalyan Mutfağı
- Hızlı & Kolay
- Hamburgerler
- Alman Mutfağı
- Hafif & Lezzetli
- Egzotik
- Kahvaltı
- Asya Mutfağı
- Fransız Mutfağı
- Yaz Tarifleri

### Tarif Bilgileri
- Malzeme listesi
- Adım adım talimatlar
- Pişirme süresi
- Zorluk seviyesi
- Fiyat kategorisi
- Beslenme bilgileri (Gluten, Vegan, Vejetaryen, Laktoz)

## 📱 Platform Desteği

- ✅ Android
- ✅ iOS
- ✅ Web
- ✅ Windows
- ✅ macOS
- ✅ Linux

## 🤝 Katkıda Bulunma

1. Bu repository'yi fork edin
2. Yeni bir branch oluşturun (`git checkout -b feature/yeni-ozellik`)
3. Değişikliklerinizi commit edin (`git commit -am 'Yeni özellik eklendi'`)
4. Branch'inizi push edin (`git push origin feature/yeni-ozellik`)
5. Pull Request oluşturun

## 📄 Lisans

Bu proje MIT lisansı altında lisanslanmıştır.

## 👨‍💻 Geliştirici

Bu proje Flutter öğrenme amaçlı geliştirilmiştir.

---

**Not**: Bu uygulama eğitim amaçlı geliştirilmiştir ve gerçek bir yemek tarifi veritabanı kullanmamaktadır. Tüm veriler örnek amaçlıdır.
