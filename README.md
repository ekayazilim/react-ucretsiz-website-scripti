# EKA Yazılım - Ücretsiz Website Scripti

Bu proje, **EKA Yazılım** tarafından geliştirilen ve işletmelerin dijital dönüşümüne katkıda bulunmak için ücretsiz olarak sunulan bir web sitesi scriptidir. Modern teknolojilerle hazırlanmış bu script, hem şık bir arayüz hem de kolay kurulum sunar.

![EKA Yazılım](https://github.com/ekayazilim/react-ucretsiz-website-scripti/blob/main/all-devices-white.png)

---

## **Video Tanıtımı**
Kurulum ve kullanım talimatları için YouTube videomuzu izleyebilirsiniz:
[![EKA Yazılım Kurulum Videosu](https://img.youtube.com/vi/pR1Gjn96SPg/0.jpg)](https://youtu.be/pR1Gjn96SPg)

---

## **Özellikler**
- **Modern Arayüz**: Mobil uyumlu (responsive) ve şık bir tasarım.
- **Kolay Kurulum**: Basit adımlarla hosting veya yerel bilgisayara kurulabilir.
- **İletişim Formu**: SMTP entegrasyonu ile doğrudan e-posta gönderimi.
- **Google Harita Entegrasyonu**: Ofis konumunu kullanıcılarla paylaşın.
- **Hizmetlerimiz Bölümü**: Şirketinizin sunduğu hizmetleri detaylıca tanıtın.

---

## **Kurulum**

Bu projeyi hem yerel bilgisayarınıza hem de hosting kontrol panelinize kurabilirsiniz.

### **1. Dosyaları İndirin**
- GitHub üzerinden [**eka-kurumsalv0.zip**](https://github.com/ekayazilim/react-ucretsiz-website-scripti/blob/main/all-devices-white.png) dosyasını indirin.

---

### **2. Hosting Üzerinde Kurulum**

1. Hosting kontrol panelinize (cPanel, Plesk vb.) giriş yapın.
2. **Dosya Yöneticisi**ne gidin ve `public_html` dizinine giriş yapın.
3. `eka-kurumsalv0.zip` dosyasını yükleyin.
4. ZIP dosyasını "Extract" (Çıkart) seçeneği ile açın.
5. Tarayıcınızda alan adınızı açarak projenin çalışıp çalışmadığını kontrol edin.

#### **Not:**
Eğer kurulum sırasında hata alırsanız:
- Hosting sağlayıcınızın **PHP 7.4 veya üzeri** desteklediğinden emin olun.
- Node.js bağımlılıklarını eksiksiz kurduğunuzdan emin olun.

---

### **3. Yerel Bilgisayarda Kurulum**

1. [Node.js](https://nodejs.org/) ve npm'in yüklü olduğundan emin olun.
2. Proje klasörüne gidin:
   ```bash
   cd eka-kurumsal
   ```
3. Gerekli bağımlılıkları yükleyin:
   ```bash
   npm install
   ```
4. Projeyi geliştirme modunda başlatmak için:
   ```bash
   npm start
   ```
5. Tarayıcınızda `http://localhost:3000` adresine giderek projeyi görüntüleyin.

#### **Derleme (Build)**
Eğer projeyi hostingde yayınlamak istiyorsanız:
```bash
npm run build
```
Bu işlemden sonra oluşan `build` veya `dist` klasörünü hosting kontrol panelinize yükleyin.

---

## **E-posta Gönderimi (SMTP)**

İletişim formunun çalışması için şu adımları izleyin:

1. `sendMail.php` dosyasını `public_html` dizinine yükleyin.
2. SMTP bilgilerinizi `sendMail.php` içinde güncelleyin:
   ```php
   $mail->Host = 'mail.ekasunucu.org';
   $mail->Username = 'info@ekabilisim.com';
   $mail->Password = 'ym?0+$+0}F+M';
   $mail->addAddress('ekasunucu@gmail.com');
   ```

E-posta gönderimi için hostinginizin **SMTP** desteğinin aktif olduğundan emin olun.

---

## **İletişim**

### **Firma Bilgileri**
- **Telefon**: 0 (850) 307 34 58
- **Faks**: 0 (212) 993 34 58
- **E-posta**: [info@ekayazilim.com.tr](mailto:info@ekayazilim.com.tr)
- **Adres**: Halkalı Merkez, Fatih Cd. Özgür Apartmanı No: 45 İç Kapı No: 3, 34303 Küçükçekmece/İstanbul

### **Sosyal Medya**
- [Facebook](https://www.facebook.com/ekayazilim)
- [Twitter](https://twitter.com/ekayazilim)
- [LinkedIn](https://www.linkedin.com/company/eka-software-limited/)
- [Instagram](https://www.instagram.com/ekayazilim.com.tr/)
- [YouTube](https://www.youtube.com/@ekayazilim)

---

## **Karşılaşılabilecek Sorunlar ve Çözümleri**

### **1. ZIP Dosyası Çıkartılamıyor**
Eğer hostingde ZIP dosyasını çıkartırken hata alıyorsanız:
- ZIP dosyasını bilgisayarınızda çıkartın ve `public_html` dizinine manuel olarak yükleyin.

### **2. `npm install` Hatası**
Yerel bilgisayarda bağımlılıkları yüklerken hata alırsanız:
```bash
npm install --force
```

### **3. İletişim Formu Çalışmıyor**
- SMTP ayarlarını `sendMail.php` dosyasında doğru yapılandırın.
- Hosting sağlayıcınızın PHP `mail()` fonksiyonunu desteklediğinden emin olun.

---

## **Klasör Yapısı**

```
/public_html
    ├── /assets             # Statik dosyalar (CSS, JS, resimler)
    ├── /php                # PHP dosyaları (sendMail.php vb.)
    ├── /src                # React bileşenleri
    ├── index.html          # Ana dosya
    └── sendMail.php        # E-posta gönderim dosyası
```

---

## **Katkı**
Proje tamamen açık kaynaklıdır. Katkıda bulunmak isterseniz **Pull Request** gönderebilirsiniz.

---

## **Lisans**
Bu proje [MIT Lisansı](LICENSE) ile lisanslanmıştır.

