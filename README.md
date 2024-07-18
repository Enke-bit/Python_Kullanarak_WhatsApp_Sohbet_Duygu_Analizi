# Python Kullanarak WhatsApp Sohbet Duygu Analizi
Bu proje, WhatsApp sohbet geçmişini analiz ederek her bir mesajın duygusal tonunu belirlemeyi amaçlar. Proje, Python programlama dili ve NLTK (Natural Language Toolkit) kütüphanesi kullanılarak gerçekleştirilmiştir. İşte projenin adım adım özeti:

## Veri Okuma ve Hazırlama:

- WhatsApp sohbet geçmişi, belirli bir dosya yolundan okunur ve satır satır işlenir.
- Her bir mesajın tarih, saat, yazar ve içerik bilgileri ayrıştırılarak bir veri yapısına (liste) eklenir.
## Verilerin Pandas DataFrame'e Dönüştürülmesi:

- Ayrıştırılan veriler, Pandas DataFrame'e dönüştürülerek daha kolay işlenebilir hale getirilir.
- 'Date' sütunundaki tarihler, datetime formatına çevrilir.
- Eksik veriler DataFrame'den çıkarılır.
## Duygu Analizi:

- NLTK'nın VADER (Valence Aware Dictionary and sEntiment Reasoner) duygu analiz aracı kullanılarak her bir mesajın duygusal tonu analiz edilir.
- Analiz sonuçları, her bir mesaj için pozitif, negatif ve nötr skorlar olarak DataFrame'e eklenir.
## Sonuçların Görselleştirilmesi ve Yazdırılması:

- Analiz sonuçlarının özet bilgileri (DataFrame'in ilk beş satırı) ekrana yazdırılır.

## Sonuç
Bu proje, WhatsApp sohbet geçmişini analiz ederek her bir mesajın duygusal tonunu belirlemeyi başardı. Bu tür bir analiz, bireylerin veya grupların sohbetlerindeki genel duygu durumunu anlamak için kullanılabilir. Projede kullanılan yöntemler ve araçlar, diğer metin tabanlı duygu analizi projelerinde de uygulanabilir.

## Katkıda Bulunma
Bu projeye katkıda bulunmak isterseniz, lütfen bir pull request gönderin veya bir sorun açın. Her türlü katkı ve geri bildirim memnuniyetle karşılanacaktır!

## Lisans
Bu proje MIT Lisansı altında lisanslanmıştır. Daha fazla bilgi için LICENSE dosyasına bakabilirsiniz.
