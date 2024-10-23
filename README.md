# akbank-ai
# KAGGLE LINK = https://www.kaggle.com/code/mehmeterdemgndz/erdemgndz-akbank-project
## Projenin Test Accuracy değeri %96.6 olarak sonuçlanmıştır.
## Model nöron sayıları sırasıyla 512-256-128-64 olan 4 Katmandan oluşmaktadır. 
### Farklı nöron ve katman sayılarıyla incelemelerde bulunduğumda en optimal olarak bu sonuca ulaştım.
### Modelde DROPOUT katmanı kullanmadım çünkü yaptığım değerlendirmelerde dropout katmanı modelin öğrenmesini önemli ölçüde sınırladı. Bu durum OVERFITTING artırıyor gibi gözükmekte ancak aldığım test skorunun yüksek olması sebebiyle modele yine de dropout katmanı eklemedim. Ancak dropout katmanını çok sayıda nöronlu katmanlardan sonra kullanmanın bu model üzerinde daha doğru olduğu sonucuna vardığımı belirtmek isterim.
### Sanıyorum elimizdeki veri setinin görece basit olması ve veri setindeki örneklerin birbirine çok yakın olmasından kaynaklanıyor. Bu nedenle model veri setindeki TEST örneklerinde çok yüksek skorlar veriyor ancak veri seti dışına çıkıldığında modelin sonuçları kötüleşebilir. Dolayısıyla modelin başka veri ve farklı parametre kombinasyonlarıyla eğitilmesi gerekebilir.
## Learning Rate parametresini çeşitli denemeler sonucunda "0.0001" olarak belirledim.
## Batch Size parametresini 16-32-64-128 değerleriyle denedikten sonra accuracy scorelarına önemsenmeyecek derecede etkisi olduğunu fark ettim ve "64" olarak belirledim.
## Optimizer olarak çoğu modelde kullanılan ve en optimal sonucu veren "Adam" optimizerini kullandım.
# Geri Dönütlerinizi bildirirseniz sevinirim
