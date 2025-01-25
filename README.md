# IMDb Veri Analizi Projesi

Bu proje, IMDb verileri kullanılarak yapılan bir veri analizi çalışmasını kapsamaktadır. Çalışma, filmlerin/türlerin popülerliği, IMDb puanı, oy sayıları ve içerik süreleri arasındaki ilişkilerin derinlemesine incelenmesini amaçlamaktadır. Ayrıca analiz bulguları, içerik üreticilerine veya sektördeki ilgililere yönelik stratejik öneriler sunmayı hedeflemektedir.

---

## Kullanılan Veri Seti

- **IMDb Verileri:** Bu çalışma için kullanılan veri seti https://www.kaggle.com/datasets/thedevastator/the-ultimate-netflix-tv-shows-and-movies-dataset adresinden alınmıştır.

Bu projede kullanılan veri setindeki sütunlar aşağıdaki gibidir:

- **`title`**: Film veya TV şovunun adı. *(String)*
- **`type`**: İçeriğin türü (Film veya TV şovu). *(String)*
- **`release_year`**: İçeriğin yayınlandığı yıl. *(Integer)*
- **`age_certification`**: İçeriğin yaş sınıflandırması. *(String)*
- **`runtime`**: Film veya TV şovunun süresi (dakika). *(Integer)*
- **`genres`**: İçeriğin türleri (örneğin: Drama, Komedi). *(String)*
- **`production_countries`**: İçeriğin yapım ülkeleri. *(String)*
- **`seasons`**: TV şovunun sezon sayısı (sadece TV şovları için geçerlidir). *(Integer)*
- **`imdb_score`**: Film veya TV şovunun IMDb puanı. *(Float)*
- **`imdb_votes`**: Film veya TV şovunun IMDb oy sayısı. *(Integer)*

---

## Proje İçeriği

Bu projede aşağıdaki analizler gerçekleştirilmiştir:
1. **IMDb Puanı ve Süre İlişkisi:**
   - Uzun içeriklerin daha fazla oy aldığı, ancak genelde daha düşük puanlarla değerlendirildiği gözlemlendi.
   - Kısa içeriklerin daha az oy aldığı fakat genelde daha yüksek puanlara sahip olduğu görüldü.

   - **Öneri:** Geniş kitlelere ulaşmak için uzun içerikler üretilebilir.

2. **IMDb Puanı ve Oy Sayısı Arasındaki İlişki:**
   - Çok sayıda oy alan içeriklerin genelde orta düzeyde puanlara sahip olduğu, az oy alan içeriklerin ise puan dağılımında daha geniş bir aralığa sahip olduğu tespit edildi.

3. **Türlerin Popülerliği:**
   - **Drama** en popüler tür olarak öne çıktı. Ardından komedi ve belgesel türleri geldi.
   - **Reality-TV** türündeki içeriklerin genelde daha düşük puanlara sahip olduğu saptandı.

    - **Öneri:** Drama türünde içerik üretmek, daha fazla izleyiciye ulaşmak için etkili olabilir.

4. **Ülkelere Göre Tür Popülerliği:**
   - ABD’de aksiyon ve macera türleri öne çıkarken, Avrupa ülkelerinde drama ve belgesel türlerinin daha popüler olduğu gözlemlendi.

5. **Yıllara Göre Türlerin Popülerliği:**
   - Türlerin popülerlik eğilimleri zamanla değişiklik göstermiş, özellikle son yıllarda drama, komedi ve belgesel türlerinin yükselişte olduğu belirlenmiştir.

   - **Öneri:** Yeni içerik üretiminde, bu türlerdeki artan talep değerlendirilebilir.

---

## Kullanılan Teknolojiler

- **Python**: Veri analizi ve işleme için ana programlama dili.
- **Pandas**: Veri manipülasyonu ve analizi için kullanıldı.
- **Matplotlib & Seaborn**: Veri görselleştirme için kullanıldı.
- **Scipy (spearmanr)**: Değişkenler arasındaki korelasyonları ölçmek için kullanıldı.
- **Ast**: Veri yapılarının dinamik olarak işlenmesi ve dönüştürülmesi için kullanıldı.
- **Jupyter Notebook**: Çalışma ve analiz ortamı.

---

## Proje Dosyaları

1. **`Analiz_raw_titler.ipynb`**:
   - IMDb verilerinin analiz edildiği Jupyter Notebook dosyası.
2. **`raw_titles.csv`**:
    - Analiz için kullanılan csv dosyası
2. **`README.md`**:
   - Proje açıklamaları ve dökümantasyonu.

