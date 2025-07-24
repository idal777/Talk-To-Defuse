# Talk To Defuse

## Nedir?

Talk to Defuse, popüler *"Keep Talking and Nobody Explodes"* oyununa fiziksel gerçeklik kazandıran açık kaynaklı bir donanım projesidir.  
Oyuncular bir "bomba" üzerinde çalışırken, diğer oyuncular da ona uzaktan yönergeler vererek bombayı etkisiz hale getirmeye çalışır. Amaç, hem eğitici hem de eğlenceli bir takım çalışması deneyimi sunmaktır.

## Nasıl Çalışır?

Sistem, birbirinden bağımsız çalışan fiziksel modüllerden oluşur. Bu modüller Arduino tabanlı mikrodenetleyicilerle kontrol edilir ve I2C protokolü üzerinden birbirleriyle haberleşir. Ana modül, oyunun yönetimini ve zamanlamasını sağlar. Her modül kendi içinde hata üretebilir ve oyuncular bu hataları çözmek zorundadır.

Oyun süreci şu adımlarla ilerler:

1. **Başlangıç:** Ana modül, oyun süresini ve modül sayısını belirler.  
2. **Modüllerin Aktifleşmesi:** Her modül kendi özel göreviyle başlar (örneğin LED dizisi, şifre çözme, switch kombosu).  
3. **İletişim:** Modüller, I2C protokolü ile ana modüle bilgi gönderir ve komut alır.  
4. **Hata ve Zorluklar:** Modüller rastgele veya önceden belirlenmiş hatalar üretir; oyuncular bunları çözmek zorundadır.  
5. **İşbirliği:** Oyuncular modüller üzerinde birlikte çalışarak hataları düzeltir ve bombayı etkisiz hale getirmeye çalışır.  
6. **Başarı / Başarısızlık:** Süre dolduğunda bomba etkisizleşmişse oyuncular kazanır, aksi takdirde oyun sona erer.

## Modül Sistemi

Modüller şu temel özelliklere sahiptir:

- **Tak-Çalıştır:** Modüller kolayca eklenip çıkarılabilir.  
- **Genişletilebilir:** Herkes yeni modül tasarlayıp projeye katkı sunabilir.  
- **Açık Standart:** Donanım ve yazılım arayüzleri açıkça belgelenmiştir.

## Teknik Altyapı

- **Donanım:** Arduino Nano/Uno, I2C haberleşme, LED, buton, ekran vb.  
- **Yazılım:** Arduino IDE ve özel kütüphanelerle geliştirilmiş bağımsız firmware’ler.  
- **Belgeler:** Tüm teknik dokümanlar GitHub’da mevcuttur.  
- **Ar-Ge:** Modüller önce breadboard veya pertinaks üzerinde test edilir, ardından PCB tasarımı yapılır.

## Vizyon

Talk to Defuse, açık kaynaklı fiziksel oyun projeleri arasında bir referans noktası olmayı hedefler. Eğlenceli ve öğretici bir deneyim sunarak maker, öğrenci ve oyun sever topluluklarını bir araya getirmeyi amaçlar.

---

## Daha Fazlası

- [Modüller](moduller.md)  
- [Parçalar](parcalar.md)  
- [3D Modeller](3dmodeller.md)
