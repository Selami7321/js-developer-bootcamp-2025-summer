Responsive Ürün Vitrini Projesi - Teknik Dokümantasyon
🌟 Proje Özeti
Bu proje, modern CSS teknikleri kullanarak tamamen responsive bir ürün vitrini oluşturmayı hedeflemektedir. Hem desktop hem de mobil cihazlarda kusursuz çalışan bu vitrin, kullanıcı deneyimini ön planda tutarak estetik ve fonksiyonelliği bir araya getirmektedir.

Canlı Demo: Proje Önizlemesi

🛠️ Teknolojiler ve Teknikler
1. Responsive Grid Sistemi
css
.product-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 30px;
}
auto-fill ve minmax() fonksiyonları ile ekran boyutuna göre otomatik sütun ayarlama

Mobil uyumluluk için media query'ler:

css
@media (max-width: 1024px) { grid-template-columns: repeat(3, 1fr); }
@media (max-width: 768px) { grid-template-columns: repeat(2, 1fr); }
@media (max-width: 480px) { grid-template-columns: 1fr; }
2. Modern CSS Özellikleri
CSS Değişkenleri (Custom Properties):

css
:root {
  --primary: #3498db;
  --secondary: #2c3e50;
  --box-shadow: 0 10px 30px rgba(0,0,0,0.12);
  --transition: all 0.3s cubic-bezier(0.25,0.8,0.25,1);
}
clamp() Fonksiyonu: Responsive font boyutları

css
header h1 { font-size: clamp(2rem, 5vw, 3rem); }
backdrop-filter: Arka plan blur efekti

css
header { backdrop-filter: blur(10px); }
3. İnteraktif Öğeler ve Animasyonlar
Ürün Kartı Hover Efekti:

css
.product-card:hover {
  transform: translateY(-10px) rotateY(5deg);
  box-shadow: 0 20px 40px rgba(0,0,0,0.2);
}
Pulsating Animasyon (Nabız Efekti):

css
@keyframes pulse {
  0% { box-shadow: 0 0 0 0 rgba(231,76,60,0.7); }
  70% { box-shadow: 0 0 0 10px rgba(231,76,60,0); }
  100% { box-shadow: 0 0 0 0 rgba(231,76,60,0); }
}
.badge { animation: pulse 2s infinite; }
4. Flexbox ile Gelişmiş Düzenleme
css
.product-info {
  display: flex;
  flex-direction: column;
  flex-grow: 1; /* Kart içeriğini genişletme */
}

.product-actions {
  margin-top: auto; /* Butonları her zaman alta sabitleme */
}
5. JavaScript Entegrasyonu
Sepete Ekleme Animasyonu:

javascript
button.addEventListener('click', function() {
  this.innerHTML = '<i class="fas fa-check"></i> Eklendi';
  this.classList.add('added');
});
Favori Butonu Etkileşimi:

javascript
wishlistBtn.addEventListener('click', function() {
  this.classList.toggle('active');
});
✨ Temel Özellikler
Tam Responsive Tasarım

Mobil (480px altı): Tek sütun

Tablet (768px altı): İki sütun

Desktop (1024px üstü): Üç sütun

Ürün Filtreleme ve Sıralama

Kategoriye göre filtreleme

Fiyata göre artan/azalan sıralama

İnteraktif UI Elementleri

Sepete ekle butonu animasyonları

Favorilere ekleme özelliği

Ürün rozetleri (Tükendi, Sınırlı Stok)

Performans Optimizasyonu

CSS değişkenleri ile kolay tema yönetimi

Hardware accelerated animasyonlar

Optimize edilmiş görseller

🚀 Kurulum ve Kullanım
Projeyi klonlayın:

bash
git clone https://github.com/Selami7321/js-developer-bootcamp-2025-summer/tree/main
Proje dizinine gidin:

bash
cd responsive-urun-vitrini
Tarayıcıda açın:

bash
# Windows
start index.html

# macOS
open index.html

# Linux
xdg-open index.html
🌐 Canlı Demo
Projenin canlı versiyonuna GitHub Pages üzerinden erişebilirsiniz:
Canlı Demo

📸 Ekran Görüntüleri
https://github.com/Selami7321/js-developer-bootcamp-2025-summer/tree/main  Repo adresimde bulabilirsiniz

📌 Öne Çıkan Gelişmiş CSS Teknikleri
3D Transform Efektleri

css
.product-card {
  transform-style: preserve-3d;
  perspective: 1000px;
}
.product-card:hover {
  transform: translateY(-10px) rotateY(5deg);
}
CSS Grid ile Dinamik Izgara

css
.features {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
}
Animasyonlu Bildirim Sistemi

javascript
// CSS
.notification {
  transition: opacity 0.3s, bottom 0.3s;
}

// JavaScript
notification.style.opacity = '1';
notification.style.bottom = '30px';
Kademeli Geliştirme (Progressive Enhancement)

Modern tarayıcılarda gelişmiş efektler

Eski tarayıcılarda temel fonksiyonelliğin korunması

💡 Öğrenilen Önemli Konular
CSS Grid ve Flexbox'un birlikte kullanımı

Responsive tasarımda clamp() fonksiyonu

CSS değişkenleri ile tema yönetimi

Transform ve transition kullanarak performanslı animasyonlar

JavaScript ile CSS arasındaki etkileşim

Mobil-first tasarım prensipleri

Erişilebilirlik (accessibility) temelleri

📚 Kaynaklar
CSS Grid Complete Guide

Flexbox Froggy

CSS Variables Guide

Animations in CSS

Bu proje, modern web geliştirme tekniklerinin bir sentezi olarak hem görsel açıdan etkileyici hem de teknik açıdan sağlam bir çözüm sunmaktadır. Tüm kodlar MIT lisansı altında açık kaynak olarak paylaşılmıştır.
