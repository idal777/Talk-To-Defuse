# Switch Modülü

Bu modül, kullanıcıdan belirli bir anahtar kombinasyonunu çözmesini ister.

## Amaç

Kullanıcı, verilen ipuçlarına göre doğru anahtarları açık ve kapalı konuma getirmelidir.

## Teknik Özellikler

- Kullanılan malzemeler: DIP switch, LED, dirençler, Arduino
- Doğru kombinasyon girildiğinde LED yanar.
- Yanlış kombinasyonlarda geri bildirim vermez veya farklı LED yanar.

## Oyun Kuralları

1. Kullanıcıya metin tabanlı bir ipucu gösterilir (örneğin: "İlk iki açık, diğerleri kapalı").
2. Kullanıcı fiziksel switch’leri çevirir.
3. Kod doğruysa sistem “Başarılı” mesajı verir ve diğer modüle geçilir.

## Geliştirme Notları

- Modül bağımsız çalışabilir şekilde tasarlanmalıdır.
- Farklı kombinasyonlar için parametreli hale getirilebilir.
