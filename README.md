# ✦ Lilithian · Cadı Bildirgeci & Göksel Takvim

**Gerçek konumunuza göre Güneş, Ay, gezegenler ve Black Moon Lilith’in doğuş/batış saatlerini hesaplayan, 9:16 video arka planlı etkileşimli bir cadı bildirgecidir.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub repo](https://img.shields.io/badge/GitHub-metatronslove%2Flilithian-blue?logo=github)](https://github.com/metatronslove/lilithian)

---

## 📖 Proje Hakkında

**Lilithian**, arka planda YouTube'dan 9:16 oranında döngüsel bir video oynatırken, ön planda **astronomy-engine** kütüphanesi ile hesaplanan gök cisimlerinin (Güneş, Ay, Merkür, Venüs, Mars, Jüpiter, Satürn, Uranüs, Neptün ve Black Moon Lilith) anlık konumlarını ve doğuş/batış saatlerini sunar.

Tüm içerikler (bitkiler, kristaller, ritüeller) gerçek bilimsel verilerle (botanik, mineraloji) harmanlanmıştır ve günlük olarak değişir. Bu proje, hem mistik hem de bilimsel merakı tek bir zarif arayüzde buluşturur.

---

## ✨ Mevcut Özellikler

- 📱 **Tam Ekran 9:16 Video Arka Plan** – YouTube videosu sesli, kontrolsüz ve döngülü.
- 🌍 **Gerçek Konum Desteği** – GPS/Konum izni ile bulunduğunuz enlem/boylam baz alınır.
- ☀️ **Gökyüzü Takvimi** – 9 gezegen + Ay ve Güneş için **doğuş/batış saatleri** ve **burç bilgileri**.
- 🜁 **Lilith (Black Moon)** – Yaklaşık ekliptik boylamı ve burç konumu.
- 🌿 **Bilimsel Bitki & Kristal Ansiklopedisi** – Günlük değişen öneriler ve kimyasal/fiziksel açıklamalar.
- 🕯 **Dinamik Ritüel Rehberi** – Günün astronomik verilerine göre oluşturulmuş adım adım niyet ritüeli.
- 🎨 **4 Sekmeli Zarif Arayüz** – Bildirge, Gökyüzü, Ansiklopedi ve Ritüel arasında geçiş.

---

## 🚀 Kurulum (Çalıştırma)

Projeyi yerel bilgisayarınızda çalıştırmak için:

```bash
git clone https://github.com/metatronslove/lilithian.git
cd lilithian
```

Dosyayı doğrudan tarayıcıda açabilirsiniz:
- Ana dosya `/docs/index.html` klasöründe yer almaktadır.
- **Önemli:** YouTube iframe'i ve Geolocation API nedeniyle, dosyayı `http://` veya `https://` ile sunan bir sunucuda (örn. VS Code Live Server) çalıştırmanız önerilir.

---

## 🧩 Proje Yapısı

```
/
├── docs/
│   └── index.html          # Ana uygulama (tüm CSS/JS tek dosyada)
├── README.md               # Bu doküman
└── LICENSE                 # (Opsiyonel) MIT Lisansı
```

---

## 🔮 Geliştirme Önerileri & Yapay Zeka Destekli Uygulama Rehberi

Aşağıda, bu projeyi fork edip geliştirmek isteyenler için **35'ten fazla somut öneri** bulunmaktadır. Her önerinin yanında, mevcut **Yapay Zeka (ChatGPT, Claude, GitHub Copilot, DeepSeek, vb.)** araçlarını kullanarak bunu nasıl başarabileceğinize dair pratik bir ipucu verilmiştir.

---

### 🌐 1. Çok Dilli (i18n / Uluslararasılaştırma) Destek

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **İngilizce, Almanca, Fransızca, İspanyolca dillerini ekleyin.** | `index.html` içindeki tüm metinleri (etiketler, başlıklar, bitki açıklamaları, ritüel adımları) kopyalayıp ChatGPT'ye yapıştırın ve "Bunu İngilizce, Almanca ve İspanyolcaya çevir ve JSON formatında çıktı ver (tr.json, en.json, de.json, es.json)" deyin. Ardından sayfaya bir dil seçici dropdown ekleyin ve JS ile `innerHTML`'leri bu JSON'dan doldurun. |
| **Tarayıcı diline göre otomatik dil seçimi.** | `navigator.language` ile kullanıcının varsayılan dilini algılayıp, uygun JSON'u yüklemek için AI'dan bir kod parçası isteyin. |
| **Sağdan sola (RTL) diller için destek (Arapça, İbranice).** | AI'ya "CSS'de `dir="rtl"` özelliğini tüm panele uygulayan ve metinleri yeniden hizalayan kod parçası oluştur" deyin. |

---

### 📱 2. Mobil / Android & iOS Uygulamasına Dönüştürme

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **Progressive Web App (PWA) yapın.** | AI'ya "Bu HTML dosyasını PWA'ya dönüştürmek için manifest.json ve service-worker.js kodlarını oluştur" deyin. Böylece kullanıcılar sayfayı ana ekrana ekleyip uygulama gibi kullanabilir. |
| **Android (WebView) APK çıkarın.** | "Bu proje için Android WebView sarmalayıcı oluştur. AndroidManifest.xml ve MainActivity.java kodlarını ver" diyerek basit bir APK oluşturun. |
| **Capacitor veya Cordova ile paketleyin.** | AI'dan "Capacitor kurulum adımlarını ve `capacitor.config.json` dosyasını oluştur" isteyin. Çıkan dosyayı Android Studio veya Xcode ile derleyin. |
| **React Native veya Flutter ile yeniden yazın.** | Mevcut HTML/JS'yi AI'ya verip "Bu arayüzü React Native (veya Flutter) widget'larına dönüştür" diyerek mobil-native bir sürüm oluşturun. |

---

### 🧠 3. Yapay Zeka ile İçerik Üretimi & Kişiselleştirme

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **Günlük mesajı AI ile oluşturun.** | `generateDailyMessage()` fonksiyonunu, OpenAI veya Claude API'sine bağlayın. AI'ya "Bugünün Ay evresi ve burcu şu, bana 50 kelimelik ilham verici cadı mesajı yaz" komutunu göndermesi için JS kodu oluşturtun. |
| **Kullanıcı günlüğü / not defteri ekleyin.** | AI'dan "LocalStorage kullanarak kullanıcının günlük ritüel notlarını kaydeden bir textarea kodu yaz" isteyin. |
| **Kişisel burç yorumu (doğum haritası).** | Kullanıcıdan doğum tarihi/saati isteyin, AI'dan "Doğum haritasındaki gezegen konumlarını hesaplamak için bir fonksiyon yaz" deyin (astronomy-engine ile mümkün). |
| **Rüya günlüğü entegrasyonu.** | Kullanıcıların rüyalarını kaydedebileceği ve AI'nın bunları yorumlayabileceği bir bölüm ekleyin. AI'dan "Rüya metnini analiz edip sembolik anlam çıkaran API bağlantısı" kurmasını isteyin. |

---

### 🌟 4. Astronomik Verileri Genişletme

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **Asteroitler (Ceres, Pallas, vb.) ekleyin.** | `astronomy-engine` dokümanlarını AI'ya verip "Asteroitlerin yörünge elemanlarını ekleyerek doğuş/batış hesaplama kodunu genişlet" deyin. |
| **Güneş ve Ay tutulmaları uyarısı.** | AI'dan "Bir sonraki güneş/ay tutulmasını hesapla ve bildirim göster" fonksiyonu yazmasını isteyin. |
| **Meteor yağmurları takvimi.** | Belirli tarihleri (Perseid, Leonid) içeren bir dizi oluşturun ve AI'dan bu tarihler yaklaştığında uyarı veren mantığı yazmasını isteyin. |
| **Sabit yıldızlar (Spica, Sirius, Regulus) ekleyin.** | Parlak sabit yıldızların koordinatlarını (RA/Dec) girip doğuş/batışlarını hesaplatın. AI'dan "Bu yıldızlar için verileri astronomy-engine ile kullan" kodunu isteyin. |
| **Galaktik merkez (Sagittarius A*) konumu.** | Galaktik merkezin Dünya'dan görünen konumunu hesaplayıp gökyüzü haritasına ekleyin. |

---

### 🎨 5. Tema, Tasarım ve Kullanıcı Deneyimi

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **Karanlık / Aydınlık tema geçişi.** | CSS değişkenlerini (custom properties) kullanarak, AI'dan "Karanlık mod için alternatif renk paleti oluştur ve JS ile toggle et" kodunu isteyin. |
| **Arka plan videosunu değiştirme (kullanıcı seçimi).** | Kullanıcının farklı 9:16 videolar arasından seçim yapması için bir galeri ekleyin. AI'dan "YouTube embed URL'lerini değiştiren bir fonksiyon yaz" deyin. |
| **Daha fazla animasyon ve geçiş efekti.** | "CSS ile yıldız kayması veya ay fazı döngüsü animasyonu ekle" diyerek AI'dan hazır CSS snippet'leri alın. |
| **Arka plan müziği (isteğe bağlı).** | Kullanıcının açıp kapatabileceği, videodan bağımsız ortam sesleri (yağmur, rüzgar) ekleyin. Bunun için HTML5 Audio elementlerini AI ile oluşturun. |
| **3D Gökyüzü Haritası (Three.js veya A-Frame).** | AI'dan "Three.js ile dönen bir gökküresi oluştur, gezegen konumlarını işaretle" kodunu isteyerek etkileşimli bir 3D harita ekleyin. |

---

### 📡 6. Harici API ve Veri Entegrasyonu

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **Hava durumu entegrasyonu (bulut örtüsü gözlem için).** | OpenWeatherMap API'sini entegre edin. AI'dan "Hava durumu API'sinden bulutluluk oranını al ve gözlem notu olarak ekle" kodunu isteyin. |
| **Güneş patlamaları (Space Weather) bilgisi.** | NASA veya NOAA'nın açık verilerini çeken bir API bağlantısı ekleyin. AI, bu verileri çekip özetleyen JS kodunu yazabilir. |
| **Konum adresini (il/ilçe) otomatik doldurma.** | Nominatim (OpenStreetMap) ile ters coğrafi kodlama yaparak enlem/boylamı adrese çevirin. AI'ya "Reverse geocoding kodu yaz" deyin. |
| **Namaz / Yoga vakitleri entegrasyonu (isteğe bağlı).** | Gün doğumu/gün batımına göre alternatif zaman dilimlerini (ör. tan vakti, mavi saat) hesaplayıp gösterin. |

---

### 📊 7. Veri Depolama ve Senkronizasyon

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **Günlük verileri Firebase / Supabase ile bulutta saklayın.** | AI'dan "Firebase Realtime Database bağlantı kodu oluştur, kullanıcının o günkü ritüel notlarını kaydet" isteyin. |
| **Birden fazla cihazda senkronizasyon.** | Kullanıcı girişi (email/şifre) ekleyerek, her hesabın kendi tercihlerini (dil, video tercihi, favori bitkiler) saklamasını sağlayın. |
| **Geçmiş arşiv (geçmiş günlerin bildirgelerini görme).** | Her günün verisini LocalStorage veya IndexedDB'ye kaydedin. AI'dan "Tarih seçici ekleyerek geçmiş verileri çağıran kod" isteyin. |
| **Verileri CSV/JSON olarak dışa aktarma.** | Kullanıcının tüm ritüel notlarını ve gözlemlerini dışa aktarabileceği bir buton ekleyin. |

---

### 🛡️ 8. Performans ve Erişilebilirlik (A11y)

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **Lazy loading ve kod bölme (Code splitting).** | `astronomy-engine` gibi büyük kütüphaneleri dynamic import ile yükleyin. AI'dan "ES module dynamic import kullanarak astronomy-engine'i sadece Gökyüzü sekmesi açıldığında yükle" kodunu isteyin. |
| **Ekran okuyucu (Screen Reader) desteği.** | Tüm butonlara, panellere `aria-label` ekleyin. AI'ya "Bu HTML'e erişilebilirlik etiketleri ekle" deyin ve çıktıyı kopyalayın. |
| **Düşük bant genişliği modu (videoyu kapat).** | Kullanıcının bağlantı hızı düşükse video arka planını durağan bir resimle değiştirin. AI'dan "Network Information API ile bağlantı hızını kontrol eden kod" isteyin. |
| **Offline destek (Service Worker).** | AI'ya "Temel HTML/CSS/JS'i cache'leyen ve çevrimdışı çalışmayı sağlayan service-worker.js yaz" deyin. |

---

### 🧪 9. Gelişmiş Bilimsel ve Astrolojik Veriler

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **Gerçek Lilith (Osculating) hesaplaması.** | Şu anki basit formül yerine, gerçek yörünge elemanlarını kullanarak daha hassas Lilith konumu hesaplayın. AI'dan "Osculating elements for Black Moon Lilith" formülünü araştırmasını ve kodlamasını isteyin. |
| **Astrolojik transit (gezegen geçişleri) etkileri.** | Gezegenlerin günlük açılarını (kavuşum, kare, üçgen) hesaplayan bir modül ekleyin. AI'dan "Gezegen açıları hesaplama fonksiyonu" yazmasını isteyin. |
| **Ev sistemi (Placidus / Koch) hesaplama.** | Doğum haritası için ev çizgilerini hesaplayan bir algoritma ekleyin (astronomy-engine ile mümkün). |
| **Güneş merkezli (Heliocentric) görünüm.** | Dünya merkezli değil, Güneş merkezli konumları da gösteren bir toggle ekleyin. |

---

### 🤖 10. Otomasyon ve Geliştirici Araçları

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **GitHub Actions ile otomatik deploy (Pages).** | AI'dan `.github/workflows/deploy.yml` dosyası oluşturmasını isteyin. Her push işleminde `docs/` klasörünü otomatik yayınlasın. |
| **Unit testler ekleyin.** | "Astronomy hesaplamaları için Jest test kodları yaz" diyerek AI'dan test senaryoları oluşturun. |
| **ESLint / Prettier ile kod formatı.** | AI'ya "Bu kod için `.eslintrc.json` ve `.prettierrc` dosyası oluştur" deyin. |
| **Docker ile konteynerleştirme.** | AI'dan "Bu statik siteyi Nginx ile servis eden bir Dockerfile oluştur" isteyin. |

---

### 📦 11. Ek Paket / Modül Geçişi

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **astronomy-engine'i npm ile yükleyip modüler hale getirin.** | Tek dosyadan kurtulup, `import` yapısına geçin. AI'dan "Webpack veya Vite ile bu projeyi modüler hale getir" adımlarını isteyin. |
| **Vue.js / React / Svelte ile yeniden yazın.** | Mevcut HTML/JS'yi alıp "Bunu React fonksiyonel bileşenlerine dönüştür" deyin. AI size dönüştürülmüş kod parçalarını verecektir. |
| **TypeScript'e geçiş.** | AI'dan "Bu JavaScript kodunu TypeScript'e çevir, interface ve type tanımlarını ekle" isteyin. |

---

### 🌿 12. İçerik Zenginleştirme

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **Bitki ve kristal veritabanını 100+ öğeye çıkarın.** | AI'dan "Bana 50 farklı şifalı bitki ve 50 farklı kristal listesi hazırla, bilimsel açıklamalarıyla birlikte (botanik adı ve kimyasal formülü ile)" isteyin. Çıkan listeyi doğrudan JS'ye yapıştırın. |
| **Mevsimsel tarımsal takvim (ekim/dikim günleri).** | Ay evresine göre "yer üstü / yer altı" bitkileri dikim takvimi ekleyin. AI'dan "Ay evresine göre bahçe takvimi oluşturma mantığı" yazmasını isteyin. |
| **Tarot / Rün çekimi (günlük fal).** | Rastgele bir kart veya rün seçip anlamını gösteren ikinci bir modül ekleyin. AI'dan "78 kartlık Tarot destesi verisi ve çekim fonksiyonu" oluşturmasını isteyin. |
| **Uçucu yağ / tütsü karışımı önerileri.** | Günün bitkisine göre aromaterapi karışımı tarifleri ekleyin. |
| **Mantra / Niyet cümlesi veritabanı.** | Her gün için farklı bir niyet cümlesi veya mantra ekleyin. AI'dan "100 farklı niyet cümlesi listesi oluştur" isteyin. |

---

### 🔔 13. Bildirim ve Hatırlatıcılar

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **Tarayıcı bildirimleri (Push API).** | AI'dan "Her gün belirli bir saatte kullanıcıya bugünün bildirgesini hatırlatan Push bildirim kodu" yazmasını isteyin (Service Worker ile). |
| **E-posta bülteni (günlük özet).** | Kullanıcının e-posta adresini alıp, her gün otomatik olarak günün bildirgesini gönderen bir sistem kurun. AI'dan "SendGrid veya Resend ile e-posta gönderme fonksiyonu" isteyin. |
| **Telegram / Discord botu entegrasyonu.** | Günlük bildirgeyi otomatik olarak bir Telegram kanalına veya Discord sunucusuna gönderen bir bot kodu oluşturun. |

---

### 🧩 14. Topluluk ve Sosyal Özellikler

| Öneri | Yapay Zeka ile Nasıl Yapılır? |
| :--- | :--- |
| **Günlük bildirgeyi sosyal medyada paylaşma.** | Twitter/X veya Instagram'da paylaşmak için görsel (OG image) oluşturma ve paylaşım linki ekleyin. AI'dan "Canvas ile günlük bildirgeyi resme çeviren kod" isteyin. |
| **Yorum / yorum yapma sistemi (basit).** | Kullanıcıların kendi ritüel deneyimlerini paylaşabileceği bir yorum alanı ekleyin (Firebase veya supabase ile). |
| **Haftalık / Aylık istatistikler.** | Kullanıcının en çok hangi bitki veya kristalle etkileşime girdiğini gösteren basit bir dashboard ekleyin. |

---

## 🤝 Katkıda Bulunma (Contributing)

Yukarıdaki önerilerden herhangi birini uyguladıysanız, lütfen bir **Pull Request** gönderin! Bu projeyi en iyi hale getirmek için tüm katkılara açığız.

1. Bu depoyu fork edin (`metatronslove/lilithian`).
2. Kendi dalınızı oluşturun (`git checkout -b feature/yeni-ozellik`).
3. Değişikliklerinizi işleyin (`git commit -m 'Yeni özellik: ...'`).
4. Dalınıza push edin (`git push origin feature/yeni-ozellik`).
5. Bir Pull Request açın.

---

## 📜 Lisans

Bu proje MIT Lisansı ile lisanslanmıştır. Dilediğiniz gibi kullanabilir, ticari projelerinize dahil edebilirsiniz.

---

## 🌌 Teşekkürler

- [Astronomy Engine](https://github.com/gmiller/astronomy-engine) - Tüm göksel hesaplamalar için.
- YouTube - Arka plan görsel videosu için.

---

**Hazırlayan:** metatronslove  
**Proje Linki:** [https://github.com/metatronslove/lilithian](https://github.com/metatronslove/lilithian)

---

⭐ Bu projeyi beğendiyseniz yıldız vermeyi unutmayın! Her gün yeni bir bildirge sizi bekliyor. 
