# Proje: Global E-Ticaret Satış Performansı Analizi ve İnteraktif Dashboard'u

Bu projede, Kaggle'ın "Global Superstore" e-ticaret veri seti kullanılarak Microsoft Power BI üzerinde interaktif bir satış performansı dashboard'u geliştirilmiştir.Projenin temel amacı, şirketin satış trendlerini, coğrafi pazar gücünü ve müşteri segmentasyonunu analiz ederek veri odaklı kararlar alınmasını sağlamaktır.

---

## 📊 Dashboard

![Dashboard Görüntüsü](superstore-dashboard.png)

---

## 🎯 Projenin Amacı
* Şirketin 2015-2018 yılları arasındaki genel satış performansını zaman içinde izlemek.
* En çok ve en az satan ürün alt kategorilerini belirlemek.
* Satışların coğrafi dağılımını analiz ederek en güçlü pazarları tespit etmek.
* Müşteri segmentlerinin satışlara olan katkısını anlamak.
* Tüm bu analizleri tek bir interaktif raporda birleştirmek.

---

## 🛠️ Kullanılan Teknolojiler

* **Microsoft Power BI Desktop**
* **Power Query (ETL için)** 
* **DAX (Veri Analizi İfadeleri)** 

---

## ⚙️ Proje Süreci

1.  **Veri Hazırlığı (ETL):** Ham veri Power Query ortamında temizlenmiş, veri tipleri dönüştürülmüş ve sipariş ile teslimat tarihleri arasındaki farkı hesaplayan "Teslimat Süresi" adında yeni bir sütun oluşturulmuştur.
2.  **KPI Geliştirme (DAX):** `Toplam Satış`, `Sipariş Sayısı` ve `Ortalama Teslimat Süresi` gibi temel performans göstergeleri, DAX ölçüleri (measures) olarak dinamik bir şekilde hesaplanmıştır.
3.  **Görselleştirme ve Rapor Tasarımı:** KPI kartları, zaman serisi için çizgi grafik, kategorik sıralama için çubuk grafik ve coğrafi dağılım için harita gibi çeşitli görseller kullanılarak interaktif bir dashboard tasarlanmıştır.

---

## 🔍 Temel Bulgular ve En Kritik Çıkarım

* Şirket satışları 2015-2018 yılları arasında istikrarlı bir artış trendi göstermektedir.
* Satışların büyük bir kısmı **California** ve **New York** eyaletlerindeki **"Consumer" (Bireysel Tüketici)** segmentinden gelmektedir.
* **KRİTİK VERİ HATASI:** Analiz sırasında, "Ortalama Teslimat Süresi" metriğinin **negatif (-4.0 gün)** olduğu tespit edilmiştir. Bu anormallik, kaynak veride sipariş tarihlerinin teslimat tarihlerinden sonra girildiği ciddi bir veri kalitesi sorununa işaret etmektedir.

---
## 💡 Stratejik Öneriler
* **Acil Eylem:** Tespit edilen negatif teslimat süresi anormalliğinin kök nedenini araştırmak üzere acil bir veri denetimi süreci başlatılmalıdır.
* **Pazarlama Odağı:** Pazarlama kampanyaları, en güçlü pazarlar olan California ve New York'taki bireysel tüketicilere yönlendirilebilir.
