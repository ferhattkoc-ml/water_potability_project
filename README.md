<div align="center">

# 🌊 Water Potability Prediction

**Machine Learning ile İçme Suyu Kalitesi Tahmini**

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

</div>

---

## 📌 Proje Hakkında

Bu proje, içme suyunun güvenli olup olmadığını tahmin etmek için geliştirilmiş bir **Makine Öğrenmesi sınıflandırma modelidir**. Su numunelerinin fiziksel ve kimyasal parametrelerini kullanarak suyun **içilebilir (Potable)** veya **içilemez (Not Potable)** olduğunu tahmin eder.

Karar destek sistemi olarak; **Decision Tree** ve **Random Forest** algoritmaları karşılaştırılmış, hiperparametre optimizasyonu ile en başarılı model belirlenmiştir.

---

## 📊 Veri Seti

Veri seti 9 bağımsız değişken ve 1 hedef değişkenden oluşmaktadır:

| Değişken | Açıklama | Birim |
|----------|----------|-------|
| `pH` | Suyun asitlik/bazlık derecesi | — |
| `Hardness` | Su sertliği | mg/L |
| `Solids` | Toplam çözünmüş katı madde | ppm |
| `Chloramines` | Kloramin miktarı | mg/L |
| `Sulfate` | Sülfat miktarı | mg/L |
| `Conductivity` | Elektriksel iletkenlik | μS/cm |
| `Organic Carbon` | Organik karbon miktarı | mg/L |
| `Trihalomethanes` | Trihalometan miktarı | μg/L |
| `Turbidity` | Bulanıklık | NTU |
| **`Potability`** | **Hedef: 1 (İçilebilir) / 0 (İçilemez)** | — |

Eksik veriler uygun istatistiksel yöntemlerle işlenmiş, outlier analizi yapılmıştır.

---

## 🧪 Metodoloji

```
Ham Veri → Eksik Veri İşleme → Train/Test Split → Model Eğitimi → Hiperparametre Optimizasyonu → Değerlendirme
```

| Adım | Açıklama |
|------|----------|
| **Veri Ön İşleme** | Eksik değer doldurma, outlier tespiti, özellik ölçeklendirme |
| **Model 1** | 🌳 Decision Tree Classifier (temel model) |
| **Model 2** | 🌲 Random Forest Classifier (ensemble model) |
| **Optimizasyon** | GridSearchCV ile hiperparametre tuning, overfitting önleme |
| **Değerlendirme** | Accuracy, Precision, Recall, F1-Score, Confusion Matrix |

---

## 📈 Sonuçlar

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| 🌳 Decision Tree | ~%76 | ~%74 | ~%73 | ~%73 |
| 🌲 **Random Forest** | **~%82** | **~%80** | **~%79** | **~%79** |

**Random Forest** modeli su potabilitesi tahmininde en başarılı model olarak belirlenmiştir.

### 🔑 En Etkili Değişkenler (Feature Importance)

1. 🥇 **Organic Carbon** — Organik karbon seviyesi
2. 🥈 **Hardness** — Su sertliği
3. 🥉 **Sulfate** — Sülfat oranı

Bu değişkenler su kalitesi üzerinde en yüksek etkiye sahip parametrelerdir.

---

## ⚙️ Kullanım

```bash
# 1. Depoyu klonla
git clone https://github.com/ferhattkoc-ml/water_potability_project.git
cd water_potability_project

# 2. Sanal ortam oluştur (opsiyonel)
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows

# 3. Bağımlılıkları yükle
pip install -r requirements.txt

# 4. Notebook'u aç
jupyter notebook
```

---

## 🛠️ Tech Stack

| Kategori | Teknolojiler |
|----------|-------------|
| **Dil** | Python 3.8+ |
| **Veri İşleme** | Pandas, NumPy |
| **Makine Öğrenmesi** | scikit-learn (Decision Tree, Random Forest, GridSearchCV) |
| **Görselleştirme** | Matplotlib, Seaborn |
| **Ortam** | Jupyter Notebook |

---

## 📂 Proje Yapısı

```
water_potability_project/
├── water_potability.ipynb   # Ana notebook
├── requirements.txt         # Bağımlılıklar
├── README.md                # Bu dosya
└── LICENSE                  # MIT Lisansı
```

---

## 👤 Yazar

**Ferhat Koç** · [GitHub](https://github.com/ferhattkoc-ml) · [LinkedIn](https://linkedin.com/in/ferhattkocc/)

> ⭐ Bu projeyi beğendiyseniz bir yıldız bırakmayı unutmayın!

---

<div align="center">
  <sub>Built with ❤️ by Ferhat Koç</sub>
</div>
