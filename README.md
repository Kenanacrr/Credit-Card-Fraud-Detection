# Credit Card Fraud Detection (Kredi Kartı Dolandırıcılığı Tespiti)

## Proje Hakkında

Bu projede, Kaggle'ın geniş çaplı [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) veri seti üzerinden gözetimli öğrenme teknikleri ile kredi kartı işlemlerinin sahte olup olmadığını tahmin eden bir makine öğrenmesi modeli geliştirilmiştir.

- **Problem:** Finansal işlemlerdeki sahteciliklerin tespiti.
- **Veri seti boyutu:** 284,807 işlem, 150+ MB.
- **Hedef değişken:** Class (0: Normal, 1: Fraud).

## Kullanılan Yöntem ve Algoritma

Çeşitli modeller denenmiş ve en iyi başarıyı Random Forest algoritması göstermiştir. Ayrıca hiperparametre optimizasyonu (GridSearchCV) ile modelin performansı artırılmıştır.

### Kullanılan Modeller:
- Logistic Regression
- Decision Tree
- KNN
- **Random Forest (En iyi performans)**
- (Bonus: k-Means ile gözetimsiz kümeleme)

## Sonuçlar

- **Accuracy (Doğruluk):** %99+ (dengesiz veri nedeniyle ROC-AUC esas alındı)
- **ROC-AUC:** 0.98+
- **En önemli özellikler:** V14, V17, V12, V10 gibi bazı anonimleştirilmiş değişkenler.

> **Karmaşıklık matrisi, ROC eğrisi ve önemli değişkenler notebook'ta görselleştirilmiştir.**

## Gerçek Hayat Uygulaması

Bu proje, bankaların ve finansal kuruluşların gerçek zamanlı olarak şüpheli işlemleri tespit ederek müşterilerini ve kendisini koruma süreçlerinde birebir kullanılabilir. Daha gelişmiş sistemlerde ek veri kaynakları ve gerçek zamanlı veri akışı entegre edilebilir.

## Geliştirme Önerileri

- Veri dengesizliği için SMOTE gibi oversampling yöntemleriyle ek analiz yapılabilir.
- Deep Learning tabanlı modeller eklenebilir.
- Daha fazla özelliğe sahip farklı veri setleri denenebilir.
- Model bir arayüz veya API olarak deploy edilebilir.

## Kaggle Notebook Linki

[Kaggle Notebook'um](https://www.kaggle.com/code/kenanaar/machine-learning-bootcamp-project/edit)

---

## Dosya Listesi

- `creditcard_fraud_supervised_learning.ipynb`: Proje kodları ve teknik anlatımlar.
- `README.md`: Projenin sözel ve özet açıklamaları.

---

## Kaynaklar

- [Kaggle Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- https://gokerguner.medium.com/machine-learning-1-7d4581caa291
