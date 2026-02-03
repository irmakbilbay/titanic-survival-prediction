# Titanic Hayatta Kalma Tahmini (Titanic Survival Prediction) 🚢

Bu proje, ünlü Titanic faciasındaki yolcu verilerini kullanarak, bir yolcunun hayatta kalıp kalamayacağını tahmin eden makine öğrenmesi modelleri geliştirmek amacıyla yapılmıştır.

## 🎯 Proje Özeti

Titanic veri seti üzerinde Sınıflandırma (Classification) algoritmaları kullanılarak "Hayatta Kaldı (1)" veya "Öldü (0)" tahmini yapılmıştır. Proje kapsamında eksik veriler istatistiksel yöntemlerle doldurulmuş ve Lojistik Regresyon ile Random Forest modelleri kıyaslanmıştır.

## 📊 İçerik ve Adımlar

### Veri Keşfi (EDA)
Cinsiyet ve bilet sınıfının hayatta kalma üzerindeki kritik etkisinin görselleştirilmesi.

### Veri Temizliği
- Age (Yaş) sütunundaki eksik verilerin yaş ortalaması ile doldurulması (Imputation)
- Gereksiz sütunların (deck, embark_town vb.) temizlenmesi

### Ön İşleme
Kategorik verilerin (Kadın/Erkek, Biniş Limanı) One-Hot Encoding ile sayısallaştırılması.

### Modelleme
- Lojistik Regresyon (Temel Model)
- Random Forest (Gelişmiş Model)

### Değerlendirme
Doğruluk (Accuracy) skorları, Hata Matrisi (Confusion Matrix) ve Özellik Önem Düzeyleri (Feature Importance).

## 🛠 Kullanılan Teknolojiler

- Python
- Pandas & NumPy: Veri manipülasyonu
- Seaborn & Matplotlib: Veri görselleştirme
- Scikit-learn: Lojistik Regresyon, Random Forest, Model Metrikleri

## 📈 Sonuçlar

İki farklı model eğitilmiş ve performansları karşılaştırılmıştır:

### Model Performansları

- Lojistik Regresyon: %79.3
- Random Forest: %81.5 🏆

### Analiz Bulguları
- Random Forest algoritması daha yüksek başarı göstermiştir.
- Özellik önemi analizinde, hayatta kalmayı en çok etkileyen faktörlerin Cinsiyet (Sex) ve Yaş (Age) olduğu görülmüştür  
  ("Kadınlar ve çocuklar önden" ilkesiyle uyumlu).

## 📂 Veri Kaynağı

Seaborn Library (Titanic Dataset)
