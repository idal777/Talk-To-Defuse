# Sorun Giderme (Troubleshooting)

Bu sayfada, "Talk to Defuse" projesiyle ilgili karşılaşabileceğiniz yaygın sorunlar ve bunların çözümleri yer almaktadır. Eğer burada çözümünü bulamadığınız bir problem olursa, lütfen **[İletişim](contact.md)** sayfasından bizimle iletişime geçiniz.

---

## 1. Kurulum Sorunları

### MkDocs Kurulumunda Hata Alıyorum
- Python yüklü ve güncel mi kontrol edin.
- `pip install mkdocs mkdocs-material` komutunu tekrar çalıştırın.
- Komut satırında `mkdocs` komutunu çalıştırdığınız dizinde `mkdocs.yml` dosyasının var olduğundan emin olun.

### Geliştirme Sunucusu Başlamıyor
- Terminalde `mkdocs serve` komutunu çalıştırırken "Config file 'mkdocs.yml' does not exist" hatası alıyorsanız, projenizin kök dizininde olduğunuzdan emin olun.
- `mkdocs.yml` dosyasının dosya adı ve uzantısını doğru yazdığınızdan emin olun.

---

## 2. Dokümantasyon Hataları

### Sayfalar Görünmüyor veya Boş
- `mkdocs.yml` dosyasındaki `nav` kısmında belirtilen dosya isimlerinin tam olarak `docs` klasöründeki dosya isimleriyle eşleştiğini kontrol edin.
- Dosya uzantılarının `.md` olduğundan ve doğru klasörde bulunduğundan emin olun.

### Bağlantılar Çalışmıyor
- Sayfa içi linklerde ve `nav` yapılandırmasında dosya yollarını doğru yazdığınızdan emin olun.
- Dosya isimlerinde boşluk ve büyük-küçük harf uyumuna dikkat edin.

---

## 3. Donanım Modülleri Sorunları

### Modül Çalışmıyor
- Arduino bağlantılarınızı ve pin konfigürasyonlarını tekrar kontrol edin.
- Modül kodlarının doğru yüklendiğinden emin olun.
- Gerekirse modül ile ilgili dökümandaki devre şemalarını gözden geçirin.

### LED veya Buton Tepki Vermiyor
- Güç kaynağını kontrol edin.
- Kabloların sağlam ve doğru bağlandığını kontrol edin.
- Arduino seri monitöründe hata mesajlarını kontrol edin.

---

## 4. Satış ve Sipariş Sorunları

### Siparişim Gelmedi veya Hasarlı Geldi
- Lütfen **[Satın Alma Koşulları](buying-conditions.md)** sayfamızı inceleyin.
- Destek için iletişim sayfasından bizimle irtibata geçin.

### Ödeme Sorunları
- Kredi kartı veya ödeme platformunda işlem sorunları olabilir.
- Bankanızla veya ödeme sağlayıcınızla iletişim kurunuz.

---

## 5. Diğer Sorunlar

### Yazılım ile İlgili Sorunlar
- Github repository’mizdeki **[Katkıda Bulun](contributing.md)** sayfasını inceleyerek hata bildirebilir veya destek alabilirsiniz.

### Belgelerde Eksik veya Hatalı Bilgi
- Lütfen bizimle iletişime geçin, belgeleri güncellemek için çalışıyoruz.

---

## Yardım ve Destek

Eğer yukarıdaki çözümler sorununuzu çözmediyse, bizimle **[İletişim](contact.md)** sayfası üzerinden irtibata geçebilirsiniz. Size yardımcı olmaktan memnuniyet duyarız!

---

*Talk to Defuse Proje Ekibi*
