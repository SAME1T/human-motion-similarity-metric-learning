# Human Motion Similarity Evaluation Based on Deep Metric Learning

Bu proje, insan hareketlerini analiz etmek ve benzerliklerini ölçmek için derin öğrenme tabanlı bir yaklaşım sunar. MediaPipe kullanılarak videolardan iskelet noktaları çıkarılır, bu noktalar bir Autoencoder modeli ile sıkıştırılmış temsillere dönüştürülür ve benzerlik ölçümleri yapılır.

## Proje Özeti

- **İskelet Noktası Çıkarımı:** MediaPipe Pose kullanılarak videolardan bel üstü 17 iskelet noktası (x, y) koordinatları çıkarılır.
- **Autoencoder Modeli:** 34 boyutlu iskelet verileri, Autoencoder modeli ile sıkıştırılmış 128 boyutlu latent vektörlere dönüştürülür.
- **Benzerlik Ölçümleri:**
  - **Cosine Similarity:** İki hareket dizisinin yönsel benzerliğini ölçer.
  - **Dynamic Time Warping (DTW):** Zaman serileri arasındaki hizalamayı ve benzerliği değerlendirir.

## Proje Yapısı

## Kullanılan Teknolojiler

- **Python Kütüphaneleri:**
  - `MediaPipe`: İskelet noktalarını çıkarmak için.
  - `PyTorch`: Autoencoder modelini oluşturmak ve eğitmek için.
  - `NumPy`: Veri işleme ve analiz için.
  - `Matplotlib`: Görselleştirme için.
  - `fastdtw`: DTW algoritması ile zaman serisi benzerliği ölçmek için.
- **Jupyter Notebook:** Proje geliştirme ve analiz için.

## Kurulum

1. **Gerekli Bağımlılıkları Yükleyin:**
   ```bash
   python -m venv venv_310
   source venv_310/Scripts/activate  # Windows için
   pip install -r requirements.txt

