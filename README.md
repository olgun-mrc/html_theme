# Modern One-Page Portfolio & Blog Teması

Modern, responsive ve etkileyici bir one-page HTML teması. Blog carousel, portfolio bölümü ve iletişim formu içerir.

## ✨ Özellikler

### Genel
- 🎨 Modern gradient tasarım ve animasyonlar
- 📱 Tam responsive (mobil, tablet, desktop)
- ⚡ Smooth scroll navigasyon
- 🎯 One-page tasarım
- 🚀 Vanilla JavaScript (bağımlılık yok)
- ♿ Semantic HTML5 yapısı

### Bölümler
- 🏠 **Hero Section** - Animasyonlu arka plan ve CTA butonları
- 👤 **About** - Kişisel bilgiler ve deneyimler
- 📝 **Blog Carousel** - Otomatik geçişli makale slider'ı
- 💼 **Portfolio** - Proje kartları grid sistemi
- 📧 **Contact** - İletişim formu
- 🔗 **Social Links** - Sosyal medya bağlantıları

### Teknik Özellikler
- Sticky navigation
- Auto-play carousel (5 saniye)
- Touch/swipe desteği (mobil)
- Klavye navigasyonu (ok tuşları)
- Scroll animasyonları
- Active nav link indicator
- Form validasyonu

## 📁 Dosya Yapısı

```
html_theme/
├── index.html          # One-page anasayfa
├── article1.html       # Örnek makale detay sayfası
├── style.css           # Tüm stiller ve animasyonlar
├── script.js           # JavaScript fonksiyonları
└── README.md          # Bu dosya
```

## 🚀 Kullanım

### Hızlı Başlangıç
1. Dosyaları bir web sunucusuna yükleyin veya doğrudan `index.html` dosyasını tarayıcıda açın
2. Kendi içeriğinizi eklemek için HTML dosyalarını düzenleyin
3. Renkleri ve stilleri `style.css` dosyasından özelleştirin

### İçerik Özelleştirme

#### Hero Section
`index.html` dosyasında hero section'ı bulun ve başlık, açıklama ve buton metinlerini değiştirin:
```html
<h1>Merhaba, Ben Bir Web Geliştiriciyim</h1>
<p>Teknoloji, yazılım ve yaratıcılık tutkusuyla projeler geliştiriyorum</p>
```

#### About Bölümü
About section'da kendi bilgilerinizi ekleyin:
```html
<div class="about-text">
    <h3>Kim ben?</h3>
    <p>Kendi açıklamanız...</p>
</div>
```

#### Blog Carousel
Yeni makale eklemek için carousel içine yeni bir carousel-item ekleyin:
```html
<div class="carousel-item">
    <div class="carousel-item-content">
        <div class="carousel-image">🎯</div>
        <div class="carousel-text">
            <h3>Makale Başlığı</h3>
            <div class="carousel-meta">
                <span>📅 Tarih</span> • <span>⏱️ Okuma süresi</span>
            </div>
            <p>Makale özeti...</p>
            <a href="#" class="btn btn-primary">Devamını Oku →</a>
        </div>
    </div>
</div>
```

#### Portfolio Projeleri
Yeni proje eklemek için portfolio-grid içine yeni bir portfolio-item ekleyin:
```html
<div class="portfolio-item">
    <div class="portfolio-image">🎨</div>
    <div class="portfolio-content">
        <h3>Proje Adı</h3>
        <div class="portfolio-tags">
            <span class="tag">Teknoloji 1</span>
            <span class="tag">Teknoloji 2</span>
        </div>
        <p>Proje açıklaması...</p>
    </div>
</div>
```

## 🎨 Renk Şeması Özelleştirme

`style.css` dosyasında aşağıdaki renkleri değiştirerek tema rengini özelleştirebilirsiniz:

```css
/* Ana gradient renkler */
#667eea /* Mavi-mor */
#764ba2 /* Mor */

/* Arka plan renkleri */
#f8f9fa /* Açık gri */
#ffffff /* Beyaz */

/* Metin renkleri */
#333    /* Koyu gri */
#555    /* Orta gri */
#666    /* Açık gri */
```

## 📱 Carousel Kullanımı

Carousel otomatik olarak çalışır, ancak kullanıcılar:
- ◀️ ▶️ butonlarına tıklayarak
- Klavyede ← → ok tuşlarını kullanarak
- Mobilde sağa/sola kaydırarak
- Alt kısımdaki indicator'lara tıklayarak

manuel olarak geçiş yapabilir.

### Carousel Ayarları
`script.js` dosyasında otomatik geçiş süresini değiştirebilirsiniz:
```javascript
// 5000ms = 5 saniye (varsayılan)
let autoPlayInterval = setInterval(nextSlide, 5000);
```

## 🌐 Tarayıcı Desteği

- ✅ Chrome (son 2 versiyon)
- ✅ Firefox (son 2 versiyon)
- ✅ Safari (son 2 versiyon)
- ✅ Edge (son 2 versiyon)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 İletişim Formu

İletişim formu şu anda sadece bir alert mesajı gösterir. Gerçek bir backend entegrasyonu için:

1. Form submit handler'ını `script.js` içinde bulun
2. Fetch API veya AJAX kullanarak backend'e istek gönderin
3. Örnek:
```javascript
contactForm.addEventListener('submit', async function(e) {
    e.preventDefault();
    const formData = new FormData(this);

    try {
        const response = await fetch('/api/contact', {
            method: 'POST',
            body: formData
        });
        // Handle response
    } catch (error) {
        // Handle error
    }
});
```

## 🛠️ Geliştirme

### Yeni Bölüm Ekleme
1. HTML'e yeni section ekleyin
2. Navigation menüsüne link ekleyin
3. CSS'te bölüm stillendirin
4. Gerekirse JavaScript fonksiyonları ekleyin

### Animasyon Ekleme
Intersection Observer API kullanılarak scroll animasyonları eklenmiştir. Yeni elementlere animasyon eklemek için `script.js` dosyasını inceleyin.

## 📄 Lisans

Bu tema özgürce kullanılabilir ve özelleştirilebilir.

## 🤝 Katkıda Bulunma

Önerileriniz ve katkılarınız için teşekkür ederiz!

---

**Not:** Bu tema vanilla HTML, CSS ve JavaScript ile yazılmıştır. Herhangi bir framework veya kütüphane gerektirmez.
