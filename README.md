# 📍 Deneyapkart 1A v2 ile GPS Konum Belirleme ve Haritalama

Bu proje, **Deneyapkart 1A v2** geliştirme kartı ve **Deneyap GPS & GLONASS** modülünü kullanarak anlık konum verisi (enlem/boylam) elde etmeyi ve bu verileri **Organic Maps** ile **uMap** platformları üzerinde görselleştirmeyi hedefler.

---

![Kapak Görseli](https://github.com/user-attachments/assets/4d99af60-dbae-4d1e-ab7d-c1ee8e7895b9)

---

## 🚀 Kullanılan Teknolojiler ve Araçlar

### 🔌 Donanım
* **Deneyapkart 1A v2** (ESP32 Tabanlı)
* **Deneyap GPS & GLONASS** Konum Belirleyici

### 💻 Yazılım / IDE
* **DeneyapKart IDE** (Arduino tabanlı geliştirme ortamı)

### 🗺️ Haritalama ve Görselleştirme
* **Organic Maps:** Çevrimdışı haritalama ve KML/GPX veri görüntüleme.
* **uMap:** OpenStreetMap tabanlı, özelleştirilebilir interaktif harita oluşturma aracı.

---

## 🛠️ Kurulum ve Kullanım

### 1. Donanım Bağlantısı
* Deneyap GPS & GLONASS modülünü, Deneyapkart üzerindeki **I2C** portuna veya uygun **UART** pinlerine bağlayın.

<img width="864" alt="Devre Şeması" src="https://github.com/user-attachments/assets/341e3865-fc1e-492a-a77e-3312b1bc7a00" />

### 2. Kodlama (DeneyapKart IDE)
* Deneyap kütüphanelerini IDE'nize dahil edin.
* GPS modülünden gelen **NMEA** verilerini ayıklamak için gerekli kodları yükleyin.
* Seri port ekranından koordinatların (**Latitude/Longitude**) akışını kontrol edin.

---

## 🗺️ Haritalama Süreci

### **A. Organic Maps Kullanımı**
1. Cihazdan alınan koordinatları `.kml` veya `.gpx` formatına dönüştürün.
2. Bu dosyayı Organic Maps uygulamasına aktararak konumları çevrimdışı harita üzerinde görün.

![Organic Maps Görseli](https://github.com/user-attachments/assets/8ccdff66-02b1-49ba-ac0c-88f6d8f9e94a)

---

### **B. [uMap](https://umap.openstreetmap.fr/) Kullanımı**
1. uMap platformuna gidin.
2. Yeni bir harita oluşturun ve **"Veri Katmanı Ekle"** seçeneği ile GPS verilerinizi yükleyin.

<img width="1919" alt="uMap Arayüzü" src="https://github.com/user-attachments/assets/54f9abb3-1669-4d53-b8ec-a2c58e2b9714" />

---

## 📝 Önemli Notlar
> ⚠️ **Uydu Bağlantısı:** GPS modülünün açık alanda "uydu kilidi" (fix) alması için birkaç dakika beklemeniz gerekebilir.
>
> 🛰️ **Hassasiyet:** Hassas konum verisi elde etmek için en az 4 uyduya bağlanılması önerilir.

---

## 👤 Geliştiriciler
* **Talha Yasin Tiryaki** - *Yönetim Bilişim Sistemleri*
* **Tamer Acar** - *Yönetim Bilişim Sistemleri*
