# KrediKartDolandiriciligindaAnomaliTespiti
Proje Amacı:

Bu proje, kredi kartı dolandırıcılığı tespiti için makine öğrenmesi modelleri geliştirmeyi ve Kafka ile gerçek zamanlı veri işleme altyapısı kurarak anomali tespiti yapmayı amaçlamaktadır.

Adımlar:


Veri Seti ve Ön İşleme:

Kaggle'dan alınan kredi kartı dolandırıcılığı veri seti üzerinde analiz yapıldı.

Eksik veri kontrolü ve gereksiz sütunların çıkarılması.

'Amount' sütununda logaritmik dönüşüm yapıldı.

Veriler MinMaxScaler ile ölçeklendirildi.

Veri dengesizliği için random oversampling uygulandı.

Veri Görselleştirme:


Korelasyon analizi ve ısı haritası oluşturuldu.

Histogramlar ve scatter plot’lar ile verinin dağılımı incelendi.

Class sütunundaki dengesizlik görselleştirildi.

Makine Öğrenmesi Modelleri:

Logistic Regression, Random Forest ve Decision Tree modelleri kullanıldı.

Model performansı, doğruluk, precision, recall ve F1 skoru ile değerlendirildi.

Random Forest en yüksek doğruluk oranını sağladı.


Kafka Yapılandırması:

Apache Kafka kullanılarak verilerin anlık olarak iletilmesi sağlandı.

Kafka Producer yapılandırması ile saniyede 833 veri gönderildi.

Veri üretimi için random veri kümesi oluşturuldu ve Kafka topic’ine gönderildi.

Sonuçlar:

Veri ön işleme ve modelleme adımları, sahtekarlık tespitinde yüksek başarı sağladı.

Kafka ile gerçek zamanlı veri işleme altyapısı etkin bir şekilde çalıştı.

Kullanılan Teknolojiler:

Python (Pandas, NumPy, Scikit-learn, Seaborn)

Apache Kafka

Makine öğrenmesi modelleri: Logistic Regression, Random Forest, Decision Tree
 
