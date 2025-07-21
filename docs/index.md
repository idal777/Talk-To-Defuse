---
title: Talk to Defuse
theme: jekyll-theme-midnight
---

# Talk To Defuse

## Nedir?

Talk to Defuse, popüler "Keep Talking and Nobody Explodes" oyununa fiziksel bir gerçeklik kazandıran açık kaynaklı bir donanım projesidir. Oyuncular bir "bomba" üzerinde çalışırken, diğer oyuncular da ona uzaktan yönergeler vererek bombayı etkisiz hale getirmeye çalışır. Amaç, hem eğitici hem de eğlenceli bir takım çalışması deneyimi sunmaktır.

## Nasıl Çalışır?

Sistem, birbirinden bağımsız çalışan fiziksel modüllerden oluşur. Bu modüller Arduino tabanlı mikrodenetleyicilerle kontrol edilir ve birbirleriyle I2C protokolü üzerinden haberleşir. Ana modül, oyunun yönetimini ve zamanlamasını sağlar. Her modül kendi içinde hata üretebilir ve oyuncular bu hataları çözmek zorundadır.

## Modül Sistemi

- **Tak-Çalıştır:** Modüller kolayca eklenip çıkarılabilir.
- **Genişletilebilir:** Herkes yeni bir modül tasarlayıp projeye katkı sunabilir.
- **Açık Standart:** Donanım ve yazılım arayüzleri açık bir şekilde belgelenmiştir.

## Teknik Altyapı

- **Donanım:** Arduino Nano/Uno, I2C haberleşme, LED, buton, ekran vb.
- **Yazılım:** Arduino IDE + Kütüphaneler
- **Belgeler:** Tüm teknik dökümanlar GitHub’dadır.
- **Ar-Ge:** Breadboard, ardından PCB tasarımı yapılır.

## Vizyon

Talk to Defuse, açık kaynak fiziksel oyun projeleri arasında bir referans noktası olmayı hedefler.
