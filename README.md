# ❤️ Heart Disease Prediction Model
### Makine Öğrenmesi ile Kalp Hastalığı Tahmini  
🚀 Veri Bilimine Giriş Dersi — Final Projesi

---

## 📌 Proje Özeti

Bu proje, **Heart Disease (Kalp Hastalığı)** veri seti kullanılarak bireylerin kalp hastalığı riski taşıyıp taşımadığını makine öğrenmesi yöntemleriyle tahmin etmeyi amaçlamaktadır.

Modelleme sürecinde üç farklı sınıflandırma algoritması kullanılmıştır:

- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Multi-Layer Perceptron (MLP Neural Network)**

Tüm modeller karşılaştırılmış, eğitim–test performansları değerlendirilmiş ve sonuçlar görselleştirilmiştir.

---

## 🗂️ Veri Seti Hakkında

Kullanılan **heart.csv** veri seti çeşitli klinik ölçümler içermektedir.

Örnek değişkenler:

- `age` → Yaş  
- `sex` → Cinsiyet  
- `cp` → Göğüs ağrısı tipi  
- `trestbps` → Dinlenme kan basıncı  
- `chol` → Serum kolesterol seviyesi  
- `thalach` → Maksimum kalp atış hızı  
- `exang` → Egzersizle tetiklenen anjina  
- `oldpeak`, `slope`, `ca`, `thal` → Ek klinik parametreler  
- `target` → (0 = Sağlıklı, 1 = Kalp hastalığı riski var)

---

## 🔍 Proje Adımları

### **1. Veri Yükleme ve Ön İnceleme**
- `head()`, `info()`, `describe()` fonksiyonlarıyla veri yapısı incelendi.  
- Eksik değer kontrolü yapıldı ve veri setinde eksik değer olmadığı belirlendi.

### **2. Veri Keşfi (EDA)**
- Yaş, kolesterol gibi değişkenlerin dağılımları incelendi.  
- Hedef değişken dağılımı analiz edildi.  
- Korelasyon matrisi ile değişkenler arasındaki ilişkiler görselleştirildi.

### **3. Veri Ön İşleme**
- `target` değişkeni çıktı (y) olarak ayrıldı.  
- Bağımsız değişkenler **StandardScaler** ile ölçeklendirildi.  
- Veri %80 eğitim – %20 test olarak bölündü.

### **4. Modelleme**
Üç farklı model oluşturuldu:

#### ✔ Logistic Regression  
Basit, hızlı ve yorumlanabilir bir modeldir.

#### ✔ KNN (K-En Yakın Komşu)  
Özellikle ölçeklendirilmiş verilerde etkili olan mesafe tabanlı bir algoritmadır.

#### ✔ MLP Classifier (Yapay Sinir Ağı)
- 2 gizli katman (32 → 16 nöron)  
- ReLU aktivasyon fonksiyonu  
- Maksimum 500 iterasyon  

---

## 📊 Model Sonuçları

Aşağıda genel performans değerlendirmesi yer almaktadır:

| Model | Accuracy |
|-------|----------|
| Logistic Regression | ⭐ İyi |
| KNN | ⭐⭐ Daha iyi |
| MLP Classifier | ⭐⭐⭐ En yüksek doğruluk |

MLP modeli, proje kapsamında **en başarılı sınıflandırıcı** olmuştur.

Her model için ayrıca:

- Confusion Matrix  
- Classification Report  
- Precision, Recall, F1-Score  

hesaplanmıştır.

---

## 📈 Görselleştirmeler

Notebook içerisinde üretilen başlıca grafikler:

- Hedef değişkeni dağılım grafiği  
- Yaş ve kolesterol histogramları  
- Boxplot analizleri  
- Korelasyon matrisi (heatmap)  
- Accuracy karşılaştırma grafiği  
- Confusion Matrix heatmap’leri  

Bu grafikler, veriyi daha iyi anlamak ve model performansını değerlendirmek için kullanılmıştır.

---

## 🧠 Kullanılan Teknolojiler

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-Learn  
- Jupyter Notebook

---

## 🧾 Proje Dosyaları

| Dosya | Açıklama |
|-------|----------|
| **HeartDiseasePredictionModel.ipynb** | Tüm Python & ML kodlarını içerir |
| **heart.csv** | Kullanılan veri seti |
| **README.md** | Proje açıklama dosyası |

---

## 👨‍🎓 Proje Sahibi

**Ekip**  
İstanbul Medeniyet Üniversitesi — Bilgisayar Mühendisliği  
*Buğrahan Ata / Ahmet Faruk Kurtkadiroğlu*

