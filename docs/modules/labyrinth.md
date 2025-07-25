# Labirent Modülü

## Tanım

Labirent modülü, oyuncunun belirli bir yoldan geçerek çıkışı bulmasını gerektirir.  
Modül üzerinde bir 5x5 LED matrisi veya joystick ile kontrol edilen bir labirent olabilir.

## Donanım

- 5x5 LED Matris
- Joystick veya yön tuşları
- Arduino mikrodenetleyici

## Bağlantılar

- LED matrisin satır ve sütun pinleri Arduino’ya bağlanır.
- Joystick X ve Y pinleri Arduino analog girişlerine bağlanır.
- Buton joystick üzerinde varsa dijital pine bağlanır.

## Oyun Mantığı

- Arduino, labirent haritasını tutar.
- Oyuncu joystick ile karakteri hareket ettirir.
- Amaç başlangıçtan çıkış noktasına ulaşmaktır.
- Yanlış hareketler veya engellere temas etmek hataya yol açar.

## Örnek Devre Şeması 

Arduino UNO
  |         |          |   
LED Matris Joystick X,Y  GND

## İpuçları
-Joystick kalibrasyonuna dikkat edin.
-Labirent haritasını kolayca değiştirilebilir yapın.
-Oyuncunun yönlendirmesini görsel olarak net yapın.


