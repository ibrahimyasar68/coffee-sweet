☕ Coffee Sweet & Loyalty App
Bu proje, modern bir kahve dükkanı deneyimini sadakat programıyla birleştiren, Flutter kullanılarak geliştirilmiş mobil bir uygulamadır. Kullanıcıların ürünleri inceleyebileceği, sepetlerine ekleyebileceği ve alışveriş yaptıkça puan kazanabileceği bütüncül bir yapı sunar.

🚀 Özellikler
Dinamik Ürün Listeleme: Kategorilere ayrılmış (Sıcak/Soğuk) kahve menüsü.

Gelişmiş Arama: Ürünler arasında anlık isimle arama yapabilme.

Sepet Yönetimi: Ürün ekleme, çıkarma ve toplam tutar hesaplama.

Sadakat Sistemi: Yapılan her alışverişten kazanılan puanların kullanıcı profiline yansıtılması.

Kalıcı Veri Depolama: Uygulama kapansa dahi verilerin kaybolmamasını sağlayan yerel veritabanı.

Yönetici Paneli: Uygulama içerisinden yeni ürün ekleme ve Hive veritabanına kaydetme.

🛠 Kullanılan Teknolojiler ve Mimari
Uygulama, sürdürülebilir ve ölçeklenebilir bir kod yapısı için MVVM (Model-View-ViewModel) benzeri bir yaklaşımla geliştirilmiştir:

Flutter: UI Framework.

Provider: State Management (Durum Yönetimi) çözümü olarak kullanıldı. Uygulama genelinde veri akışı reaktif bir şekilde sağlanır.

Hive: NoSQL yerel veritabanı. Nesne tabanlı (Object-oriented) depolama ve yüksek performans için tercih edildi.

Hive Adapters: Coffee ve User modelleri özel adaptörler aracılığıyla doğrudan diskte saklanır.

📂 Proje Yapısı
Plaintext
lib/
├── models/         # Veri modelleri (Coffee, User) ve Hive Adaptörleri
├── providers/      # İş mantığı (Logic) ve State Management sınıfları
├── screens/        # Uygulama sayfaları (Home, Cart, AddProduct vb.)
├── widgets/        # Tekrar kullanılabilir UI bileşenleri
└── main.dart       # Uygulamanın giriş noktası ve servislerin başlatılması
⚙️ Kurulum
Projeyi yerel makinenizde çalıştırmak için:

Bu depoyu klonlayın:

Bash
git clone https://github.com/ibrahimyasar68/coffee_shop_loyalty.git
Proje dizinine gidin:

Bash
cd coffee_shop_loyalty
Bağımlılıkları yükleyin:

Bash
flutter pub get
Hive adaptörlerini oluşturun (Gerekliyse):

Bash
flutter pub run build_runner build
Uygulamayı çalıştırın:

Bash
flutter run
Geliştirici: İbrahim Yaşar

Lisans: MIT
