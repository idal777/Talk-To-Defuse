# 🔘 Buton Modülü

Bu modül, oyuncunun doğru zamanda butona basmasını gerektirir. Renkli LED’ler ve buton kullanılarak yapılır.

## 💡 Amaç

Oyuncu, belirli bir süre içinde butona basmalı veya basmamalıdır. Kurallar, kılavuza göre değişir.

## 🔌 Donanım Gereksinimleri

- 1x Buton
- 1x LED (renkli)
- 1x 220 ohm direnç
- Jumper kablolar
- Arduino Uno

## 🔧 Bağlantı Şeması

- LED: Dijital pin 7'ye, direnci 220Ω olacak şekilde bağlanır.
- Buton: Dijital pin 2'ye bağlanır. Pull-down direnci ile bağlanmalıdır.

## 🧠 Oyun Mantığı

1. LED yanıp sönmeye başlar.
2. Oyuncu LED yeşil olduğunda butona basarsa başarılı olur.
3. Yanlış zamanda basarsa modül patlar.

## 💻 Arduino Kodu (Örnek)

```cpp
const int buttonPin = 2;
const int ledPin = 7;

void setup() {
  pinMode(buttonPin, INPUT);
  pinMode(ledPin, OUTPUT);
  Serial.begin(9600);
}

void loop() {
  digitalWrite(ledPin, HIGH);
  delay(1000);
  digitalWrite(ledPin, LOW);
  delay(1000);

  if (digitalRead(buttonPin) == HIGH) {
    Serial.println("Butona basıldı!");
    // Kontrol mekanizması buraya
  }
}
