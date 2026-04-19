# ml-covid19-hasta-tahmin
# ml-covid19-hasta-tahmini

## Proje Açıklaması

Bu projede COVID-19 belirtileri ve sağlık verileri kullanılarak bir kişinin COVID-19 pozitif veya negatif olma durumu tahmin edilmiştir. Projede makine öğrenmesi yöntemleri kullanılmış ve birden fazla algoritma karşılaştırılmıştır.

Amaç, veri analizi sürecini uçtan uca uygulamak ve hangi modelin daha başarılı sonuç verdiğini incelemektir.

---

## Kullanılan Veri Seti

Veri seti Kaggle platformundan alınmıştır.

Örnek veri seti içeriği:

* Fever
* Cough
* Breathing Problem
* Tiredness
* Sore Throat
* Age
* Gender
* Other Symptoms
* COVID Result

Kaggle üzerinden benzer veri setleri kullanılabilir.

Örnek arama:

COVID-19 Symptoms Dataset

---

## Kullanılan Kütüphaneler

Projede aşağıdaki Python kütüphaneleri kullanılmıştır:

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn

---

## Veri Ön İşleme Adımları

Model eğitiminden önce veri temizleme ve hazırlama işlemleri yapılmıştır.

### Yapılan işlemler:

1. CSV dosyası okunmuştur.
2. Eksik veriler kontrol edilmiştir.
3. Eksik satırlar silinmiştir.
4. Kategorik veriler LabelEncoder ile sayısal hale getirilmiştir.
5. Giriş ve hedef değişkenler ayrılmıştır.
6. Eğitim ve test verisi olarak bölünmüştür.
7. StandardScaler ile veriler ölçeklendirilmiştir.

---

## Keşifsel Veri Analizi (EDA)

Veri seti üzerinde aşağıdaki analizler yapılmıştır:

* İlk 5 satır görüntüleme
* Veri boyutu kontrolü
* Sütun isimleri inceleme
* İstatistiksel özet
* Eksik veri kontrolü

---

## Oluşturulan Grafikler

Projede veri analizi ve model karşılaştırması için grafikler kullanılmıştır.

### Kullanılan Grafikler:

1. COVID sonuç dağılım grafiği
2. Korelasyon ısı haritası
3. Tüm değişken histogramları
4. Boxplot ile aykırı değer analizi
5. Model başarı oranı bar grafiği
6. Özellik önem sıralaması grafiği
7. Confusion Matrix ısı haritaları

---

## Kullanılan Makine Öğrenmesi Algoritmaları

Bu projede 3 farklı model kullanılmıştır:

### 1. Logistic Regression

İkili sınıflandırma problemlerinde kullanılan temel bir algoritmadır.

### 2. Random Forest

Birden fazla karar ağacının birleşiminden oluşur. Genellikle yüksek başarı verir.

### 3. K-Nearest Neighbors (KNN)

En yakın komşulara göre sınıflandırma yapan algoritmadır.

---

## Model Performans Değerlendirme

Her model için aşağıdaki ölçümler yapılmıştır:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

---

## Model Karşılaştırma

Kod çalıştırıldığında 3 modelin başarı oranları karşılaştırılır ve en başarılı model ekrana yazdırılır.

Örnek:

* Logistic Regression: 0.91
* Random Forest: 0.95
* KNN: 0.89

En başarılı model: Random Forest

---

## Dosya Yapısı

```bash
ml-covid19-hasta-tahmini/
│── covid.csv
│── covid_model.py
│── README.md
```

---

## Projeyi Çalıştırma

### Gerekli Kütüphaneleri Kur:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Programı Çalıştır:

```bash
python covid_model.py
```

---

## Sonuç ve Yorum

Bu projede COVID-19 verileri üzerinde farklı makine öğrenmesi algoritmaları uygulanmıştır. Sonuçlara göre Random Forest modeli genellikle daha başarılı performans göstermektedir.

Grafikler sayesinde veri daha iyi analiz edilmiş ve modeller karşılaştırılmıştır.

---

## Geliştirme Fikirleri

Projeye ileride şu özellikler eklenebilir:

* Daha büyük veri seti kullanımı
* XGBoost modeli ekleme
* Web arayüzü oluşturma
* Gerçek zamanlı tahmin sistemi
* Kullanıcıdan veri alarak canlı tahmin yapma

---

## Hazırlayan

Ad Soyad: şevval özer
Ders: Makine Öğrenmesi
Teslim Tarihi: 20.04.2026
