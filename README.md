# Mugla Tarim - Harita Analiz (GitHub Pages Sürümü)

Bu klasör, projenizin PHP bağımlılığı olmadan GitHub Pages üzerinde statik olarak yayınlanması için hazırlanmıştır. Ayrıca PWA desteği sayesinde mobil cihazlara "Uygulama" olarak yüklenebilir.

## 🚀 GitHub'a Yükleme ve Yayınlama Adımları

Bu klasörü GitHub'a yüklemek için şu adımları izleyin:

1.  **GitHub'da bir Repository oluşturun:**
    - Tarayıcınızda GitHub'a gidin ve yeni bir "Public" repository oluşturun (örneğin adı `harita-analiz` olsun).
    - "Initialize this repository with a README" seçeneğini **işaretlemeyin**.

2.  **Terminali açın ve `github` klasörüne gidin:**
    ```bash
    cd c:\xampp\htdocs\muglatarimmobil\haritagosterim\github
    ```

3.  **Git deposunu başlatın ve dosyaları gönderin:**
    ```bash
    git init
    git add .
    git commit -m "İlk sürüm: Statik ve PWA desteği"
    git branch -M main
    git remote add origin https://github.com/KULLANICI_ADINIZ/harita-analiz.git
    git push -u origin main
    ```

4.  **GitHub Pages'i Etkinleştirin:**
    - GitHub'daki repository sayfanızda **Settings** > **Pages** sekmesine gidin.
    - **Build and deployment** > **Branch** kısmında `main` ve `/ (root)` seçili olduğundan emin olun.
    - **Save** butonuna basın.
    - Birkaç dakika içinde siteniz `https://KULLANICI_ADINIZ.github.io/harita-analiz/` adresinde yayına alınacaktır.

## 📱 Mobil Uygulama Olarak Yükleme
- Sitenizi telefonunuzun tarayıcısından (Chrome veya Safari) açın.
- Tarayıcı menüsünden "Ana Ekrana Ekle" veya "Uygulamayı Yükle" seçeneğine basın.
- Artık harita analiz aracını telefonunuzdan bir uygulama gibi kullanabilirsiniz.

## ⚠️ Önemli Notlar
- **Yeni Harita/Dosya Ekleme:** `maps/` veya `data/` klasörlerine yeni bir dosya eklediğinizde, bu dosyayı `maps.json` veya `mappings.json` listesine manuel olarak eklemeniz ve GitHub'a tekrar "push" etmeniz gerekir.
- **Güvenlik:** GitHub Pages herkese açık (Public) bir alandır. İçerisinde hassas veri bulunan (TC, VKN vb.) Excel dosyalarını veya JSON'ları yanlışlıkla GitHub'a yüklememeye dikkat edin.
