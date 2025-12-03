# AutoDock 4 Moleküler Docking Rehberi

Modern, interaktif ve kapsamlı AutoDock 4 tutoriali - Protein hazırlamadan validasyona kadar eksiksiz Türkçe rehber.

## 🚀 GitHub Pages'de Yayınlama - Adım Adım Rehber

### Ön Gereksinimler
- GitHub hesabı
- Git kurulumu (bilgisayarınızda)

### Adım 1: GitHub Repository Oluşturma

1. GitHub'da oturum açın: https://github.com
2. Sağ üst köşeden **"+"** işaretine tıklayın → **"New repository"**
3. Repository ayarları:
   - **Repository name**: `autodock-tutorial` (veya istediğiniz isim)
   - **Description**: "AutoDock 4 Moleküler Docking - Türkçe Rehber"
   - **Public** seçin (GitHub Pages için gerekli)
   - ✅ **Add a README file** - İŞARETLEMEYİN (zaten var)
   - **Create repository** butonuna tıklayın

### Adım 2: Dosyaları Repository'ye Yükleme

#### Yöntem A: Web Arayüzü ile (Kolay)

1. Oluşturduğunuz repository'de **"uploading an existing file"** linkine tıklayın
2. Bu projedeki tüm dosyaları sürükleyip bırakın:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `README.md`
3. Commit message yazın: "Initial commit - AutoDock tutorial"
4. **"Commit changes"** butonuna tıklayın

#### Yöntem B: Git ile (Terminal/Command Prompt)

```bash
# 1. Proje klasörüne gidin (dosyaların olduğu klasör)
cd /path/to/autodock-website

# 2. Git repository'yi başlatın
git init

# 3. Tüm dosyaları ekleyin
git add .

# 4. İlk commit'i yapın
git commit -m "Initial commit - AutoDock 4 tutorial"

# 5. GitHub repository'nizi remote olarak ekleyin
# (YOUR-USERNAME yerine GitHub kullanıcı adınızı yazın)
git remote add origin https://github.com/YOUR-USERNAME/autodock-tutorial.git

# 6. Ana branch'ı main olarak ayarlayın
git branch -M main

# 7. Dosyaları GitHub'a gönderin
git push -u origin main
```

### Adım 3: GitHub Pages'i Aktifleştirme

1. Repository sayfanızda üst menüden **"Settings"** sekmesine gidin
2. Sol menüden **"Pages"** bölümünü bulun ve tıklayın
3. **"Source"** kısmında:
   - Branch: **main** seçin
   - Folder: **/ (root)** seçin
4. **"Save"** butonuna tıklayın
5. ⏳ Birkaç dakika bekleyin (1-5 dakika)
6. ✅ Sayfa yenilediğinizde yeşil bir kutu ile sitenizin URL'sini göreceksiniz:
   - `https://YOUR-USERNAME.github.io/autodock-tutorial/`

### Adım 4: Sitenizi Ziyaret Edin

Tarayıcınızda şu URL'yi açın:
```
https://YOUR-USERNAME.github.io/autodock-tutorial/
```

🎉 **Tebrikler!** AutoDock tutorial siteniz artık yayında!

---

## 📝 Güncelleme Yapma

Sitede değişiklik yapmak isterseniz:

### Web Arayüzü ile:
1. GitHub repository'de değiştirmek istediğiniz dosyayı açın
2. Sağ üstteki kalem ikonuna (✏️ Edit) tıklayın
3. Değişiklikleri yapın
4. Altta "Commit changes" ile kaydedin
5. ⏳ 1-2 dakika bekleyin, değişiklikler otomatik yayınlanacak

### Git ile:
```bash
# Değişikliklerinizi yapın (index.html, styles.css, vb.)

# Değişiklikleri ekleyin
git add .

# Commit yapın
git commit -m "Açıklama mesajınız"

# GitHub'a gönderin
git push origin main
```

---

## 🎨 Özelleştirme

### Renk Paletini Değiştirme

`styles.css` dosyasında `:root` bölümündeki renk değişkenlerini düzenleyin:

```css
:root {
    --primary: #1e3a8a;      /* Ana renk */
    --secondary: #f59e0b;    /* İkincil renk */
    --accent: #10b981;       /* Vurgu rengi */
    /* ... diğer renkler */
}
```

### Logo ve Başlık

`index.html` dosyasında `<nav>` bölümünü düzenleyin:

```html
<div class="nav-brand">
    <span class="logo">AD4</span>  <!-- Kısaltmayı değiştirin -->
    <span class="brand-text">AutoDock 4 Rehberi</span>  <!-- Başlığı değiştirin -->
</div>
```

### İçerik Güncelleme

Her bölüm `<section id="..." class="section">` etiketi içindedir. İlgili bölümü bulup düzenleyin.

---

## 📁 Proje Yapısı

```
autodock-tutorial/
│
├── index.html          # Ana sayfa (tüm içerik)
├── styles.css          # Stil dosyası (tasarım)
├── script.js           # JavaScript (interaktivite)
└── README.md           # Bu dosya (deployment talimatları)
```

