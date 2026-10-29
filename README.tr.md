<div align="center">

# 🎮 FiveLive Roleplay — Web Platformu

**FiveM roleplay topluluğu için geliştirilmiş, framework kullanmayan, tam kapsamlı web platformu.**

[![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-8.x-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Status](https://img.shields.io/badge/Durum-YAKINDA%20YAYINDA-orange?style=for-the-badge)]()

[💬 Discord](https://discord.gg/T6fH3KNDqC)

</div>

---

## 📖 Proje Hakkında

Bu depo, bir FiveM roleplay topluluğu için sıfırdan geliştirilmiş **tam kapsamlı web platformunun** kaynak kodlarını barındırır.

İçinde **tanıtım sitesi**, **forum**, **wiki (bilgi bankası)**, **başvuru formları**, **yönetim paneli** ve **ödeme entegrasyonu** gibi bir topluluğun ihtiyaç duyduğu her şey tek bir çatı altında toplanmıştır.

Proje **herhangi bir framework kullanılmadan**, saf PHP + HTML + CSS + JavaScript ile geliştirilmiştir. Hafif yapısı sayesinde paylaşımlı hosting dahil her ortamda ek yapılandırma gerektirmeden çalışır.

### Öne Çıkanlar

- ⚡ **Hafif ve Hızlı** — Ağır framework/kütüphane yok, sadece ihtiyaç duyulan kod.
- 🔐 **Güvenlik Odaklı** — CSRF, rate limit, HMAC imza, XSS sanitizer, SSRF koruması, session fixation koruması.
- 🎨 **Çoklu Tema** — Birden fazla tema; yönetim panelinden dinamik olarak yönetilebilir.
- 🌍 **Çift Dil Desteği** — Türkçe / İngilizce (`/tr`, `/en`).
- 📱 **Tamamen Duyarlı (Responsive)** — Telefon, tablet ve masaüstünde kusursuz görünüm.
- 🧩 **Modüler Yapı** — Router + template sistemi ile kolay genişletilebilir.
- 💳 **Güvenli Ödeme Akışı** — Webhook doğrulama, otomatik kredi yükleme.
- 🎮 **Discord OAuth** — Discord ile giriş, rol bazlı yetkilendirme.

---

## ✨ Özellikler

### 🌐 Genel Site

| Bölüm | Açıklama |
|-------|----------|
| **🏠 Ana Sayfa** | Tanıtım, öne çıkan özellikler, canlı sayaç |
| **📰 Haberler** | Dinamik haber listesi, sayfalama, detay sayfası |
| **📖 Wiki (Bilgi Bankası)** | Kategori + makale yapısı, arama, görüntülenme sayacı |
| **🤝 Başvuru Formu** | AJAX tabanlı form, Discord webhook bildirimi |
| **🎁 Ödeme Sayfası** | Paket satın alma akışı |
| **📄 Yasal Sayfalar** | Gizlilik Politikası, Kullanıcı Sözleşmesi, İade Politikası |
| **🎬 Başlangıç Rehberi** | Adım adım rehber, video, SSS |
| **❓ SSS** | Sık sorulan sorular ve yanıtları |
| **🔗 Dinamik Sayfalar** | Yönetim panelden oluşturulan özel sayfalar |
| **📱 Mobil Menü** | Küçük ekranlarda tam işlevsel hamburger menü |

### 👥 Forum Sistemi

| Özellik | Açıklama |
|---------|----------|
| **Kategori Yönetimi** | Sonsuz derinlikte alt kategoriler, sıralama, bölüm grupları |
| **Konu (Topic)** | Açma, düzenleme, silme, pinleme, kilitleme, durum değiştirme, taşıma |
| **Yanıt (Reply)** | Zengin metin editörü, resim yükleme, alıntı, düzenleme, silme |
| **Toplu İşlem** | Konu seç + toplu taşı / durum değiştir / yanıtla / kilitle / pinle / sil |
| **Bildirimler** | Anlık bildirimler, okundu işaretleme, dropdown panel |
| **Çöp Kutusu** | Silinen konu/yanıt/kategorileri geri getirme |
| **Kategori İzinleri** | Rol bazlı görüntüleme, yazma, konu açma, kilitleme, taşıma vb. |
| **Genel Yetki Matrisi** | Panel menüsü + aksiyon bazlı rol yetkileri |

### 🛡️ Yönetim Paneli

| Modül | Açıklama |
|-------|----------|
| **Genel Bakış** | Toplam konu/kullanıcı, hızlı işlemler, tema yönetimi |
| **Kategoriler** | Oluşturma, düzenleme, silme, sıralama |
| **Ceza Yönetimi** | Ban / Mute verme, süre, IP bazlı ban |
| **Kullanıcı Yönetimi** | Detaylı filtreleme, rol verme, oturum sonlandırma, bilgi yenileme |
| **Kategori İzinleri** | Rol × kategori yetki matrisi, izin kopyalama |
| **Genel Yetki Matrisi** | Rol bazlı menü/aksiyon yetkileri |
| **Sıralama Yönetimi** | Konu sayısı yarışı, haftalık snapshot geçmişi |
| **Çöp Kutusu** | Silinen öğeleri geri getirme |
| **Tema İstatistikleri** | Tema kullanım dağılımı, yüzdelik oranlar |
| **Panel Erişim Rolleri** | Rol bazlı panel erişimi + bireysel kullanıcı override |
| **Aktif Kullanıcılar** | Son 5 dakikada aktif olan kullanıcılar |
| **Token Durumu** | Discord token expire durumları |
| **Rate Limit İhlalleri** | Aktif rate limit kayıtları |
| **Oturum Yönetimi** | Son giriş yapanlar, oturum sonlandırma |
| **Görsel Kotası** | Kullanıcı başına disk kullanımı |
| **Action Logs** | Log kod sayaçları |
| **Anonim Görüntülenmeler** | IP bazlı anonim view istatistikleri |
| **IP Ban Listesi** | IP bazlı ban cezaları |
| **Settings Viewer** | Tüm site ayarlarını görüntüleme/düzenleme |
| **Hata Logu** | Son PHP error_log satırları |
| **Güvenlik Logları** | Güvenlik olayları kaydı |

### 💳 Ödeme Entegrasyonu

| Özellik | Açıklama |
|---------|----------|
| **Ürün Yönetimi** | Ürün ekleme, düzenleme, silme, aktif/pasif |
| **Güvenli Oturum** | HMAC-SHA256 imzası ile token oluşturma |
| **Webhook Doğrulama** | HMAC imza kontrolü, status güncelleme |
| **Çarpan Kampanyası** | Otomatik hesaplama ile bonus çarpanı |
| **Happy Hour** | Yüzdelik bonus kampanyası |
| **Sipariş Yönetimi** | Sipariş listesi, kredi işaretleme, silme |
| **Oyun Sunucusu Callback** | Oyun sunucusuna kredi bildirimi |
| **Log Sistemi** | Tüm istek/yanıtlar detaylı loglanır |

### 🎨 Tema Sistemi

| Tema | Klasör |
|------|--------|
| **Ana Tema** | `maintheme` |
| **Altın Obsidyen** | `goldobsidian` |
| **Galaksi** | `galaxy` |
| **Kış** | `winter` |
| **Obsidian Premium** | `obsidianpremium` |

- Yönetim panelden **seçicide gösterilecek temalar** ayarlanabilir.
- **Varsayılan tema** belirlenebilir.
- **Zorla tema (Force)** — Tüm ziyaretçilere zorunlu tema.
- **Bireysel kullanıcı teması** — Kilitleme seçeneğiyle.
- **Tüm kullanıcılara uygula** — Anonim ziyaretçiler dahil.

---

## 🛠️ Teknolojiler

<div align="center">

| Katman | Teknoloji |
|--------|-----------|
| **Backend** | PHP 8.x (saf, framework yok) |
| **Veritabanı** | MySQL 8.x / MariaDB (PDO) |
| **Frontend** | HTML5, CSS3 (Flexbox, Grid, Custom Properties), Vanilla JS (ES6+) |
| **Kimlik Doğrulama** | Discord OAuth2 |
| **Görsel İşleme** | GD Library |
| **HTML Sanitizer** | HTMLPurifier (opsiyonel) |
| **İkonlar** | Inline SVG |
| **Yazı Tipleri** | Google Fonts (Inter / Poppins / HCo Gotham) |

</div>

> Proje herhangi bir build aracı, paket yöneticisi veya frontend framework gerektirmez.

---

## 📁 Proje Yapısı

```text
fivelive-site/
│
├── index.php                   # Ana router + API dispatcher
├── router.php                  # URL yönlendirici
├── dodopin_webhook.php         # Ödeme webhook handler
├── ingame_callback.php         # Oyun sunucusu kredi callback
├── .env                        # Ortam değişkenleri
│
├── templates/                  # HTML şablonları
│   ├── index2.html             # Ana sayfa
│   ├── news.html               # Haberler
│   ├── article.html            # Haber detay
│   ├── category_detail.html    # Kategori detay
│   ├── topic_detail.html       # Konu detay
│   ├── new_topic.html          # Yeni konu
│   ├── profile.html            # Profil
│   ├── wiki.html               # Wiki ana sayfa
│   ├── wiki_category.html      # Wiki kategori
│   ├── wiki_article.html       # Wiki makale
│   ├── partnership.html        # Başvuru formu
│   ├── donate.html             # Ödeme sayfası
│   ├── howtoplay.html          # Başlangıç rehberi
│   ├── policy.html             # Gizlilik politikası
│   ├── contract.html           # Kullanıcı sözleşmesi
│   ├── chargeback.html         # İade politikası
│   ├── notifications.html      # Bildirimler
│   ├── maintenance.html        # Bakım modu
│   ├── 404.html                # 404 sayfası
│   ├── admin_login.html        # Admin giriş
│   └── admin_dashboard.html    # Yönetim paneli
│
├── static/
│   ├── css/
│   │   ├── maintheme/
│   │   ├── goldobsidian/
│   │   ├── galaxy/
│   │   ├── winter/
│   │   └── obsidianpremium/
│   ├── js/
│   └── uploads/                # Kullanıcı görselleri
│
└── vendor/                     # Composer bağımlılıkları (opsiyonel)
```

---

## 🔒 Güvenlik Özellikleri

Platform, üretim ortamında çalışacak şekilde güvenlik odaklı geliştirilmiştir:

| Kategori | Koruma |
|----------|--------|
| **CSRF** | Tüm POST isteklerinde token doğrulaması |
| **XSS** | HTMLPurifier + dahili sanitizer (beyaz liste) |
| **SQL Injection** | Tüm sorgular PDO prepared statement |
| **Session Fixation** | `session_regenerate_id()` + UA hash + süre kontrolü |
| **Rate Limit** | Session + IP + dosya bazlı çok katmanlı limit |
| **Brute Force** | Deneme limiti + hesap kilitleme |
| **SSRF** | Webhook URL'lerinde host kontrolü, private IP engeli |
| **Log Injection** | Kontrol karakterleri temizlenir |
| **Path Traversal** | Statik dosya yolu `realpath()` ile sınırlandırılır |
| **DoS** | POST boyut limiti, görsel boyut limiti |
| **Clickjacking** | `X-Frame-Options: SAMEORIGIN` |
| **MIME Sniffing** | `X-Content-Type-Options: nosniff` |
| **Webhook Güvenliği** | Sadece izinli domainlere istek atılır |
| **HMAC** | Ödeme ve oyun callback imza doğrulaması |

---

## 🗺️ Yol Haritası

- [x] Ana sayfa + haberler
- [x] Forum sistemi (konu/yanıt)
- [x] Wiki (kategori + makale)
- [x] Yönetim paneli
- [x] Discord OAuth
- [x] Çoklu tema sistemi
- [x] Ödeme entegrasyonu
- [x] Toplu işlemler
- [x] Çöp kutusu
- [x] Bildirim sistemi
- [ ] REST API genişletmesi
- [ ] PWA desteği
- [ ] Ek dil desteği
- [ ] Real-time chat (WebSocket)

---

## 🤝 Katkıda Bulunma

Bu proje bir topluluk projesidir. Katkılarınız memnuniyetle karşılanır!

- 🐛 **Hata bulduysanız** — Issue açın veya doğrudan Discord üzerinden bildirin.
- 💡 **Fikriniz varsa** — Issue açarak önerinizi paylaşın.
- 🛠️ **Katkı sağlamak istiyorsanız** — Büyük değişiklikler için önce bir issue açarak tartışın.
- 🔐 **Güvenlik açığı tespit ettiyseniz** — Lütfen herkese açık issue açmayın; doğrudan Discord üzerinden iletişime geçin.

---

## 🙏 Teşekkürler

- **HTMLPurifier**, **Discord API** — Sağladıkları altyapı için.

---

## 📬 İletişim

- **Discord:** [discord.gg/T6fH3KNDqC](https://discord.gg/T6fH3KNDqC)

---

<div align="center">

**FiveLive Roleplay Web Platformu**

[![Discord](https://img.shields.io/badge/Discord-Katıl-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/T6fH3KNDqC)

<sub>Bu README, projenin kendisini tanıtmak için hazırlanmıştır. ❤️</sub>

</div>
