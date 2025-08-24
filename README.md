# Enuygun.com Load Test (JMeter)

Bu proje, **Enuygun.com uçuş arama modülü** üzerinde basit bir yük testi senaryosu çalıştırmak için hazırlanmıştır.  
Amaç, uçuş arama işlemi sonrası sistemin cevap sürelerini, hata oranlarını ve throughput değerlerini ölçmektir.  

---

## Proje Yapısı

- `EnUygunPerformans.jmx` → JMeter test planı  
- `results.jtl` → Test çalıştırma sonucu (otomatik üretilir)  
- `htmlReport/` → Renkli HTML rapor çıktısı (otomatik üretilir)  

---

## Test Senaryosu

- Kullanıcı, İstanbul → Ankara uçuşlarını arar.  
- JMeter HTTP Request Sampler üzerinden bu uçuş araması gerçekleştirilir.  
- Sonuçlar `Aggregate Report` ve HTML raporunda gözlemlenir.  

---

## Çalıştırma

### 1. JMeter ile GUI’den
- Apache JMeter’i aç.  
- `EnUygunPerformans.jmx` dosyasını yükle.  
- Thread Group içinden testi başlat.  
- Listener’lardan (`View Results Tree`, `Aggregate Report`) sonuçları incele.  

