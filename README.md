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

# PHP FrameWork

## Laravel 
Modern php uygulamaları oluşturmak için kullanılır.

* Dil : PHP
* [MVC](https://github.com/xBugor/MVC "MVC NEDİR") yapısıyla çalışır.
* OOP sistemine hakim olmak gerekir.
* Açık Kaynak kodludur.
* Ölçeklenebilirlik: Modüler yapı ve yerleşik araçlar ölçeklenebilir uygulama geliştirmeyi destekler.

* Güçlü bir topluluğa sahib olan laravel ilk defa öğrenmek isteyenler için [laracats](https://laracasts.com/)  adında bir platform kurmuştur eğtim alabilirsiniz.
* **Object Relational** Mapping kullanarak çok karmaşık ve uzun sql komutlarını nesneye yönelik programlama kullanarak daha kısa ve verimli şekilde kullanmamıza olanak sağlar.(bknz: **Elequent ORM**)
* Güvenlik: CLI komutlarını güvenli bir şekilde yürütmek için SSH (Güvenli Kabuk) kullanır.
* **Blade Templating**:   HTML ve PHP kodlarını karıştırarak dinamik sayfalar oluşturur.
* **Middleware (Ara Katman)**: Middleware, gelen HTTP isteklerini filtrelemeye olanak tanır.
* **Migrations ve Seeding**: Laravel, veritabanı sürümlemeyi ve test amaçlı veritabanı verisi eklemeyi kolaylaştıran migration ve seeding özellikleri sunar.
* **Artisan CLI**, Laravel’in güçlü komut satırı aracıdır. Veri tabanı oluşturma,çalıştırma, model oluşturma vs gibi işlemleri yapabilirsiniz.
## Symfony




## Codeignitor 

* Dil : PHP
* Hızlı ve hafiftir çünkü kütüphanesi daha az bellek tüketir.
* Öğrenmesi basittir.PHP ye aşina olan herkes Codeignitoru rahatça kavrayabilir.
* [MVC](https://github.com/xBugor/MVC "MVC NEDİR") yapısıyla çalışır.
* Yüksek performanslı.
* Basitleştirilmiş kod yapısı.
* Gelişmiş Güvenlik Özelliklerine sahiptirç
* Active Record sistemi kullanır.

PHP frameworkleri yukarıdaki gibidir.

Her birinin avantajları ve dezavantajları aşağıdaki tabloda belirtilmiştir.

| Özellik   | Laravel  | Symfony  | CodeIgniter |
|-----------|---------|----------|-------------|
| **Öğrenme kolaylığı** | Kolay öğrenilir başta kavramaları kavranması zordur  | Öğrenmesi zordur kapsamlı bilgi gerektirir. | En kolay öğrenilen frameworktür. |
|**Performans** | Kaynak kullanımı fazladır. Önbellekleme gibi optimizasyonlarla düzeltilebir.| Diğerlerine göre daha fazla kaynak tüketimini sebep olur. (Modülerlik)| Hafif ve az kaynak kullanımı|
**Kullanım Alanı**| Büyük ve orta ölçekli projeler için uygundur. API geliştirme için ideal| Kurumsal ve büyük projelerde kullanmak için daha uygundur. Modüler özelleştirilebilir.| Küçük ve orta ölçekli projelerde uygundur. Bütük projelerde eksik kalabilir.|
|**MVC Desteği**| MVC vardır|Modüler MVC destekler.|Destek var ama katı değil.
|**Topluluk desteği**| Çok büyük bir topluluğa sahiptir ve laracasts gibi eğitim kaynakları mevcuttur| Symfony php ekosisteminde yaygındır.| Büyük bir topluluk değil temel destek var|
| **Güvenlik** | CSRF, XSS, SQL Injection gibi tehditlere karşı güçlü güvenlik önlemleri içerir. |  Yüksek güvenlik standartlarına sahiptir. | Güvenlik mekanizmaları temel düzeydedir.|
| **Ölçeklenebilirlik** | Büyük projeler için ölçeklenebilir, microservices ile uyumlu. | Büyük ve kurumsal projeler için en uygun framework. |  Ölçeklenebilirlik konusunda sınırlamalar olabilir. |
| **Özellik Zenginliği** | Task scheduling, queue sistemi, authentication, Blade template engine gibi birçok yerleşik özellik sunar. | Modüler yapısı sayesinde genişletilebilir, her şeyi içerir.  Ancak bazı temel özellikler için ekstra konfigürasyon gerekebilir. | Laravel ve Symfony’ye kıyasla çok az yerleşik özellik içerir. |
| **ORM Desteği** | Eloquent ORM, kullanımı kolay ve güçlü. |  Doctrine ORM, çok güçlü ancak öğrenmesi daha zor. | ORM yerine Active Record sistemi kullanır, Eloquent kadar güçlü değil. |



### Yukardaki bazı kavramlar

- **Task Scheduling** (Görev Zamanlayıcı)
Cron job yazmaya gerek kalmadan zamanlanmış görevler tanımlanması.
   - 1 . Örneğin, her gün belirli bir saatte bir e-posta göndermek için:
 
- **Queue Sistemi (Kuyruk İşlemleri)**
Yoğun işlemleri (örneğin e-posta gönderme, büyük veri işlemleri) kuyruğa alarak asenkron çalıştırabilir.
Böylece performans artar.

- **Authentication (Kimlik Doğrulama)** k
Laravel’de kimlik doğrulama (authentication) yerleşik olarak gelir. Kullanıcı giriş-çıkışı, şifre sıfırlama, iki faktörlü kimlik doğrulama gibi işlemler kolayca yapılabilir.

- **Blade Template Engine**
Laravel’in kendi şablon motoru (Blade) sayesinde dinamik HTML sayfaları kolayca oluşturulabilir.
Bu, PHP ve HTML’yi birleştirmeyi çok daha pratik hale getirir.


|  ORM |  Active Record  |
|-----------|---------|
|Genel bir kavramdır.| ORM nin bir türüdür. Tasarım deseni|
|Farklı ORM türleri olabilir (Data Mapper, Active Record vb.).	|Veriyi temsil eden nesneler doğrudan veritabanı tablolarına karşılık gelir.
|veritabanı tablolarını nesne yönelimli programlama dillerindeki nesnelere dönüştürerek veritabanı işlemlerini daha kolay ve doğal hale getirmektir.|

ORM, veritabanı ve nesne yönelimli programlama dilleri arasında bir köprüdür.

Active Record, bu köprüyü kurmak için kullanılan bir tasarım desenidir.

 ORM bir tekniktir, Active Record ise bu tekniğin bir uygulama şeklidir (desenidir). Yani, Active Record bir ORM desenidir.

  Genel ORM araçları(Entity framework, Laravel Eloquent) Active Record'a göre daha fazla esneklik sunabilir, daha karmaşık veritabanı yapılarını ve sorgularını destekleyebilir. Active Record ise daha çok hızlı ve basit veritabanı işlemleri için uygundur.