# Titanic ve Breast Cancer Veri Setleri ile Gelişmiş Fonksiyonel Keşifçi Veri Analizi

Bu projede Titanic veri seti üzerinde kategorik ve sayısal değişkenlerin analizlerini yaparak, ilgili verileri fonksiyonlaştırdım. Ayrıca, Breast Cancer veri seti üzerinde korelasyon analizi gerçekleştirdim. Amaç, veri setlerinin temel özelliklerini daha iyi anlayarak, veri analizi sürecini otomatikleştirebilmektir.

### Kurulum

1. Depoyu klonlayın
2. Gerekli kütüphaneleri kurun
3. Korelasyon analizinde kullanılan dataseti (https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data) projenize yükleyin.
4. Analizleri çalıştırın


## Proje İçeriği

### Genel Veri İncelemesi:

- Titanic veri seti ile başlanarak, veri yapısı ve genel istatistiksel analizler yapıldı.
- `check_df` fonksiyonu ile veri setinin temel özellikleri (satır/sütun sayısı, veri tipleri, eksik değerler vb.) gözlemlendi.

### Kategorik Değişken Analizi:

- Titanic veri setindeki kategorik değişkenler (`embark_town`, `sex`, `class`, vb.) üzerinde frekans ve oran analizleri yapıldı.
- Fonksiyonlar kullanılarak kategorik değişkenlerin incelenmesi ve görselleştirilmesi sağlandı.

### Sayısal Değişken Analizi:

- Titanic veri setindeki sayısal değişkenler (`age`, `fare`) için özet istatistikler ve histogramlar oluşturuldu.
- `num_summary` fonksiyonu ile sayısal değişkenlerin temel istatistikleri elde edildi.

### Hedef Değişken İlişkisi Analizi:

- Titanic veri setindeki "survived" (hayatta kalma) hedef değişkeni ile kategorik ve sayısal değişkenler arasındaki ilişkiler incelendi.
- `target_summary_with_cat` ve `target_summary_with_num` fonksiyonları kullanılarak hedef değişken ile olan bağlantılar analiz edildi.

### Korelasyon Analizi:

- Breast Cancer veri seti üzerinde korelasyon analizi yapıldı.
- Değişkenler arasındaki yüksek korelasyonlar (0.90 üzeri) tespit edilerek bu değişkenler dışarıda bırakıldı.
- Korelasyon ısı haritası ile değişkenler arasındaki ilişkiler görselleştirildi.

## Fonksiyonlar

- `check_df()`: Veri setinin index, boyut, istatistik gibi temel özelliklerini özetleyen fonksiyon.
- `cat_summary()`: Kategorik değişkenlerin özetini ve dağılımını veren fonksiyon.
- `num_summary()`: Sayısal değişkenlerin özetini ve dağılımını veren fonksiyon.
- `grab_col_names()`: Veri setindeki kategorik, sayısal ve kardinal değişkenlerin isimlerini sınıflandırarak döndüren fonksiyon. Bu fonksiyonun işlevi docstringde belirtildi.
- `target_summary_with_cat()`: Hedef değişken ile kategorik değişkenler arasındaki ilişkiyi gösteren fonksiyon.
- `target_summary_with_num()`: Hedef değişken ile sayısal değişkenler arasındaki ilişkiyi gösteren fonksiyon.
- `high_correlated_cols()`: Korelasyonu yüksek olan değişkenleri tespit eden fonksiyon.

## Testleri Çalıştırma

Analizi çalıştırmak için Python betiklerini çalıştırın ve çıktı dosyalarında sonuçları kontrol edin.

### Adım Adım Testler

Her fonksiyonun çalıştığını test etmek için Titanic ve Breast Cancer veri setleri üzerinde analizleri çalıştırın.


## Kullanılan Teknolojiler

* [Pandas](https://pandas.pydata.org/) - Veri manipülasyonu ve analizi
* [Seaborn](https://seaborn.pydata.org/) - Görselleştirme
* [Matplotlib](https://matplotlib.org/) - Grafikler ve görselleştirmeler

## Yazar

* **Ali Cem DURAN** - (https://github.com/ali-cemputer)

