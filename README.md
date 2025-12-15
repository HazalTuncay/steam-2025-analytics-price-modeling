# 🎮 Steam 2025 – Pazar Analizi ve Oyun Fiyat Tahmini
**Python • BigQuery • dbt Cloud • Looker Studio**

---

## Projeye Genel Bakış

Bu çalışma Team 6 tarafından, **Steam 2025 veri seti (240.000+ oyun)** üzerinden oyun pazarının yapısını inceleyen ve oyunların teknik/kategorik özelliklerine dayanarak **piyasa fiyatı tahmini** yapan kapsamlı bir veri analizi ve makine öğrenmesi projesidir.

Proje boyunca hem **veri mühendisliği** hem de **veri bilimi** perspektifiyle uçtan uca (End-to-End) bir analiz süreci yürütülmüştür.

---

## Amaç ve Kapsam

Bu projenin temel amacı:

- Oyun pazarındaki **fiyatlandırma dinamiklerini** anlamak  
- Zaman içinde oluşan **pazar trendlerini** ortaya koymak  
- Oyunlara ait teknik özellikleri kullanarak **ideal satış fiyatını tahmin eden** makine öğrenmesi modelleri geliştirmek  

Bu kapsamda analizler; fiyat, donanım gereksinimleri, kullanıcı geri bildirimleri, yayınlanma sıklığı ve pazar büyümesi eksenlerinde ele alınmıştır.

---

## Kullanılan Teknoloji ve Mimari

Proje, **Modern Data Stack** yaklaşımıyla bulut tabanlı olarak tasarlanmıştır.

### Veri Altyapısı ve Modelleme
- **Google BigQuery:** Ham ve işlenmiş verilerin tutulduğu merkezi veri ambarı  
- **dbt Cloud:** Analitik veri modelleme  
  - Katmanlar: **Staging → Intermediate → Mart**

### Analiz ve Modelleme
- **Python & SQL:** Keşifçi veri analizi (EDA), veri temizleme ve dönüşümler  
- **Google Colab:** Analiz ve makine öğrenmesi geliştirme ortamı

### Görselleştirme ve Proje Yönetimi
- **Looker Studio:** Karar destek amaçlı interaktif dashboard  
- **Notion & Slack:** Görev takibi ve proje koordinasyonu

---

## Canlı Çıktılar ve Dokümantasyon

Projeye ait ana çıktılara aşağıdaki bağlantılar üzerinden erişilebilir:

| İçerik | Açıklama | Link |
|--------|----------|------|
| 📊 Looker Studio Dashboard | Canlı analiz ve görselleştirme | [👉 Raporu Görüntüle](https://lookerstudio.google.com/reporting/b9a540f5-3547-47dd-93e2-4615199bd0fb) |
| 🗺️ Veri Mimarisi | Model ve veri akışı şeması (tldraw) | [👉 Mimariyi Görüntüle](https://www.tldraw.com/f/A1G0ucpf2pwONYo6cEshK?d=v-873.343.2568.1220.page) |

---

## Geliştirme Dosyaları

Projenin analiz ve modelleme sürecinde kullanılan çalışma dosyaları:

- **Model_1_Pazar_Tahmini.ipynb**  
  Oyun yayınlanma sıklığı ve pazar büyümesini inceleyen zaman serisi analizi

- **Steam_Oyun_Fiyatı_Tahminlemesi_Modeli.ipynb**  
  Oyun özelliklerine dayalı fiyat tahmini yapan regresyon modeli

- **Steam_Analizi_Data_visualization.pdf**  
  Analiz çıktıları ve iş içgörülerinin yer aldığı rapor

---

## Öne Çıkan Analitik Bulgular

### 📈 1. Oyun Fiyatlarında Yukarı Yönlü Baskı
2021–2025 dönemini kapsayan analizlerde, ortalama oyun fiyatlarının istikrarlı biçimde yükseldiği gözlemlenmiştir.  
Ortalama fiyatın **$8.28 → $10.15** seviyesine çıkması, pazar genelinde **%22’nin üzerinde** bir artışa işaret etmektedir.

---

### 🧩 2. Teknik Gereksinimler Fiyatı Belirliyor
Makine öğrenmesi modelinde **sistem gereksinimleri**, fiyat tahmininde en etkili değişkenlerden biri olarak öne çıkmıştır.  
Yüksek donanım gereksinimine sahip oyunların, piyasa ortalamasının yaklaşık **%60 üzerinde** fiyatlandığı görülmüştür.

---

### 🎯 3. Fiyat ve Algılanan Kalite Arasındaki Zayıf İlişki
Oyun fiyatı ile Metacritic puanı arasındaki korelasyon **0.23** seviyesinde hesaplanmıştır.  
Bu durum, yüksek fiyatın oyuncu memnuniyetini doğrudan garanti etmediğini göstermektedir.

---

### 🚀 4. Artan Rekabet ve Görünürlük Problemi
Zaman serisi analizleri, oyun yayınlanma sayısında **üstel bir artış** olduğunu ortaya koymuştur.  
Özellikle bağımsız geliştiriciler için rekabet avantajının artık üretimden çok **görünürlük (discoverability)** üzerinden şekillendiği gözlemlenmiştir.

---

## Sonuç

Bu proje, Steam pazarındaki fiyatlama davranışlarını hem analitik hem de öngörüsel (predictive) bir bakış açısıyla ele alarak, veri odaklı karar alma süreçlerine katkı sağlamayı amaçlamaktadır.
