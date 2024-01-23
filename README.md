# Obesity Prediction Project

Bu proje, obeziteye etki eden faktörleri inceleyen ve obezite durumunu tahminlemek için bir makine öğrenimi modeli geliştiren bir çalışmadır.

## Veri Seti

Bu projede kullanılan veri seti "Obesitydata.csv" adlı bir CSV dosyasından okunmuştur. Veri seti, obezite ile ilgili çeşitli özellikleri içermektedir.

## Kullanılan Özellikler

Proje, obezite durumunu tahminlemek için aşağıdaki özellikleri kullanmaktadır:

- Cinsiyet (Gender): Bir katılımcı erkekse 1, kadınsa 0'dır.

- Yaş (Age): Bir katılımcının yaşı, yıl cinsindendir.

- Boy (Height): Bireylerin boy uzunluğu bilgileri verilmektedir.

- Kilo (Weight): Bireylerin kilo ağırlıkları belirtilmektedir.

- Ailede Şişmanlık Hikayesi (family_history_with_overweight): Bir katılımcının ailesinde şişmanlık hikayesi varsa 1, yoksa 0'dır.

- Yüksek Kalorili Yiyecek Tüketimi (FAVC): Bir katılımcı sık sık yüksek kalorili yiyecek tüketiyorsa 1, değilse 0'dır.

- Sebze Tüketimi (FCVC): Bir katılımcı genellikle yemeklerinde sebze tüketiyorsa 1, değilse 0'dır.

- Günlük Ana Öğün Sayısı (NCP): Bir katılımcının günlük ana öğün sayısı. 0, 1-2 öğün; 1, 3 öğün; 2, 3'ten fazla öğün.

- Öğünler Arası Yiyecek Tüketimi (CAEC): Bir katılımcının öğünler arasında yemek tüketim miktarı, 0 ile 3 arasında bir ölçekte ifade edilir.

- Sigara İçme Durumu (SMOKE): Bir katılımcı sigara içiyorsa 1, içmiyorsa 0'dır.

- Su Tüketimi (CH2O): Bir katılımcının su içme miktarı, 0 ile 2 arasında bir ölçekte ifade edilir.

- Kalori Takibi (SCC): Bir katılımcı kalori alımını takip ediyorsa 1, etmiyorsa 0'dır.

- Fiziksel Aktivite Düzeyi (FAF): Bir katılımcının fiziksel aktivite düzeyi, 0 ile 3 arasında bir ölçekte ifade edilir.

- Ekran Başında Geçirilen Zaman (TUE): Bir katılımcının ekran başında geçirdiği zaman, 0 ile 2 arasında bir ölçekte ifade edilir.

- Alkol Tüketimi Sıklığı (CALC): Bir katılımcının alkol tüketme sıklığı, 0 ile 3 arasında bir ölçekte ifade edilir.

- MTRANS (Automobile, Bike, Motorbike, Public_Transportation, Walking): Bir katılımcının ana ulaşım aracını belirtir. Ana ulaşım aracı 1 olarak belirtilir, diğer araçlar 0 olarak belirtilir.

- NObeyesdad (obezite tipleri): 
  - Zayıf(Underweight): 18,5'tan az
  - Normal(Normal): 18,5 ila 24,9
  - Aşırı kilolu(Overweight): 25,0 ila 29,9
  - Obezite I(Obesity I): 30,0 ila 34,9
  - Obezite II(Obesity II): 35,0 ila 39,9
  - Obezite III(Obesity III): 40'tan yüksek

- Obezite Durumu (Obsity_Status): Bir katılımcı obezse 1, değilse 0'dır.


## Kullanım

Projenin çalıştırılması için aşağıdaki adımlar takip edilmiştir:

1. Veri setini "Obesitydata.csv" olarak sağlayın.
2. Ana kod dosyasını çalıştırarak makine öğrenimi modelini eğitin ve sonuçları gözlemleyin.

## Gereksinimler

Projenin çalışması için aşağıdaki Python kütüphanelerine ihtiyaç vardır:

