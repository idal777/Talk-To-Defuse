# Switch Modülü

## Genel Bakış

Switch Modülü, oyuncunun belirli bir sırada düğmelere basmasını gerektiren bir oyundur.  
Bu modül, hızlı refleksler ve dikkat gerektirir. Yanlış tuşa basılması durumunda modül alarm verir ve sıfırlanır.

## Devre Bağlantıları

- Modülde **4 adet buton (switch)** kullanılır.
- Her buton Arduino’nun dijital pinlerinden (örneğin D2, D3, D4, D5) okunur.
- Butonlar pull-down dirençleri ile bağlanmalıdır, böylece basılmadığında giriş pini LOW olur.
- Butonlara basıldığında pin HIGH olur.

## Çalışma Mantığı

- Arduino, önceden tanımlanmış bir tuş sırasını hafızasında tutar.
- Oyuncu butonlara bu sırayla basmalıdır.
- Doğru sıralama takip edildiği sürece ilerlenir ve sıra uzar.
- Yanlış basışta modül hata verir ve oyuncu tekrar başlamak zorunda kalır.

## Örnek Devre Şeması

Arduino UNO
  |          |           |          |
 D2 (Button1) D3 (Button2) D4 (Button3) D5 (Button4)
   |          |           |          |
  Butonlar to GND via 10kΩ direnç

## Kullanıcı İpuçları

-Butonlara hızlı ve doğru basmaya çalışın.
-Hatalı basışlarda sesli uyarı alınabilir.
-Oyun zorlaştıkça sıra daha uzun olacaktır.