# 🧠 N8N Workflow Agent Builder Prompt

Bu repository, n8n otomasyonları üretmek için gelişmiş bir *LLM tabanlı prompt sistemini* barındırır. Amaç; girilen workflow ihtiyaçlarına göre **tam donanımlı, üretim düzeyinde N8N iş akışları** oluşturmaktır.

---

## ✨ Neden Bu Prompt?

Geleneksel promptlardan farklı olarak bu sistem, sadece JSON çıktısı üretmekle kalmaz, aynı zamanda her workflow için eksiksiz bir belge seti sunar:

- 📘 **Ayrıntılı Açıklama Dosyası**
- 📦 **Tam ve Geçerli N8N JSON Workflow**
- 🛠 **Kurulum ve Kimlik Bilgisi Talimatları**

---

## 📂 Yapı

Her istek, aşağıdaki 3 temel bileşeni içerecek şekilde yanıtlanır:

### 1. `DETAILED EXPLANATION` – Ayrıntılı Workflow Açıklama Dosyası
> **Format**: Markdown  
> **İçerik**:
- Amaç ve genel bakış
- Adım adım süreç açıklaması
- Tetikleyici mantığı
- Aksiyon ve entegrasyon açıklamaları
- Veri akış haritası
- Hata yönetimi ve geri dönüş mekanizmaları
- Kullanım senaryoları
- Örnek ile kıyaslama

### 2. `JSON WORKFLOW` – Geçerli N8N JSON Workflow Dosyası
> **Format**: JSON  
> **Özellikler**:
- N8N’ye doğrudan import edilebilir
- En son N8N şemasına uyumlu
- Tüm node'lar doğru şekilde yapılandırılmış
- Yorumlu ve okunabilir yapı
- Yeniden denenebilir, zaman aşımlı, hatalara dayanıklı yapı

### 3. `SETUP INSTRUCTIONS` – Kurulum ve Kimlik Bilgileri Talimatları
> **Format**: Markdown  
> **İçerik**:
- Gereksinimler ve ön koşullar
- API Anahtarı / Google Auth / Webhook kurulum adımları
- Gerekli Google Sheet şablonları (varsa)
- Örnek yapılandırmalar
- Test etme prosedürleri
- Hata ayıklama rehberi
- Sağlanan örneklerle karşılaştırma

---

## 🧠 Nasıl Kullanılır?

1. **Prompt'u kullanarak** sistem mesajına sahip bir LLM'ye bağlanın.
2. Kullanıcıdan ihtiyaç duyduğu workflow'u ve varsa örnekleri isteyin.
3. Her istekten sonra üçlü çıktıyı üretin:
   - Açıklama
   - JSON
   - Kurulum talimatları
4. Yanıtta verilen formatı kullanın:

