# 🎵 EverYTube - Kurulum Rehberi (Türkçe)

## 📋 Gereksinimler

- Node.js (v14+)
- npm veya yarn
- MongoDB (yerel veya Docker)
- YouTube API Key

## 🚀 Hızlı Başlangıç

### 1. YouTube API Key Al

1. [Google Cloud Console](https://console.cloud.google.com/) aç
2. Yeni proje oluştur
3. YouTube Data API v3'ü etkinleştir
4. API Key oluştur
5. Key'i kopyala

### 2. Backend Kurulumu

```bash
cd backend
npm install
```

`.env` dosyası oluştur:

```
MONGODB_URI=mongodb://localhost:27017/everytube
YOUTUBE_API_KEY=your_youtube_api_key_here
JWT_SECRET=your_secret_key_here
PORT=5000
```

Backend'i başlat:

```bash
npm run dev
```

### 3. Frontend Kurulumu

Yeni terminal aç:

```bash
cd frontend
npm install
npm start
```

### 4. MongoDB Başlat

#### Yerel MongoDB:
```bash
mongod
```

#### Docker ile MongoDB:
```bash
docker run -d -p 27017:27017 --name mongodb mongo
```

#### Docker Compose ile Hepsi:
```bash
docker-compose up -d
```

## 🎯 Kullanım

1. **Kaydol**: İlk sayfada yeni hesap oluştur
2. **Giriş Yap**: E-posta ve şifre ile giriş yap
3. **Görevler**: Görev ekle, düzenle, sil
4. **Müzik**: YouTube'da şarkı ara ve çal

## 🌐 Erişim

- **Frontend**: http://localhost:3000
- **Backend**: http://localhost:5000
- **MongoDB**: mongodb://localhost:27017

## 📝 Özellikler

### To-Do List
- ✅ Görev ekleme
- ✅ Tamamlandı işareti
- ✅ Öncelik seviyeleri
- ✅ Kategori ve etiketler
- ✅ Tarih/Deadline
- ✅ Filtreleme
- ✅ Local Storage

### Müzik Streaming
- 🔍 YouTube'da müzik ara
- ▶️ Doğrudan YouTube'dan çal
- 📋 Playlist oluştur
- ❤️ Favorilere ekle

---

**Hoşça Kalın! 🎵📝**