---

## 🌟 Özellikler

- ✅ **Responsive Design**: Mobil, tablet ve desktop uyumlu
- ✅ **Modern Tasarım**: Bilimsel estetik, profesyonel görünüm
- ✅ **Interaktif Navigasyon**: Smooth scroll, aktif bölüm vurgulama
- ✅ **Kod Kopyalama**: Kod bloklarında tek tıkla kopyalama
- ✅ **Sekme Sistemi**: Terminal komutları için Windows/Unix seçenekleri
- ✅ **Baskıya Uygun**: PDF olarak kaydetme desteği
- ✅ **SEO Optimizasyonu**: Meta etiketleri ve semantic HTML
- ✅ **Hızlı Yükleme**: Minimal bağımlılık, optimize edilmiş kod

---

## 🔧 Gelişmiş Özelleştirme

### Özel Domain Ekleme

1. GitHub repository → Settings → Pages
2. "Custom domain" alanına domain'inizi yazın (örn: `autodock.example.com`)
3. DNS sağlayıcınızda CNAME kaydı oluşturun:
   ```
   CNAME -> YOUR-USERNAME.github.io
   ```

### Google Analytics Ekleme

`index.html` dosyasının `<head>` bölümüne ekleyin:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### Sosyal Medya Meta Etiketleri

`<head>` bölümüne ekleyin:

```html
<!-- Open Graph / Facebook -->
<meta property="og:type" content="website">
<meta property="og:url" content="https://YOUR-USERNAME.github.io/autodock-tutorial/">
<meta property="og:title" content="AutoDock 4 Moleküler Docking Rehberi">
<meta property="og:description" content="Eksiksiz Türkçe AutoDock 4 tutoriali">
<meta property="og:image" content="https://YOUR-USERNAME.github.io/autodock-tutorial/preview.png">

<!-- Twitter -->
<meta property="twitter:card" content="summary_large_image">
<meta property="twitter:url" content="https://YOUR-USERNAME.github.io/autodock-tutorial/">
<meta property="twitter:title" content="AutoDock 4 Moleküler Docking Rehberi">
<meta property="twitter:description" content="Eksiksiz Türkçe AutoDock 4 tutoriali">
<meta property="twitter:image" content="https://YOUR-USERNAME.github.io/autodock-tutorial/preview.png">
```

---

## 🐛 Sorun Giderme

### Site görünmüyor / 404 hatası

**Çözüm:**
- GitHub Pages'in aktif olduğunu kontrol edin (Settings → Pages)
- Branch'in "main" ve root "/" olduğunu doğrulayın
- URL'yi doğru yazdığınızdan emin olun
- 5-10 dakika bekleyin (ilk deployment biraz sürebilir)

### Değişiklikler yansımıyor

**Çözüm:**
- Tarayıcı cache'ini temizleyin (Ctrl+Shift+Delete)
- Gizli pencerede açın (Ctrl+Shift+N)
- 2-3 dakika bekleyin (GitHub Pages güncelleme süresi)
- Hard refresh yapın (Ctrl+F5)

### CSS/JavaScript yüklenmiyor

**Çözüm:**
- Dosya isimlerinin tamamen küçük harf olduğunu kontrol edin
- Dosya uzantılarını doğrulayın (.css, .js)
- Tarayıcı konsolunu açın (F12) ve hataları kontrol edin

---

## 📚 Ek Kaynaklar

- [GitHub Pages Dokümantasyonu](https://docs.github.com/en/pages)
- [Git Temel Komutlar](https://git-scm.com/docs)
- [AutoDock Resmi Site](http://autodock.scripps.edu/)
- [Markdown Syntax](https://www.markdownguide.org/)

---

## 📄 Lisans

Bu proje eğitim ve araştırma amaçlıdır. Özgürce kullanabilir, değiştirebilir ve paylaşabilirsiniz.

---

## 🤝 Katkıda Bulunma

Hata bulursanız veya iyileştirme önerileriniz varsa:

1. Repository'yi fork edin
2. Yeni bir branch oluşturun (`git checkout -b feature/iyilestirme`)
3. Değişikliklerinizi commit edin (`git commit -m 'İyileştirme açıklaması'`)
4. Branch'inizi push edin (`git push origin feature/iyilestirme`)
5. Pull Request açın

---

## 📧 İletişim

Sorularınız için GitHub Issues kullanabilirsiniz.

---

## ✨ Önemli Notlar

- **Public repository olmalı**: GitHub Pages ücretsiz kullanımı için repository public olmalıdır
- **index.html zorunlu**: Ana sayfa mutlaka `index.html` olarak adlandırılmalıdır
- **Dosya boyutu**: Tek dosya 100 MB'dan küçük olmalıdır
- **Repository boyutu**: Toplam 1 GB'dan küçük olmalıdır
- **Bant genişliği**: Ayda 100 GB soft limit vardır

---

**Son güncelleme:** 2024  
**Hazırlayan:** AutoDock Tutorial Project  
**Teknoloji:** HTML5, CSS3, JavaScript (Vanilla)
