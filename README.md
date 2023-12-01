Veri Yüklemesi ve İnceleme:

Kaggle'dan alınan "Dog Breed Identification" veri seti kullanılmıştır.
Etiketler ve örnek bir gönderi için örnek bir CSV dosyası yüklenmiştir.

Veri Temizleme ve İşleme:

Veri seti üzerinde çeşitli işlemler yapılmıştır.
Sınıf sayısı 100'den fazla olanları filtrelemek için bir eşik belirlenmiştir.
Veri seti temizlenerek, belirlenen sınıflara ait örnekler seçilmiştir.

Veri Görselleştirmesi:

Sınıf sayıları görselleştirilmiş ve sınıfların dağılımı incelenmiştir.
Örnek görsellerin boyutları değiştirilerek görselleştirme yapılmıştır.

Veri Hazırlığı:

Etiketler üzerinde Label Encoding ve One-Hot Encoding işlemleri yapılmıştır.
Veri seti eğitim ve test olarak ayrılmıştır.
Eğitim verisi üzerinde görüntü artırma teknikleri uygulanmıştır.

Model Oluşturma:

Önceden eğitilmiş modellerden (EfficientNetB4, Xception, ResNet50) özellik çıkarıcılar elde edilmiştir.
Bu özellik çıkarıcılar birleştirilerek final özellik seti oluşturulmuştur.
Bu özellik seti üzerinde bir Dense layer ile 120 sınıfa karşılık gelen softmax aktivasyonu kullanılarak model oluşturulmuştur.

Eğitim ve Değerlendirme:

Model, eğitim verisi üzerinde belirli sayıda epoch için eğitilmiştir.
Modelin eğitim süreci görselleştirilmiştir.
Modelin en iyi performans gösterdiği aşamada kaydedilmiştir.

Modelin Değerlendirilmesi:

Eğitilen model, test verisi üzerinde değerlendirilmiş ve tahminler yapılmıştır.
Confusion matrix ve sınıflar arası karşılaştırmalar görselleştirilmiştir.

Sonuçlar ve Analiz:

Modelin doğruluğu ve kayıp değerleri değerlendirilmiş ve görselleştirilmiştir.
Rastgele seçilen 20 örneğin tahminleri ve gerçek etiketleri karşılaştırılmıştır.

Modelin Yapısının Görselleştirilmesi:

Modelin katmanları ve bağlantıları, keras.utils.plot_model ile görselleştirilmiştir.
