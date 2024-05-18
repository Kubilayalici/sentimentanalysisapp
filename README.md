# Duygu Analiz Uygulaması

## Genel Bakış
Duygu Analiz Uygulaması, kullanıcıların bir CSV dosyasını yüklemesine, bir sütun seçmesine, metin verilerini ön işlemesine, verileri görselleştirmesine, duygu analizi yapmasına ve çeşitli makine öğrenimi modelleri kullanarak tahminler yapmasına olanak tanıyan bir Tkinter tabanlı grafik kullanıcı arayüzü (GUI) uygulamasıdır.

## Özellikler
- CSV dosyası yükleyin
- Analiz için bir sütun seçin
- Metin verilerini ön işleyin
- Verileri çubuk grafiği ve kelime bulutu kullanarak görselleştirin
- Duygu analizi yapın
- Lojistik Regresyon, Random Forest ve K-En Yakın Komşu (KNN) modelleri kullanarak tahminler yapın
- Rastgele bir inceleme örneğinin ham ve ön işlenmiş halini görüntüleyin

## Gereksinimler
- Python 3.x
- pandas
- nltk
- scikit-learn
- wordcloud
- matplotlib
- tkinter

## Kurulum
1. Gerekli kütüphaneleri yükleyin:
    ```bash
    pip install pandas nltk scikit-learn wordcloud matplotlib tkinter
    ```

2. Script'i yerel makinenize indirin veya klonlayın.

## Kullanım
1. Uygulamayı çalıştırmak için terminalden şu komutu çalıştırın:
    ```bash
    python sentiment_analysis_app.py
    ```

2. Uygulama açıldıktan sonra:
    - "CSV Dosyası Yükle" butonuna tıklayarak bir CSV dosyası seçin.
    - Analiz etmek istediğiniz sütunun adını giriş kutusuna girin ve "Devam Et" butonuna tıklayın.
    - Verileri görselleştirmek için "Barplot Göster" veya "Wordcloud Göster" butonlarına tıklayın.
    - Duygu analizi yapmak için "Duygu Analizi Yap" butonuna tıklayın.
    - Tahminler yapmak için "Logistic Regression Tahmini", "Random Forest Tahmini" veya "KNN Tahmini" butonlarına tıklayın.
    - Rastgele bir incelemenin ham ve ön işlenmiş hallerini görüntülemek için tahmin butonlarına tıkladıktan sonra bilgi kutusunda incelemeleri görün.

## Kod Açıklaması
Uygulama kodu `SentimentAnalysisApp` sınıfında yer almaktadır. Bu sınıfın metodları şunlardır:
- `__init__(self, root)`: Uygulamanın ana bileşenlerini ve başlangıç ayarlarını tanımlar.
- `load_csv(self)`: CSV dosyasını yükler ve analiz edilecek kolonu seçer.
- `continue_analysis(self)`: Seçilen kolonda analiz işlemlerine devam eder.
- `preprocess_data(self)`: Metin verilerini ön işler.
- `show_barplot(self)`: En sık geçen kelimelerin çubuk grafiğini gösterir.
- `show_wordcloud(self)`: Kelime bulutunu gösterir.
- `sentiment_analysis(self)`: Duygu analizi yapar.
- `predict_logistic(self)`: Lojistik Regresyon modeli kullanarak tahmin yapar.
- `predict_rf(self)`: Random Forest modeli kullanarak tahmin yapar.
- `predict_knn(self)`: KNN modeli kullanarak tahmin yapar.

## Lisans
Bu proje MIT Lisansı ile lisanslanmıştır. Daha fazla bilgi için `LICENSE` dosyasına bakın.

---

Bu README dosyasını projenizin kök dizinine `README.md` adıyla kaydedebilirsiniz. Bu dosya, projeyi klonlayan veya indiren kullanıcıların projeyi kolayca anlamalarına ve kullanmalarına yardımcı olacaktır.
