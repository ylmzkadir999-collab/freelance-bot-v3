# 🤖 Freelance Otomasyon Botu

Web tabanlı freelance otomasyon aracı. OCR, Excel ve profesyonel Fatura PDF üretimi.

## ✨ Özellikler
- 🔍 **OCR**: Fotoğraf/taranmış belge → metin çıkarma
- 📊 **Excel**: Manuel giriş veya CSV → formatlı Excel
- 📄 **Fatura PDF**: Profesyonel fatura, KDV hesaplama, indirme

---

## 🚀 Railway'e Deploy (Ücretsiz, Telefondan)

### 1. GitHub'a Yükle
```
github.com → + New Repository → "freelance-bot" → Create
```
Tüm dosyaları yükle (GitHub Mobile veya github.dev ile).

### 2. Railway'e Deploy
```
railway.app → Start New Project → Deploy from GitHub Repo
→ Repoyu seç → Deploy
```

### 3. Domain Al
```
Railway Dashboard → Settings → Domains → Generate Domain
```
Sana `https://freelance-bot-xxx.up.railway.app` gibi bir URL verilecek. ✅

---

## 💻 Lokal Çalıştırma

### Tesseract Kur (OCR için)
- **Windows**: https://github.com/UB-Mannheim/tesseract/wiki
- **Mac**: `brew install tesseract tesseract-lang`
- **Linux**: `sudo apt install tesseract-ocr tesseract-ocr-tur`

### Python Paketleri
```bash
pip install -r requirements.txt
```

### Çalıştır
```bash
python app.py
# Tarayıcıda aç: http://localhost:5000
```

---

## 📁 Dosya Yapısı
```
freelance_bot/
├── app.py           ← Flask backend (OCR + Excel + PDF)
├── index.html       ← Web arayüzü
├── requirements.txt ← Python paketleri
├── Procfile         ← Railway/Render başlatma
├── railway.json     ← Railway ayarları
├── nixpacks.toml    ← Tesseract sisteme kurulumu
└── README.md
```

---

## 💡 Kullanım
1. Tarayıcıda aç
2. **OCR** → Görüntü yükle → Metin çıkar → Excel veya Fatura'ya aktar
3. **Excel** → Manuel giriş veya CSV yükle → İndir
4. **Fatura** → Formu doldur → PDF İndir

---

## ⚠️ Notlar
- OCR Türkçe ve İngilizce destekler
- Railway ücretsiz planda aylık 500 saat süre var
- Dosyalar sunucuda saklanmaz, direkt tarayıcıya indirilir
