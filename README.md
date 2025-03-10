# Web FrameWork Nedir?

Web frameworkleri yazılım geliştiricileri tarafından önceden yazılmış kütüphanelerin toplanıp oluşturulan  dökümantasyonlardır.
Sık kullanılan kodları sayfa sayfa yeniden yazmaktan kurtulmaktır.
Hazır kodlar gibi düşünebiliriz.
Böylece her defasında yeniden kod satırı oluşturmaya gerek kalmadan hızlı bir şekilde amacımıza ulaşmamız sağlanır.

## Avantajlar
- Kodları hızlı bir şekilde yazmayı sağlar.
- SQL injection XSS gibi saldıralara karşı korunma sağlar.
- Kod düzeni sağlar.
- Ölçeklenebirlik
- Açık kaynak kodludur. Kodları değiştirip,güncelleyip kullanabilirsiniz.


gibi avantajları bulunmaktadır.

## Laravel :
Modern php uygulamaları oluşturmak için kullanılır.

* Dil : PHP
* MVC yapısıyla çalışır.
* OOP sistemine hakim olmak gerekir.

#### MVC NEDİR ? (Model-View-Controller)
 Yazılım geliştirmede kullanılan(özellikle webte) geliştirme patternidir.(Yazılım mimari deseni).
![xBugor ][resim]

[resim]: ./assets/mvc.jpg "Bugrahan"


Modüler bir yaklaşım kullanarak yazlımı parçalara ayırıyoruz.Bu da bir bileşende yapılan değişiklikleri bağımsızlaştırır. Bu parçalar:

* Model
* View
* Controller
* User 

### Model 

1. Verinin yönetilmesi ve iş mantığının çalışmasını yönetir.
2. Veritabanı ile iletişim kurar.
3. Controllere veri sağlar.
4. Validation işlemini gerçekleştirir.
Örnek (Django Model - Python)

### View
 Projelerimizde arayüzlerin oluştuğu bölüme view denir. Kullanıcının iletişim kuracağı ekrana view diyoruz.


 1. Kullanıcıya verileri görüntüler
 2. HTML ,CSS ,JavaScript  kullanarak görsel bir arayüz sunar.


### Controller

 1. Kullanıcıdan gelen istekler burda değerlendirilir. İsteğin detaylarına göre hangi işlemin yapılacağını seçer.(veri güncelleme gibi )

2. Gerekli verileri Model’den alır, üzerinde işlem yapar ve View’e (görünüme) yönlendirir.
 View’e işlenmiş verileri iletir ve istemciye HTML, JSON veya başka bir formatta yanıt döndürülmesini sağlar.









Senaryo 
Kullanıcı bir istek oluşturuyor (Request)
Kullanıcı bir girdi oluşturduğu zaman bu girdiler Controllera geliyor.
Bu veriler üzerinde ne yapılacağına lojik denir.
Controller üzerinde Model(veritabanına) yapılacak bir işlem varsa yapar. Örneğin veri kaydetme gibi