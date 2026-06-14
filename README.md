# calc
##  WORK LOG - Kişisel Mesai Takip & Hesaplama Sistemi

WORK LOG , çalışanların mesai saatlerini yasal standartlara uygun olarak hesaplayan ve tüm verileri tamamen yerel (local) olarak kullanıcının kendi tarayıcısında saklayan tek sayfalık (Single Page Application) güvenli bir takip portalıdır.

Herhangi bir uzak sunucuya veya bulut servisine bağımlılığı olmadığı için internet bağlantısı olmadan da çalışabilir ve verileriniz üçüncü şahıslarla asla paylaşılmaz.

---

## ✨ Öne Çıkan Özellikler

*   Çoklu Kullanıcı Desteği: Aynı tarayıcı üzerinde farklı kullanıcı adları ve şifrelerle bağımsız yerel hesaplar oluşturabilme.
*   Hassas Maaş & Mesai Hesaplama: Aylık yasal çalışma süresi olan 225 saat baz alınarak; Hafta İçi (%150), Hafta Sonu (%200), Resmi Tatil (%250) ve Ek Mesai (%100)     çarpanlarına göre dinamik hakediş hesaplama.
*   Canlı Özet Kartı: Form doldurulurken anlık olarak normal saat ücretini, çarpanlı mesai ücretini ve toplam kazanılacak tutarı gösteren dinamik arayüz.
*   Gelişmiş Kullanılabilirlik (UX): Canlı özet kartındaki hesaplama detaylarını tek tıkla gizleyip gösterebilme özelliği.
*   Veritabanı Geçmişi & İstatistikler: Kaydedilen tüm geçmiş mesailerin listelenmesi, tarihe göre sıralanması, toplam mesai saati ve birikmiş toplam ödemenin anlık takibi.
*   Güvenli Silme Modalı: Yanlış girilen mesai kayıtlarının onay mekanizmasıyla yerel veritabanından kalıcı olarak silinebilmesi.
*   Modern Tasarım: Tailwind CSS ve Lucide Icons kütüphaneleri ile güçlendirilmiş, mobil uyumlu (responsive) ve şık arayüz.

---

## 🛠️ Kullanılan Teknolojiler

*   HTML5 & JavaScript (ES6+)
*   Tailwind CSS: Modern ve esnek arayüz tasarımı için.
*   Lucide Icons: SVG tabanlı dinamik arayüz ikonları için.
*   IndexedDB: Verilerin tarayıcı içinde SQL benzeri, yüksek performanslı ve kalıcı olarak saklanması için (Ana Veritabanı).
*   LocalStorage: Kullanıcının oturum durumunun (beni hatırla) yönetimi için.

---

## 📂 Veri Depolama Yapısı & Gizlilik

Bu uygulama %100 kullanıcı dostu gizlilik esasına göre tasarlanmıştır:
*   Girdiğiniz kullanıcı bilgileri, şifreler, maaşlar ve mesai kayıtları hiçbir uzak sunucuya veya bulut veritabanına gönderilmez.
*   Veriler, yalnızca kullandığınız cihazdaki tarayıcının IndexedDB alanında izole bir şekilde saklanır (Same-Origin Policy).
*   Tarayıcı geçmişini temizlerken "Çevrimdışı web sitesi verileri ve çerezler" seçeneğini silmediğiniz sürece verileriniz cihazınızda güvenle kalır.

---

## 🔒 Siber Güvenlik Notları

*   Avantajı: İnternet trafiği oluşturmadığı için ağ üzerinden veri çalınma (MITM) veya merkezi veri sızıntısı (data breach) riskleri barındırmaz.
*   Dikkat Edilmesi Gerekenler: Veriler yerel tarayıcıda düz metin (plain text) olarak saklandığından, ortak kullanılan bilgisayarlarda cihazınızı açık bırakmamanız önerilir. Tarayıcıyı tamamen izole etmek kişisel güvenliğiniz için yeterlidir.

---

## 🚀 Gelecek Planları (Roadmap)

*   [ ] Google Drive API Entegrasyonu: Verilerin kullanıcının kendi Google Drive hesabındaki gizli uygulama klasöründe yedeklenmesi ve cihazlar arası senkronizasyon (Bilgisayar, Telefon, Tablet).
*   [ ] Kriptografik Güvenlik: Şifrelerin SHA-256 ile hash'lenmesi ve hassas verilerin (maaş, mesai) tarayıcı içinde AES algoritmasıyla şifrelenerek IndexedDB'ye kaydedilmesi.
*   [ ] Gelişmiş Raporlama: Aylık ve yıllık mesai grafiklerinin görselleştirilmesi, verilerin Excel (XLSX) veya PDF olarak dışa aktarılabilmesi.

---

## 💻 Kurulum ve Çalıştırma

Uygulama herhangi bir kurulum gerektirmez. 
1. "index.html" dosyasını bilgisayarınıza indirin.
2. Dosyaya çift tıklayarak herhangi bir modern tarayıcıda (Chrome, Edge, Safari, Firefox) anında çalıştırın.

