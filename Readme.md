# 🚀 Kişisel Blog ve Yönetim Paneli (PHP Web Programlama Ödevi)

Bu proje, Web Programlama dersi kapsamında vize ve final gereksinimlerini karşılamak amacıyla geliştirilmiş, dinamik içerik yönetimine sahip tam kapsamlı bir kişisel blog web sitesidir. 

Proje, herhangi bir harici veritabanı (MySQL vb.) kullanılmadan, verilerin **JSON dosyası** üzerinde işlendiği dosya tabanlı bir sistemle kurgulanmıştır.

## 🎯 Projenin Amacı ve Özellikleri
Öğrencilerin PHP ile dinamik web sayfaları oluşturabilme becerisini göstermesi hedeflenen bu projede, ödev yönergesindeki tüm şartlar başarıyla uygulanmıştır:

* **Gelişmiş Site Yapısı:** Ana sayfa, Blog, Projeler, Hakkımda, İletişim ve Admin Paneli olmak üzere toplam 6 sayfadan oluşmaktadır.
* **Dinamik İçerik ve Döngüler:** Blog yazıları ve projeler listesi, PHP dizileri kullanılarak (`foreach` döngüleri ile) dinamik olarak ekrana yazdırılmaktadır.
* **Koşul Yapıları (if/else):** Admin paneline giriş sisteminde, iletişim formunda ve sayfa içerik kontrollerinde aktif olarak koşul yapıları kullanılmıştır.
* **Veri Saklama (JSON):** Yönetim panelinden eklenen yeni blog yazıları `data/admin_blogs.json` dosyasına kaydedilmekte ve anında sitede listelenmektedir.
* **Yönetim Paneli (Admin):** Yetkisiz girişleri engelleyen `session` (oturum) kontrollü bir yönetici paneli bulunmaktadır. Bu panel üzerinden yeni içerik eklenebilir veya silinebilir.

## 🛠️ Kullanılan Teknolojiler
* **Backend:** PHP 8
* **Frontend:** HTML5, CSS3 (Modern Flexbox & Grid yapıları)
* **Veritabanı:** Dosya Tabanlı JSON (`admin_blogs.json`), PHP Dizileri
* **İkonlar:** FontAwesome

## 📂 Klasör Yapısı
```text
/proje-klasoru
│
├── data/
│   └── admin_blogs.json     # Admin panelinden eklenen yazıların tutulduğu veri dosyası
├── includes/
│   ├── blog_data.php        # Statik blog yazılarının bulunduğu ana dizi dosyası
│   ├── header.php           # Tüm sayfaların ortak üst menüsü (Navbar)
│   └── footer.php           # Tüm sayfaların ortak alt bölümü
│
├── style.css                # Sitenin ana tasarım dosyası
├── index.php                # Ana Sayfa (Son 3 blog yazısını çeker)
├── blog.php                 # Tüm blog yazılarının listelendiği sayfa
├── blog-detail.php          # Seçilen blog yazısının detay sayfası
├── projeler.php             # PHP dizisi ile oluşturulan projeler sayfası
├── about.php                # Hakkımda sayfası
├── contact.php              # İletişim formu sayfası
├── admin.php                # Admin giriş ekranı (Kullanıcı adı ve şifre kontrolü)
└── dashboard.php            # Admin yönetim paneli (İçerik ekleme/silme)





⚙️ Kurulum ve Çalıştırma

Projeyi yerel ortamınızda (Localhost) çalıştırmak için aşağıdaki adımları izleyin:

Bilgisayarınıza XAMPP veya benzeri bir yerel sunucu yazılımı kurun.

XAMPP Control Panel üzerinden Apache modülünü başlatın.

Bu repository'deki tüm dosyaları indirin veya klonlayın.

Dosyaları bilgisayarınızdaki C:\xampp\htdocs\ klasörünün içine yeni bir klasör açarak (örn: blog-projesi) yerleştirin.

Tarayıcınızın adres çubuğuna http://localhost/blog-projesi yazarak siteye erişin.

🔐 Admin Paneli Giriş Bilgileri:

Kullanıcı Adı: Salih1903

Şifre: 1903