---
title: Ana Modül
---

# Ana Modül

> ℹ️ Diğer tüm modüller ile iletişim kuran, oyunun başlamasını, bitmesini belirleyen, her oyunda bulunması zorunlu olan temel modüldür. Herhangi bir bulmaca içermez.

## Elektronik Detayları

### Malzemeler

1. **Durum Göstergesi:** İçinde 3 adet RGB LED bulunur. Duruma göre renk değiştirerek bildirim verir.  
2. **Kalan Can Göstergesi:** 3 adet kırmızı LED içerir. Her bir can kaybedildiğinde birisi söner.  
3. **Güç Anahtarı:** Sistemi açıp kapatmak için anahtar.  
4. **Süresayar:** Bombanın imha edilmesi için kalan süreyi gösterir.  
5. **Ekran:** Başta zorluk seçimi gibi işlevler için, sonra seri numarası gibi bilgiler için kullanılır.  
6. **Buton:** Oyunu başlatmak, zorluk seçmek, sıfırlamak gibi işlevleri üstlenir.  

### Devre Şeması

> ⚠️ Görseller GitHub’a henüz yüklenmedi. Yüklediğinde burada görünecekler:

## Yazılım Detayları

### Genel Mimari

Kod dili: **Arduino (C++)**  
Ana kontrol: `main.ino` dosyasında yapılır.  
I2C kullanılır: Ana modül master’dır, diğerleri slave.

### Ana Modül Görevleri

- Oyun başlatma ve sıfırlama
- Zorluk seviyesi seçimi
- Süre başlatma ve gösterme
- Seri numarası üretimi
- Can takibi
- Oyun bitiş senaryoları

### Modül Haberleşme Sistemi

- **Protokol:** I2C  
- **Adresleme:** Her modül sabit I2C adresine sahip  
- **Komut sistemi:** Başlat, çözüm kontrolü, hata bildirimi vs.

### Zaman Yönetimi

- `millis()` fonksiyonu ile süre tutulur  
- TM1637 ekranına kalan süre gösterilir  
- Süre biterse oyun sona erer  

### Oyun Akışı

1. Açılış ekranı
2. Zorluk seçimi
3. Geri sayım başlar
4. Modül kontrolleri
5. Can/süreye göre kazanma veya kaybetme




