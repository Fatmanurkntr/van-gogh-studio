# 🎨 Van Gogh Studio - Ultimate Edition

**Van Gogh Studio**, Vincent van Gogh’un impasto tekniğinden ilham alan, statik görüntüleri yaşayan parçaçık simülasyonlarına dönüştüren etkileşimli ve üretken bir sanat uygulamasıdır.

Bu proje, klasik bilgisayar grafikleri algoritmalarını (Flow Fields) modern Üretken Yapay Zekâ (Google Gemini) ile birleştirerek benzersiz bir dijital sanat deneyimi sunar.

🔗 **Live Demo:**  
https://Fatmanurkntr.github.io/van-gogh-studio/

---

## ✨ Key Features (What You Can Do)

### 1. 🖌️ Interactive Painting & Animation
- **Living Canvas:** Görsel sabit değil; görüntü verisine göre sıvı gibi akar.  
- **Magic Brush:** Fare veya dokunmatik ekran ile “canlandırma” hareketi yapabilirsin.  
- **Freeze & Flow:** Simülasyonu dondur veya akmaya bırak.

### 2. 🎵 Audio Reactive Art
- **Dance with Music:** Mikrofonu aç, sanat eserin müziğin ritmiyle hareket etsin.  
- **Bass & Rhythm:** Bas seslerde parçacıklar hızlanır; müzik durunca sakinleşir.

### 3. 🧠 Hybrid AI Capabilities
- **Smart Filters (No API Required):**  
  “Fire”, “Ocean”, “Forest”, “Matrix” gibi kelimelerle anında renk paleti değiştir.  
- **Gemini Art Critic:**  
  Yaptığın tabloyu analiz edip şiirsel yorumlar üretebilir.  
- **Generative Art (Pro):**  
  Metin açıklamalarından yeni SVG görüntüler oluştur (örnek: *“A cyberpunk city in Van Gogh style”*).

### 4. ⏪ Time Travel (Robust Undo System)
- **Step-by-Step Undo:**  
  Fırça hatalarını veya filtre değişikliklerini tek tek geriye al.  
- **Snapshot Memory:**  
  Her parçacığın konumu kaydedildiği için pürüzsüz geri sarma mümkündür.

### 5. 🛠️ Customization Studio
- Parçacık yoğunluğu (pixel size), akış hızı (viscosity), fırça yarıçapını anlık değiştir.  
- **Shape Shifting:** Square, Circle veya Line parçacık tipleri.  
- **Export:** Yüksek çözünürlüklü PNG indirme veya 5 saniyelik video kaydı.

---

## 🔧 How It Works (The Engineering)

Bu proje, tamamen **Vanilla JavaScript** ve **HTML5 Canvas API** ile, çekirdek motorda hiçbir dış bağımlılık olmadan geliştirildi.

### 1. Flow Field Algorithm
- **Luminance Calculation:**  
  Her pikselin parlaklığı şöyle hesaplanır: `0.299R + 0.587G + 0.114B`
- **Vector Mapping:**  
  Parlak piksel → belirli bir açıya sahip akış vektörü.  
- **Particle Physics:**  
  Binlerce parçacık bu görünmez vektörleri takip eder ve “rüzgârla akan fırça darbeleri” efekti oluşur.

### 2. "Tethered Flow" Physics
- **Liquid Motion:** Parçacıklar fırça hareket yönünde akar.  
- **Form Retention:**  
  Parçacıklar kaçıp kaybolmaz; orijinal konumlarına geri dönerler.  
- **Underpainting:**  
  Arkaplan katmanı siyah boşluk oluşmasını engeller.

### 3. Hybrid AI Integration
- **Local Logic (Free):**  
  Kelime → renk paleti dönüşümü için yerel hashing algoritması.  
- **Remote API (Google Gemini):**  
  - Görüntü üretimi  
  - Sanat analizi  
  - SVG işleme  

---

## 🚀 Tech Stack
- **Frontend:** HTML5, CSS3 (Glassmorphism), JavaScript (ES6+)  
- **Graphics:** HTML5 Canvas API  
- **AI:** Google Gemini API  
- **Hosting:** GitHub Pages

---

## 📦 Installation & Usage

```bash
git clone https://github.com/Fatmanurkntr/van-gogh-studio.git
