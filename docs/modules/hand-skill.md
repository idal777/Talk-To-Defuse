# El Becerisi (Hand Skill) Modülü

## 🧩 Modül Tanımı

Bu modül, oyuncunun fiziksel el becerisini ve dikkatini test eden bir sistemdir. Oyuncunun, bir metal halkayı eğimli bir spiral tel boyunca geçirmesi gerekir. Halkayla tel temas ettiğinde hata algılanır ve sistem uyarı verir. Süreç dikkat ve el-göz koordinasyonu gerektirir.

## ⚙️ Kullanılan Malzemeler

- 1 adet spiral şekilde bükülmüş sert iletken tel (örneğin alüminyum ya da bakır)
- 1 adet metal halka (oyuncunun elinde tutacağı)
- 1 adet buzzer (temas uyarısı için)
- 1 adet LED (uyarı için opsiyonel)
- Arduino UNO (veya benzeri)
- 10K Ohm direnç (pull-down için)
- Jumper kablolar
- Breadboard (veya lehimlenmiş devre)

## 🔌 Devre Bağlantısı

| Bileşen         | Arduino Bağlantısı      |
|------------------|-------------------------|
| Spiral Tel       | GND                     |
| Metal Halka      | D2 (dijital giriş pini) |
| Buzzer           | D9                      |
| LED (opsiyonel)  | D10                     |

Not: Metal halka ile spiral tel temas ettiğinde, D2 pinine düşük sinyal gider ve bu da hata olarak algılanır.

## 🎮 Oyun Mekaniği

- Oyuncu, modülün başından başlayarak halkayı spiral tel boyunca geçirir.
- Tel ile temas durumunda LED ve buzzer aktif hale gelir.
- 3 temas hakkı olabilir veya temas süresi ölçülerek oyuncunun skoru belirlenebilir.

## 🛠️ Zorluk Ayarı

- Spiral telin eğimi ve uzunluğu artırılarak zorluk seviyesi değiştirilebilir.
- Daha dar geçişler veya zaman kısıtı ile daha zor hale getirilebilir.

## 📷 Görsel (Örnek)

*3D modeli veya gerçek fotoğraf burada yer alabilir.*
