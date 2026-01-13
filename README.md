# 🎵 Moodify
# 🎵 Moodify (TR/EN)

---

## 🇹🇷 Türkçe

Moodify, kullanıcının yüz ifadesinden **duygu tespiti** yaparak, bu duygu durumuna uygun şekilde **Spotify üzerinden kişiselleştirilmiş şarkı önerileri** sunan bir mobil uygulamadır.

### ✨ Özellikler
- 📷 Instagram/Snap benzeri kamera ekranı ile fotoğraf çekme
- 🧠 ML ile duygu tespiti (angry, happy, neutral, sad, surprised)
- 🎧 Duyguya göre **5 şarkılık öneri listesi**
  - Kullanıcının dinleme geçmişi
  - Beğendiği şarkılar
  - Beğenebileceği öneriler
- ▶️ Şarkıyı uygulama içinden oynatma
- ➕ Spotify playlist’ine ekleme
- ❤️ Spotify “Liked Songs” listesine ekleme
- 🔐 Spotify OAuth ile giriş/izin yönetimi

### 🧭 Kullanıcı Akışı
1. Kullanıcı giriş yapar (Spotify ile)
2. Kamera ekranında fotoğraf çeker
3. Fotoğraf ML modülüne gider → duygu tahmini yapılır
4. Duyguya göre 5 şarkı önerisi gösterilir
5. Kullanıcı şarkıyı çalar / playlist’e ekler / beğenir

### 🏗️ Mimari (Özet)
- **Mobile UI:** (Plan) React Native
- **ML Module:** MediaPipe FaceMesh + scikit-learn (RandomForest)
- **Spotify Integration:** Spotify Web API (OAuth/PKCE önerilir)

> Not: Dataset görselleri repo’ya dahil edilmez.

---

## EN English

Moodify is a mobile application that detects the user’s **emotion from facial expressions** and provides **personalized Spotify music recommendations** based on that emotion.

### ✨ Features
- 📷 Instagram/Snap-like camera screen to capture a photo
- 🧠 ML-based emotion recognition (angry, happy, neutral, sad, surprised)
- 🎧 A list of **5 recommended songs** based on:
  - Listening history
  - Liked songs
  - Additional personalized recommendations
- ▶️ Play a selected track inside the app
- ➕ Add the track to a Spotify playlist
- ❤️ Save the track to Spotify “Liked Songs”
- 🔐 Spotify OAuth login & permissions management

### 🧭 User Flow
1. User logs in (with Spotify)
2. User captures a photo via the camera screen
3. The photo is sent to the ML module → emotion is predicted
4. The UI displays 5 songs tailored to the detected emotion
5. User can play / add to playlist / like the song

### 🏗️ Architecture (Summary)
- **Mobile UI:** (Planned) React Native
- **ML Module:** MediaPipe FaceMesh + scikit-learn (RandomForest)
- **Spotify Integration:** Spotify Web API (OAuth/PKCE recommended)

> Note: Training images/datasets are not included in this repository.
