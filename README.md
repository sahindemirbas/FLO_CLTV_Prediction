## FLO CLTV Tahmin Projesi
Bu proje, FLO müşterileri için BG/NBD ve Gamma-Gamma modellerini kullanarak Müşteri Yaşam Boyu Değerini (CLTV) tahmin etmeyi amaçlamaktadır. Veri seti, 2020-2021 yılları arasındaki müşteri işlemleri ve alışveriş davranışlarını içermektedir. Proje, veri temizleme, aykırı değerlerin işlenmesi, model kurma ve tahmin edilen CLTV'ye göre müşterilerin segmentlere ayrılmasını içerir.

# Proje Adımları

Veri Hazırlığı:
Veriyi bir CSV dosyasından yükleyin.
Tarih sütunlarını datetime formatına çevirin.
Eksik ve sıfır değerleri kontrol edin ve kaldırın.
Belirli sütunlar için aykırı değerleri işleyin.
Toplam sipariş ve toplam değer için yeni değişkenler oluşturun.
CLTV Veri Yapısının Oluşturulması:
Recency ve tenure hesaplamalarını haftalık terimlerle yapın.
Frequency ve monetary değerleri hesaplayın.
Bir CLTV dataframe'i oluşturun.
Model Kurma ve CLTV Hesaplama:
BG/NBD modelini fit edin.
3 ve 6 ay için beklenen satışları tahmin edin.
Gamma-Gamma modelini fit edin.
Ortalama değeri tahmin edin ve 6 aylık CLTV'yi hesaplayın.
Müşteri Segmentasyonu:
Müşterileri tahmin edilen CLTV değerlerine göre dört gruba ayırın.
İlk iki segment için uygulanabilir aksiyon önerileri sağlayın.

# Projenin Çalıştırılması

Depoyu Klonlayın:
git clone https://github.com/kullaniciadi/FLO_CLTV_Tahmin_Projesi.git
cd FLO_CLTV_Tahmin_Projesi

Bağımlılıkları Yükleyin:
pandas ve lifetimes kütüphanelerine sahip olmanız gerekmektedir. Bunları pip kullanarak yükleyebilirsiniz:


pip install pandas lifetimes

Jupyter Notebook'u Çalıştırın:
Sağlanan Jupyter Notebook'u (FLO_CLTV_Prediction.ipynb) açarak adım adım süreci takip edebilir ve hücreleri çalıştırabilirsiniz.
Sonuçları Görüntüleyin:
Notebook, veri hazırlığından model kurma ve segmentasyona kadar tüm süreci yönlendirecektir.

# Notebook'taki Detaylı Adımlar

Veri Yükleme ve Temizleme:
CSV dosyasını okuyun ve tarih sütunlarını dönüştürün.
Eksik ve sıfır değerleri kontrol edin ve kaldırın.
Aykırı değerleri işleyin.
Metriği Hesaplama:
Toplam sipariş ve toplam değer gibi yeni özellikler oluşturun.
Recency, frequency ve monetary değerleri hesaplayın.
Model Kurma:
BG/NBD modelini fit edin ve işlem sayısını tahmin edin.
Gamma-Gamma modelini fit edin ve ortalama monetary değeri tahmin edin.
6 aylık CLTV'yi hesaplayın.
Müşteri Segmentasyonu:
Müşterileri CLTV'ye göre dört gruba ayırın.
En yüksek CLTV değerine sahip 20 müşteriyi gözlemleyin.
İlk iki segment için aksiyon önerileri sağlayın.

# Örnek Çıktılar

Notebook, en yüksek CLTV değerine sahip ilk 20 müşteriyi ve en üst segmentler için aksiyon önerilerini gösterecektir.

# Grup A ve B için Öneriler

Grup A:

Sadakat Programları: En değerli müşterilerinize özel sadakat programları sunun. Özel indirimler, erken erişim fırsatları ve ücretsiz kargo gibi avantajlar sağlayarak sadakati artırın.
Kişiselleştirilmiş Pazarlama: Müşterilerin önceki alışveriş alışkanlıklarına dayanarak kişiselleştirilmiş pazarlama kampanyaları oluşturun. Onlara özel ürün önerileri ve kampanyalar sunarak müşteri memnuniyetini artırın.
Grup B:

Çapraz Satış Stratejileri: Bu gruptaki müşterilere ilgili ürünleri sunarak çapraz satış fırsatlarını değerlendirin. Örneğin, bir ayakkabı satın alan müşteriye uyumlu çorap veya bakım ürünleri önerin.
Müşteri Geri Bildirimi: Müşteri geri bildirimlerini toplamak ve değerlendirmek için anketler düzenleyin. Müşteri memnuniyetini artırmak için geri bildirimlere dayalı iyileştirmeler yapın.
 
