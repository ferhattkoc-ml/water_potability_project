# water_potability_project
🌊 Water Potability Prediction

💧 Machine Learning ile İçme Suyu Kalitesi Tahmini

Bu proje, içme suyunun güvenli olup olmadığını tahmin etmek için geliştirilen bir Makine Öğrenmesi sınıflandırma modelidir. Veri seti; pH, sertlik, mineral oranları, klor, iletkenlik gibi su kalitesini belirleyen fiziksel ve kimyasal parametreleri içermektedir.

Çalışmada özellikle Decision Tree ve Random Forest modelleri kullanılarak suyun “içilebilir — 1” veya “içilemez — 0” sınıfına ayrılması hedeflenmiştir.

⸻

🔍 Amaç
	•	İçme suyunun laboratuvar sonuçlarına göre potabilitesini tahmin etmek
	•	Fiziksel ve kimyasal değişkenlerin su kalitesi üzerindeki etkisini incelemek
	•	Doğru ve hızlı çalışan bir karar destek sistemi geliştirmek

⸻

🧪 Kullanılan Modeller
	•	🌳 Decision Tree Classifier
	•	🌲 Random Forest Classifier
	•	Feature importance analizi yapıldı
	•	Overfitting engellenmesi için hiperparametre optimizasyonu uygulandı

⸻

📊 Veri Seti

Veri seti şu değişkenlerden oluşmaktadır:
	•	pH
	•	Hardness
	•	Solids
	•	Chloramines
	•	Sulfate
	•	Conductivity
	•	Organic Carbon
	•	Trihalomethanes
	•	Turbidity
	•	Potability (Hedef Değişken)

Eksik veriler uygun tekniklerle işlendi.

⸻

🚀 Sonuçlar
	•	Random Forest modeli, su kalitesinin belirlenmesinde en başarılı model olmuştur.
	•	Su potabilitesinde en etkili değişkenler: Organic Carbon, Hardness ve Sulfate
	•	Oluşturulan model, gerçek dünyadaki su analizlerinde hızlı ön değerlendirme amacıyla kullanılabilir.

⸻

📌 Öne Çıkanlar

⭐ Veri temizleme, eksik değer tamamlama
⭐ Sınıflandırma modellerinin karşılaştırılması
⭐ Feature importance görselleştirmeleri
⭐ Hem akademik hem uygulamalı kullanım için uygun altyapı

⸻

🛠️ Kullanılan Teknolojiler
	•	Python
	•	Pandas
	•	Scikit-Learn
	•	Matplotlib / Seaborn
	•	Jupyter Notebook

⸻

📂 Notebook

📎 Projenin tüm kodları Jupyter Notebook dosyasında detaylı şekilde verilmiştir.

⸻
