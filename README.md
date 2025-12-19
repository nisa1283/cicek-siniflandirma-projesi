# 🌸 Çiçek Sınıflandırma Projesi (Flower Classification)

Bu proje, görüntü işleme ve derin öğrenme yöntemleri kullanılarak çiçek türlerinin otomatik olarak sınıflandırılmasını amaçlamaktadır.  
Proje kapsamında TensorFlow ve Keras kütüphaneleri kullanılarak Evrişimli Sinir Ağı (CNN) tabanlı bir model geliştirilmiştir.

---

## 📌 Projenin Amacı

Bu çalışmanın amacı, renkli çiçek görüntülerinden yola çıkarak çiçek türlerini yüksek doğrulukla sınıflandırabilen bir derin öğrenme modeli oluşturmaktır.  
Model, hem akademik amaçlı görüntü işleme projeleri hem de makine öğrenmesi uygulamaları için örnek teşkil etmektedir.

---

## 🗂️ Kullanılan Veri Seti

Projede TensorFlow tarafından sağlanan **Flower Photos Dataset** kullanılmıştır.

- Toplam görüntü sayısı: **3.670**
- Sınıf sayısı: **5**
  - Daisy
  - Dandelion
  - Rose
  - Sunflower
  - Tulip
- Görüntüler: Renkli (RGB)

**Veri seti kaynağı:**  
https://storage.googleapis.com/download.tensorflow.org/example_images/flower_photos.tgz

---

## 🛠️ Kullanılan Teknolojiler ve Kütüphaneler

- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Matplotlib
- pathlib, os

---

## 🧠 Model Mimarisi

Model, Evrişimli Sinir Ağı (CNN) mimarisi kullanılarak oluşturulmuştur.

- Rescaling (Normalizasyon)
- Conv2D (32 filtre)
- MaxPooling
- Conv2D (64 filtre)
- Conv2D (128 filtre)
- Flatten
- Dense (256 nöron)
- Dropout (0.3)
- Softmax çıkış katmanı

Bu yapı sayesinde model, hem uzamsal özellikleri hem de renk bilgilerini etkili şekilde öğrenmektedir.

---

## 📊 Model Eğitimi

- Kayıp fonksiyonu: `categorical_crossentropy`
- Optimizasyon algoritması: `Adam`
- Başarı metriği: `accuracy`
- Eğitim ve doğrulama verileri ayrılmıştır

---

## 🎯 Elde Edilen Sonuçlar

Eğitilen model, test verisi üzerinde yüksek doğruluk oranı elde etmiştir.  
Sonuçlar, CNN tabanlı yaklaşımların görüntü sınıflandırma problemlerinde etkili olduğunu göstermektedir.

---

## 📁 Proje Yapısı

cicek-siniflandirma-projesi/
│
├── main.py
├── README.md
├── flower_photos/
│ ├── daisy/
│ ├── dandelion/
│ ├── rose/
│ ├── sunflower/
│ └── tulip/


---

## 🚀 Çalıştırma

1. Gerekli kütüphaneleri yükleyin:
```bash
pip install tensorflow opencv-python matplotlib numpy
