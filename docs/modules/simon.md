# Simon Says Modülü

## Genel Tanıtım

Simon Says, klasik renk ve ses tabanlı hafıza oyunudur.  
Oyuncu, LED ışıkların gösterdiği renk sırasını tekrarlamalıdır.  
Her başarılı denemede sıra bir renk uzar ve zorluk artar.

## Donanım

- **5x5 LED Matris** (25 LED)
- **Buzzer** ses çıkışı için
- 4 adet renkli buton (Renkler: Kırmızı, Yeşil, Mavi, Sarı)
- Arduino UNO veya muadili

## Bağlantılar

- LED matrisi, Arduino’nun dijital pinlerine bağlanır (ör. 8,9,10…).
- Butonlar ve buzzer ilgili pinlere bağlanır.
- Butonlar pull-down dirençleri ile bağlanmalıdır.
- Buzzer PWM çıkışına bağlanır.

## Oyun Mantığı

1. Arduino rastgele bir renk dizisi oluşturur.
2. LED matris üzerinde renkli ışıklar yanar.
3. Oyuncu bu diziyi butonlara basarak tekrar eder.
4. Doğruysa sıra bir renk artar ve tekrar edilir.
5. Hatalıysa oyun başa döner.

## Örnek Devre Bağlantısı
Arduino UNO
| | | |
LED Matris Pins Buton Pins Buzzer Pin GND

## İpuçları

-LED matrisin doğru sürüldüğünden emin olun.
-Butonların temiz sinyal verdiğinden emin olun.
-Sesli uyarılar oyuncuya geri bildirim sağlar.


