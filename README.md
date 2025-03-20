# Web FrameWork Nedir?

Web frameworkleri yazılım geliştiricileri tarafından önceden yazılmış kütüphanelerin toplanıp oluşturulan  yapılardır.
Sık kullanılan kodları sayfa sayfa yeniden yazmadan hızlıca amacımıza ulaştıran hazır kodlar gibi düşünebilirsiniz.

Back-end ve Front-end frameworkleri, mobil uygulama geliştirme frameworkleri ve veri bilimi frameworkleri  gibi birçok framework çeşidi bulunmaktadır.

İhtiyaca göre kullanılabilen ve değiştirilebilen genel bir şablondur.

## Avantajlar
- Hızlı kod yazmayı sağlar.
- Kod düzeni sağlar. Anlaşılması ve üzerinde çalışılması çok daha kolaydır
- Bakım kolaylığı:  Güncellemeler ve iyileştirmeler genellikle framework tarafından yapılır, bu da geliştiricinin bakım yükünü azaltır.
- Ölçeklenebirlik , uygulamanın artan kullanıcı sayısı ve veri yüküyle başa çıkabilme yeteneğidir.
- Açık kaynak kodludur. Kodları değiştirip,güncelleyip kullanabilirsiniz.
- SQL injection XSS gibi saldıralara karşı korunma sağlar.

Geliştirme sürecine başlamadan önce, projeniz için hangi programlama dilinin uygun olacağını seçmeniz gerekir.

# Web Framework Çeşitleri

