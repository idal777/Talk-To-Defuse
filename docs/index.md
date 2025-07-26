# 💣 Talk To Defuse – Fiziksel Modüler Bomba İmha Oyunu

> 🎮 *"Keep Talking and Nobody Explodes"* oyununa gerçek donanım geldi.  
> 🛠️ Açık kaynaklı, geliştirilebilir, modüler bir bomba imha deneyimi.

---

## 🚀 Proje Nedir?

**Talk to Defuse**, takım çalışması, iletişim ve mühendislik becerilerini oyunlaştırarak öğreten fiziksel bir bomba imha oyunudur.  
Oyuncular bir bombayı etkisiz hale getirmeye çalışırken, diğer oyuncular uzaktan yönergeler verir. Proje tamamen açık kaynaklıdır ve Arduino temellidir.

🎯 **Hedefimiz:**  
Maker, öğrenci ve oyun tutkunlarını bir araya getirerek eğlenceli ve öğretici bir deneyim sunmak.

---

## 🌟 Projenin Vizyonu ve Hakkında

Bu projenin temel vizyonu, fiziksel oyun sistemleri ve maker kültürü alanında kullanıcı dostu, erişilebilir ve açık kaynaklı bir çözüm sunmaktır.  
Geliştiricilere, öğrencilere ve oyun severlere hem öğretici hem de yaratıcı bir deneyim sağlamak hedeflenmiştir.

### 📌 Neden Bu Proje?

- Gerçek dünyadaki teknik problemleri eğlenceli bir formatla çözümlemeyi öğretmek  
- Açık kaynak topluluğuna katkı sağlamak  
- Eğitim süreçlerinde kullanılabilecek örnek bir platform sunmak  
- Donanım-yazılım entegrasyonunu eğlenceli hale getirmek

### 🎯 Hedeflerimiz

- Tak-çalıştır yapıda, kolay kurulum  
- Her seviyeden kullanıcıya hitap eden dökümantasyon  
- Sürekli güncellenen açık bir geliştirme modeli  
- Topluluk geri bildirimlerine dayalı evrim

---

## ⚙️ Nasıl Çalışır?

📦 Sistem, fiziksel olarak birbirine bağlanan **modüllerden** oluşur. Her biri Arduino mikrodenetleyici ile kontrol edilir ve I2C protokolü ile ana modüle bağlanır.

🧩 Oyun Süreci:
1. ⏱️ Süre ve modül sayısı ana modül tarafından başlatılır  
2. 🔄 Modüller aktifleşir ve görevler başlar  
3. 🔌 Oyuncular modülleri kontrol eder ve sorunları çözmeye çalışır  
4. 💬 Yardımcı oyuncu, yönergeleri ileten kişidir  
5. 🎉 Bomba zamanında etkisiz hale getirilirse takım kazanır

---

## 🧠 Modül Sistemi

- 🔗 **Tak-Çalıştır** yapısı (her modül kolayca eklenip çıkarılır)
- 🧱 **Bağımsız firmware** ve I2C haberleşme
- 🛠️ **Topluluk katkısına açık** geliştirme modeli

📚 Modül yazılım/donanım belgeleri:  
👉 [Modüller](modules.md)

---

## 🔬 Teknik Detaylar

| Alan         | İçerik                                            |
|--------------|---------------------------------------------------|
| 💡 Donanım   | Arduino Nano/Uno, I2C, LED, buzzer, ekran, buton  |
| 💻 Yazılım   | Arduino IDE, özel modül kütüphaneleri             |
| 🧾 Belgeler  | Tüm modüller için teknik dökümantasyon             |
| 🧪 Prototipleme | Breadboard → PCB dönüşümü                     |

🔗 Daha fazla teknik içerik için:  
👉 [Parçalar Listesi](temelparcalar.md)  
👉 [3D Modeller](3dmodeller.md)

---

## 🌍 Topluluk ve Gelişim

Talk to Defuse, açık kaynak fiziksel oyunlar arasında ilham veren bir proje olmayı hedefler.  
👥 Topluluk desteğiyle gelişen bu proje, farklı disiplinleri (elektronik, yazılım, oyun tasarımı) bir araya getirir.

Katkıda bulunmak için → [Katkı Rehberi](contributing.md)

---

## 📦 Hızlı Başlangıç

```bash
git clone https://github.com/idal777/Talk-To-Defuse
cd Talk-To-Defuse
mkdocs serve







