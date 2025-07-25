# Kablolar (Cables) Modülü

## Genel Bakış

Kablolar modülü, oyuncunun dikkat ve mantık becerisini sınayan bir modüldür.  
Oyuncu, birden fazla renk ve türdeki kablo arasından doğru kabloyu seçip kesmeli veya bağlantıyı sağlamalıdır.  
Yanlış kablo kesilmesi veya bağlanması hata ile sonuçlanır.

## Kullanılan Malzemeler

- Farklı renklerde ve kalınlıklarda kablolar (örneğin kırmızı, siyah, sarı)  
- Bağlantı noktaları ve konnektörler  
- Kesme butonu veya mekanizması (Opsiyonel)  
- Arduino UNO (veya uyumlu)  
- Butonlar (kablo kesme onayı için)  
- LED’ler (başarı veya hata göstergesi için)  

## Devre Bağlantıları

| Bileşen         | Arduino Bağlantısı    |
|-----------------|-----------------------|
| Kablo Kesme Butonu | D2                   |
| Kablo Seçim Butonları | D3, D4, D5 (opsiyonel) |
| Başarı LED      | D9                    |
| Hata LED        | D10                   |

Not: Kablo kesme işlemi buton ile tetiklenir. Doğru kablo kesildiğinde başarı LED’i yanar, yanlış kesilirse hata LED’i ve alarm aktif olur.

## Çalışma Mantığı

1. Modül üzerinde birden fazla kablo vardır.  
2. Arduino, doğru kabloyu önceden belirler (örneğin kırmızı kablo).  
3. Oyuncu doğru kabloyu bulup butona basarak kesmelidir.  
4. Doğru kablo kesildiğinde modül başarılı olur ve ilerler.  
5. Yanlış kablo kesildiğinde modül hata verir ve alarm aktif olur.

## Kullanıcı İpuçları

- Kabloların renklerine ve sırasına dikkat edin.  
- Bazı modlarda, kabloların numaraları veya renk kodları ipucu verebilir.  
- Acele etmeyin, dikkatli ve mantıklı seçim yapın.

## Geliştirme Önerileri

- Kablo sayısını artırarak zorluk seviyesi yükseltilebilir.  
- Kabloların bağlanması veya kesilmesi için farklı buton kombinasyonları eklenebilir.  
- Zaman sınırlaması veya yanlış kesim sayısı sınırı getirilebilir.