- Pandas (import pandas as pd): Veri analizi ve manipülasyonu için kullanılır. Pandas DataFrame'leri ile veri tablolarını işlemek ve analiz etmek için kullanılır.

- NumPy (import numpy as np): Bilimsel hesaplamalar ve çok boyutlu dizilerle çalışmak için kullanılır.

- Matplotlib (import matplotlib.pyplot as plt): Veri görselleştirme için kullanılır. pyplot modülü, grafik çizimi ve veri görselleştirmeyi sağlar.

- PyLab (import pylab as pl): Matematiksel hesaplamalar ve grafik çizimi için kullanılır. Genellikle Matplotlib ile birlikte kullanılır.

- Seaborn (import seaborn as sns): Matplotlib tabanlı bir veri görselleştirme kütüphanesidir. Özellikle istatistiksel grafikler oluşturmak için kullanılır.

- Plotly Express (import plotly.express as px): İnteraktif ve çarpıcı grafikler oluşturmak için kullanılır. Özellikle interaktif web tabanlı uygulamalarda kullanılabilir.

- Scikit-learn (from sklearn import preprocessing, model_selection, linear_model, ensemble, tree, svm, metrics): Makine öğrenimi algoritmalarını içeren bir kütüphanedir. Öğrenme, ölçekleme, sınıflandırma, regresyon ve performans ölçümü gibi işlemleri destekler.




## Projenin Amacı
 Obezite üzerinde etkili olan faktörlerin neler olduğunu belirlemek ve bunlar üzerinde bir model oluşturarak modelin doğruluğunu ölçümlerle karşılaştırmak.

 Uygulanan modeli doğrulamak için obezite olan hastaları tespit etmek ve belirlenebilmesine yönelik veri görselleştirme yapmak ve makine öğrenimini kullanmak.

## Projenin Önemi
 Obezitenin küresel bir sağlık sorunu olması ve bu tür bir modelin kullanılarak bireylere sağlıklı yaşam tarzı konusunda bilgi verilmesi veya sağlık profesyonellerine yardımcı olmasıdır. Bu tür modeller, obeziteye yönelik önleyici stratejilerin geliştirilmesinde ve toplum sağlığının iyileştirilmesinde önemli bir rol oynayabilir.



# Obezite tahminleme yapmak için bir makine öğrenimi modeli oluşturulması aşamaları:

# Veri Toplama ve Hazırlama:

Obezite ile ilgili bir veri seti bulunması ve bu veri setini incelenmesi.
Veri setinde obezite durumunu ifade eden bir hedef değişken ve obezite ile ilişkili olabilecek özellikleri içeren sütunlar bulunmalıdır.

# Veri Keşfi ve Temizleme:

Veri setinin incelenerek eksik veya anormal değerleri tespit edilmesi ve bu değerlerin ele alınması.
Veri setindeki kategorik değişkenleri one-hot encoding veya label encoding gibi yöntemlerle sayısallaştırılması.
Anlamsız veya aykırı verilerin düzeltilmesi veya çıkarılması.