## 1. Backend (Sunucu Tarafı) Frameworkler
| Framework       | Dil          | Özellikler |
|---------------|------------|------------|
| **Laravel**   | PHP        | MVC yapısı, Blade template engine, güçlü ORM (Eloquent), kolay kimlik doğrulama |
| **Django**    | Python     | Güçlü güvenlik, [ORM](#Orm) desteği, admin paneli, hızlı geliştirme |
| **Flask**     | Python     | Minimalist yapı, genişletilebilir, esnek |
| **Express.js**| JavaScript (Node.js) | Hafif ve hızlı, REST API geliştirmeye uygun |
| **Spring Boot** | Java     | Mikroservis desteği, kapsamlı güvenlik özellikleri |
| **Ruby on Rails** | Ruby   | "Convention over Configuration" prensibi, güçlü ORM (Active Record) |

## 2. Frontend (İstemci Tarafı) Frameworkler
| Framework   | Dil         | Özellikler |
|------------|------------|------------|
| **React.js**  | JavaScript | Bileşen tabanlı yapı, sanal DOM, hızlı performans |
| **Vue.js**    | JavaScript | Kolay öğrenim, esnek yapı, reaktif sistem |
| **Angular**   | TypeScript | Büyük ölçekli projeler için uygun, güçlü entegrasyonlar |
| **Svelte**    | JavaScript | Sanal DOM yerine doğrudan derleme, performans avantajı |

## 3. Full-Stack Frameworkler
| Framework   | Dil         | Özellikler |
|------------|------------|------------|
| **Next.js**   | JavaScript | SSR (Sunucu Tarafı Render), React ile uyumlu, SEO dostu |
| **Nuxt.js**   | JavaScript | Vue.js tabanlı, SSR ve statik site desteği |
| **Meteor.js** | JavaScript | Gerçek zamanlı uygulamalar için ideal, full-stack çözüm |
| **Blitz.js**  | JavaScript | Next.js tabanlı, tam entegre full-stack çözüm |

## 4. UI Frameworkler (CSS & UI Kütüphaneleri)
| Framework     | Kullanım Alanı | Özellikler |
|--------------|---------------|------------|
| **Bootstrap** | CSS & UI | Responsive tasarım, hazır bileşenler, kolay grid sistemi |
| **Tailwind CSS** | CSS Utility | Düşük seviyeli sınıflarla esnek stil oluşturma |
| **Material UI** | React UI Kit | Google’ın Material Design sistemine uygun React bileşenleri |
| **Ant Design** | React UI Kit | Büyük ölçekli projeler için kapsamlı bileşenler |
| **Bulma** | CSS & UI | Modern ve hafif CSS frameworkü |


Bu yazımızda php frameworklerine detaylı yer verilmiştir.

## Laravel 

* Dil : PHP
* [MVC](https://github.com/xBugor/MVC "MVC NEDİR") yapısıyla çalışır.
* OOP sistemine hakim olmak gerekir.
* Açık Kaynak kodludur.
* Ölçeklenebilirlik: Modüler yapı ve yerleşik araçlar ölçeklenebilir uygulama geliştirmeyi destekler.

* Güçlü bir topluluğa sahib olan laravel ilk defa öğrenmek isteyenler için [laracats](https://laracasts.com/)  adında bir platform kurmuştur eğtim alabilirsiniz.
* **Object Relational Mapping** kullanarak çok karmaşık ve uzun sql komutlarını nesneye yönelik programlama kullanarak daha kısa ve verimli şekilde kullanmamıza olanak sağlar.(bknz: **Elequent ORM**) [ORM](https://github.com/xBugor/ORM)
* **Routing (Yönlendirme)**: Laravel, URL yönlendirmeleri için oldukça esnek ve güçlü bir yönlendirme sistemi sunar. Route'lar kolayca tanımlanabilir ve yönetilebilir.
* **Blade Templating**:   HTML ve PHP kodlarını karıştırarak dinamik sayfalar oluşturur.
* **Middleware (Ara Katman)**: Middleware, gelen HTTP isteklerini filtrelemeye olanak tanır.
* **Migrations ve Seeding**: Laravel, veritabanı sürümlemeyi ve test amaçlı veritabanı verisi eklemeyi kolaylaştıran migration ve seeding özellikleri sunar. Değişiklikleri yönetmek migrations,veritabanına başlangıç verisi eklemeye seeding.
* **Artisan CLI**, Laravel’in güçlü komut satırı aracıdır. Veri tabanı oluşturma,çalıştırma, model oluşturma vs gibi işlemleri yapabilirsiniz.
* **Authentication ve Authorization** Kullanıcı girişi, yetkilendirme ve şifreleme işlemleri için hazır araçlar sunar. [Laravel Breeze](https://laravel.com/docs/10.x/starter-kits#laravel-breeze)
* **Queues ve Jobs**: Laravel, arka planda işlem yapmayı sağlayan Queue ve Job yapısını destekler. Bu, zaman alan görevleri (örneğin, e-posta gönderme, video işleme) kullanıcı etkileşimi dışında çalıştırılmasını sağlar.
* **Laravel Forge ve Envoyer**: Laravel Forge, Laravel projelerini sunuculara dağıtmayı otomatikleştiren bir platformdur. Envoyer ise Laravel uygulamaları için sıfır kesintiyle dağıtım yapmayı sağlar. Kullanıcılar, uygulamanıza her yeni güncelleme geldiğinde, kesinti yaşanmaz.
* **Laravel Ecosystem**: Laravel ekosistemi, Laravel Passport (API Authentication), Laravel Horizon (Queue yönetimi), Laravel Nova (Admin paneli) gibi bir dizi araç ve paketle genişletilebilir.


* **Güvenlik**: CLI komutlarını güvenli bir şekilde yürütmek için SSH (Güvenli Kabuk) kullanır.


## Symfony

* Dil : PHP
* Modüler ve genişletilebir bir yapıya sahitir.
* [MVC](https://github.com/xBugor/MVC "MVC NEDİR") yapısıyla çalışır.
* Öğrenmesi zordur.
* Büyük ve kurumsal işlemlerde rahatça kullanılabilir.
* Düzenli güncellemeler
* Yeniden kullanılabilir kod bileşenleri
* Laravel’in temelinde Symfony bileşenleri yer alır.
* Symfony Flex – Projeleri daha esnek ve hafif hale getiren bir yönetim sistemidir.


## Codeigniter 

* Dil : PHP
* Hızlı ve hafiftir çünkü kütüphanesi daha az bellek tüketir.
* Öğrenmesi basittir.PHP ye aşina olan herkes Codeignitoru rahatça kavrayabilir.
* [MVC](https://github.com/xBugor/MVC "MVC NEDİR") yapısıyla çalışır.
* Yüksek performanslı.
* Basitleştirilmiş kod yapısı.
* Gelişmiş Güvenlik Özelliklerine sahiptirç
* Active Record sistemi kullanır.
* Kolay Kurulum – Composer gerektirmez, doğrudan indirip çalıştırabilirsiniz.

PHP frameworkleri yukarıdaki gibidir.

Her birinin avantajları ve dezavantajları aşağıdaki tabloda belirtilmiştir.

| Özellik   | Laravel  | Symfony  | CodeIgniter |
|-----------|---------|----------|-------------|
| **Öğrenme kolaylığı** | Kolay öğrenilir başta kavramaarı anlamak zor gelebilir  | Öğrenmesi zordur kapsamlı bilgi gerektirir. | En kolay öğrenilen frameworktür. |
|**Performans** | Kaynak kullanımı fazladır. Önbellekleme gibi optimizasyonlarla düzeltilebir.| Diğerlerine göre daha fazla kaynak tüketimini sebep olur. (Modülerlik)| Hafif ve az kaynak kullanımı|
**Kullanım Alanı**| Büyük ve orta ölçekli projeler için uygundur. API geliştirme için idealdir.| Kurumsal ve büyük projelerde kullanmak için daha uygundur.| Küçük ve orta ölçekli projelerde uygundur. Büyük projelerde eksik kalabilir.|
|**MVC Desteği**| MVC vardır|Modüler MVC destekler.|Destek var ama katı değil.
|**Topluluk desteği**| Çok büyük bir topluluğa sahiptir ve laracasts gibi eğitim kaynakları mevcuttur| Symfony php ekosisteminde yaygındır.| Büyük bir topluluk değil temel destek var|
| **Güvenlik** | CSRF, XSS, SQL Injection gibi tehditlere karşı güçlü güvenlik önlemleri içerir. |  Yüksek güvenlik standartlarına sahiptir. | Güvenlik mekanizmaları temel düzeydedir.|
| **Ölçeklenebilirlik** | Büyük projeler için ölçeklenebilir, microservices ile uyumlu. | Büyük ve kurumsal projeler için en uygun framework. |  Ölçeklenebilirlik konusunda sınırlamalar olabilir. |
| **Özellik Zenginliği** | Task scheduling, queue sistemi, authentication, Blade template engine gibi birçok yerleşik özellik sunar. | Modüler yapısı sayesinde genişletilebilir, her şeyi içerir.  Ancak bazı temel özellikler için ekstra konfigürasyon gerekebilir. | Laravel ve Symfony’ye kıyasla çok az yerleşik özellik içerir. |
| **ORM Desteği** | Eloquent ORM, kullanımı kolay ve güçlü. |  Doctrine ORM, çok güçlü ancak öğrenmesi daha zor. | ORM yerine Active Record sistemi kullanır, Eloquent kadar güçlü değil. |

## Hangisini Seçmelisin?
| **İhtiyacın** | **Önerilen Framework** |
|--------------|------------------------|
| Küçük ve hızlı bir proje mi yapıyorsun? | **CodeIgniter** |
| Modern ve ölçeklenebilir bir web uygulaması mı istiyorsun? | **Laravel** |
| Kurumsal, büyük ve modüler bir uygulama mı geliştireceksin? | **Symfony** |


### Bazı kavramlar

- **Task Scheduling** , belirli görevlerin otomatik olarak belirli zamanlarda çalışmasını sağlar. Laravel, bu işlemi schedule komutuyla yapar. <code> `app/Console/Kernel.php `</code> dosyasına  görevler eklenir. Zamanlanmış görevler, cron job kullanılarak çalıştırılır ve Laravel, bu görevlerin düzenli olarak belirlenen aralıklarla çalışmasını sağlar. Bu özellik, örneğin e-posta gönderme, veritabanı yedekleme gibi işlemler için oldukça kullanışlıdır.
   -  Örneğin, her gün belirli bir saatte bir e-posta göndermek için:
 
- **Queue Sistemi (Kuyruk İşlemleri)**
Yoğun işlemleri (örneğin e-posta gönderme, büyük veri işlemleri) kuyruğa alarak asenkron çalıştırabilir.
Böylece performans artar.

- **Authentication (Kimlik Doğrulama)** 
Laravel’de kimlik doğrulama (authentication) yerleşik olarak gelir. Kullanıcı giriş-çıkışı, şifre sıfırlama, iki faktörlü kimlik doğrulama gibi işlemler kolayca yapılabilir.

- **Blade Template Engine**
Laravel’in kendi şablon motoru (Blade) sayesinde dinamik HTML sayfaları kolayca oluşturulabilir.
Bu, PHP ve HTML’yi birleştirmeyi çok daha pratik hale getirir.
- **MiddleWare** 
Middleware, Laravel'de HTTP isteklerini kontrol etmek için kullanılır.
Middleware ile istekleri filtreleyebilir, değiştirebilir ve yanıtları işleyebilirsiniz.
php artisan make:middleware komutuyla middleware oluşturabilirsiniz.
Middleware, Kernel.php dosyasında tanımlanır ve sonra route veya route grubu üzerinde kullanılabilir.

- **Route** web uygulamanızdaki URL taleplerine yanıt veren ve işlevsel işlemler yapan bir yapıdır. Laravel'in yönlendirme (routing) sistemi, gelen HTTP isteklerini belirli bir controller metoduna veya closure (anonim fonksiyon) ile eşleştirir.

 #### **ORM VE Active Record**


|  # ORM |  Active Record  |
|-----------|------------|
|Genel bir kavramdır.| ORM nin bir türüdür. Tasarım deseni|
|Farklı ORM türleri olabilir (Data Mapper, Active Record vb.).	|Veriyi temsil eden nesneler doğrudan veritabanı tablolarına karşılık gelir.
|Veritabanı tablolarını nesne yönelimli programlama dillerindeki nesnelere dönüştürerek veritabanı işlemlerini daha kolay ve doğal hale getirmektir.|

ORM, veritabanı ve nesne yönelimli programlama dilleri arasında bir köprüdür.

Active Record, bu köprüyü kurmak için kullanılan bir tasarım desenidir.

 ORM bir tekniktir, Active Record ise bu tekniğin bir uygulama şeklidir (desenidir). Yani, Active Record bir ORM desenidir.

  Genel ORM araçları(Entity framework, Laravel Eloquent) Active Record'a göre daha fazla esneklik sunabilir, daha karmaşık veritabanı yapılarını ve sorgularını destekleyebilir. Active Record ise daha çok hızlı ve basit veritabanı işlemleri için uygundur.

## KAYNAKÇA
1. [Scheduling](https://laravel.com/docs/8.x/scheduling)

2. [Symfony](https://symfony.com/doc/current/index.html)

3. [Symfony Github](https://github.com/symfony/symfony-docs)

4. [laracast](https://laracasts.com/)

5. [CodeIngineter](https://codeigniter.com/user_guide/index.html)

6. [geeksforgeeks](https://www.geeksforgeeks.org/top-frameworks-for-web-applications/#1-ruby-on-rails)