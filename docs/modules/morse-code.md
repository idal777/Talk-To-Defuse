# Mors Kodu Modülü

## Genel Bakış

Mors Kodu Modülü, kullanıcıya LED ile yanıp sönen bir kod dizisi gösterir.  
Oyuncunun, bu kodu çözerek doğru kelimeyi veya harfi bulması gerekir.  
Kodlar uluslararası Mors alfabesine göre verilir ve modül, çözüm tamamlanana kadar çalışmaya devam eder.

## Donanım Bileşenleri

- 1 adet LED (mors kodu için yanıp söner)
- 1 adet buton (kullanıcı girişi için)
- 1 adet buzzer (sesli geri bildirim için, opsiyonel)
- Arduino UNO (veya uyumlu bir kart)

## Devre Bağlantıları

- LED → D2  
- Buton → D3 (pull-down direnç ile bağlanmalı)  
- Buzzer (opsiyonel) → D4  
- GND ve 5V bağlantıları yapılmalı  
- LED için 220Ω direnç önerilir

## Çalışma Mantığı

1. LED, Mors koduyla bir harf veya kelimeyi gösterir.  
   - Kısa yanıp sönme: **`.` (dot)**  
   - Uzun yanıp sönme: **`-` (dash)**  
   - Harfler arasında kısa duraklama  
2. Oyuncu, verilen Mors kodunu çözmeye çalışır.  
3. Doğru giriş yapılırsa başarı sesi verilir, yanlış girişte hata sesi ve tekrar.

## Örnek Mors Kodu

**LED yanıp sönme dizisi:**

- Kısa (.) → 250ms
- Uzun (-) → 750ms
- Noktalar arası boşluk: 250ms
- Harfler arası boşluk: 1000ms

Örnek: `.-` = A harfi

## Kullanıcı İpuçları

- LED’leri dikkatle takip edin; süre farklarını gözlemleyin.  
- Dilerseniz Mors tablosu yanında bulunsun.  
- Yanlış girişlerde tekrar başlamak gerekebilir.

## Geliştirme Fikirleri

- Mors kodunu kullanıcıdan buton ile girmesini sağlayabilirsiniz.  
- Sesli mors çıkışı için buzzer kullanın.  
- Daha uzun kelimeler ve zaman sınırlı çözüm modları ekleyin.

---

🛠️ *Modül, oyuncunun gözlem becerisi ve hafızasını test eder. Kod çözme yeteneğini artırmak için idealdir.*