# Veri Görselleştirme
 Veri setinin daha iyi anlaşıması için veriler arasındaki bağlantıların görselleştirilmesi işlemidir. Bunun için kullanılan bazı metodlar:

  - Pair Plot: Bir veri kümesindeki farklı sayısal özelliklerin çiftler arasındaki ilişkileri ve dağılımları görselleştiren bir grafik türüdür. Seaborn kütüphanesi içinde bulunan sns.pairplot() fonksiyonu, bir DataFrame içindeki sayısal sütunlar arasındaki ilişkileri çiftler halinde gösteren bir matris oluşturur.

  - Bar Plot(Sütun Grafiği): Kategorik verilerin miktarını karşılaştırmak için kullanılır.

  - Scatter Plot(Nokta Grafiği): Scatter plot, iki değişken arasındaki ilişkiyi gösteren bir grafik türüdür. Bu grafikte, her bir veri noktası (gözlem birimi) iki değişkenin değerlerini temsil eder ve bu noktalar bir düzlem üzerine dağılmıştır. X ekseni bir değişkeni, Y ekseni ise diğer değişkeni temsil eder.

  - Histogram: Sürekli bir değişkenin dağılımını görmek için kullanılır.

  - Seaborn Linear Model Plot: sns.lmplot, Seaborn kütüphanesinde bulunan ve regresyon analizi sonuçlarını görselleştirmek için kullanılan bir fonksiyondur. Bu fonksiyon, iki sayısal değişken arasındaki ilişkiyi değerlendirmek ve bu ilişkiyi regresyon çizgisi ile göstermek amacıyla kullanılır.

  - FacetGrid: Seaborn kütüphanesinde veri görselleştirmek için kullanılan bir metoddur. Bu metot, alt grafiklere bölünmüş bir ana grafik oluşturmak ve her bir alt grafikte belirli bir alt küme veriyi göstermek için kullanılır. 

  - Pie Chart: Bir bütünün parçalarını yüzde olarak göstermek için kullanılır.

  - Heatmap: İki boyutlu bir matrisin değerlerini renklerle göstermek için kullanılır.

# Veri Bölme:

Veri setinin eğitim ve test veri setlerine ayırılması. Bu, modeli eğitirken kullanılan veri seti ile modelin gerçek dünya performansını değerlendirmek için kullanılan veri setini ayırmaya yardımcı olur.

# Model Seçimi:

Obezite tahminlemesi için uygun bir model seçilmesi. Bu veri için kullanılan makine öğrenimi modellerinin bazıları:

  - K-nearest Neighbors (K-NN): Gözetimli bir makine öğrenimi algoritmasıdır. Bir veri noktasının sınıfını, ona en yakın k komşusunun etiketi üzerinden belirler.

  - Random Forest: Birçok karar ağacını bir araya getiren bir ensemble (kolektif) öğrenme algoritmasıdır. Her ağaç, rastgele seçilmiş bir alt örneklem üzerinde eğitilir ve sonuçlarını bir araya getirerek daha güçlü ve genelleme yeteneği yüksek bir model oluşturur.

  - Support Vector Machine (SVM): Sınıflar arasında bir karar sınırı (hiper düzlem) oluşturarak veri noktalarını sınıflandırmaya çalışan bir sınıflandırma algoritmasıdır. SVM, aynı zamanda regresyon problemlerini çözmek için de kullanılabilir.

  - Logistic Regression: İki sınıflı sınıflandırma problemlerinde kullanılan bir istatistiksel modeldir. Logistik regresyon, giriş özelliklerinin ağırlıklı toplamını ve bir logit fonksiyonunu kullanarak veri noktasının bir sınıfa ait olma olasılığını tahmin eder.
  
  - Decision Tree (Karar Ağacı): Veri noktalarını sınıflandırmak veya regresyon problemlerini çözmek için kullanılan bir ağaç yapısıdır. Karar ağaçları, sırasıyla özellikler üzerinden yapılan kararlarla oluşturulur ve genellikle ağaç yapısıyle anlaşılırlığı yüksektir.
  
Seçilen modelin eğitilmesi. Eğitim veri setini kullanarak modelin obezite durumunu tahmin etmeyi öğrenmesinin sağlanması.

# Model Değerlendirmesi:

Test veri seti üzerinde modelin değerlendirilmesi. Genellikle accuracy, recall, precision ve F1-skor gibi metrikler kullanılır.

# Feature Importance Analizi:
Oluşturduğumuz model üzerinden feature importance analizi yaparak, hangi özelliklerin obeziteyi daha fazla etkilediğinin belirlenmesi.

# Tahminler Yapma:

Modeli kullanarak yeni veri noktaları üzerinde obezite tahminleri yapılması.

# Sonuçların İncelenmesi:

Tahmin sonuçlarının değerlendirilmesi ve modelin ne kadar başarılı olduğunun analiz edilmesi.














