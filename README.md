# Dilden Dile: Türk Masalları Derlemesi

Medipol Üniversitesi, Görsel İletişim Tasarımı, **Programlamaya Giriş** dersi vize projesi.

**Hazırlayan:** Rojin Esma Bacni
**Video sunumu (YouTube):** https://youtu.be/Gs1zI0n4LDw

## Proje nedir?

Türk halk anlatı geleneğinden seçilmiş **8 masalın** bir arada okunabildiği bir web sayfasıdır. Sayfa, HTML, CSS ve JavaScript ile sıfırdan tasarlanmıştır; hazır şablon kullanılmamıştır. Amaç, masalları süslemeden çok **okumaya hizmet eden** bir arayüzle sunmaktır.

## Sayfa nasıl açılır?

1. Bu depodaki **üç dosyayı** (`index.html`, `style.css`, `script.js`) aynı klasöre indirin.
2. `index.html` dosyasına çift tıklayın, sayfa tarayıcıda açılır.

İnternet bağlantısı gerekmez; harici yazı tipi, kütüphane ya da görsel dosyası kullanılmamıştır.

## Dosya yapısı

| Dosya | Görevi |
|---|---|
| `index.html` | Sayfanın iskeleti: başlık, masal kapakları, okuma bölümü |
| `style.css` | Renkler, yazı, düzen ve telefon uyumu (duyarlı tasarım) |
| `script.js` | Masalların verisi ve sayfadaki tüm işlevler |

## Sayfadaki işlevler (JavaScript)

- **Masal seçme:** Kapağa tıklayınca masal okuma sayfasında açılır.
- **Tür süzgeci:** Masal, Mizah, Destan, Halk hikâyesi gruplarına göre kapakları süzer.
- **Bir masal seç bana:** Rastgele bir masal açar.
- **Kitaplığım:** Devam ettiklerim, Bitirdiklerim ve Favorilerim ayrı sayfalarda, ilerleme çubuğuyla gösterilir. Veriler tarayıcıda (`localStorage`) saklanır. İlk açılışta sayfa boş görünmesin diye birkaç örnek kayıt vardır.
- **Okuma ilerlemesi:** Sayfa kaydırıldıkça okunma yüzdesi artar, sona gelince masal "Bitirdiklerim"e geçer. "Okudum" ve "Favorilere ekle" düğmeleri de vardır.
- **Okuma ayarları:** Yazı boyutunu büyütme ve küçültme, gece modu (seçim hatırlanır).
- **Gezinme:** Önceki ve sonraki masal düğmeleri, klavyede sağ ve sol ok tuşları, ana sayfaya dönüş.
- **Dinle:** Tarayıcının Türkçe sesiyle masalı sesli okutur (cihazda Türkçe ses yüklüyse çalışır).
- **Okuma süresi:** Metindeki kelime sayısına göre tahmini süre gösterir.

## Tasarım kararları

- **Renkler:** Derin bordo zemin, altın ve krem vurgular, siyah ve koyu petrol mavisi kapaklar. Kilim, tezhip ve çini sanatındaki renkleri çağrıştırdığı için seçildi. Masal metni açık krem bir sayfa üzerinde koyu kahve yazıyla verildi, böylece okunabilirlik (karşıtlık) yüksek kalır.
- **Yazı tipleri:** Masal metni ve başlıklar için kitap havası veren serif yazı tipleri (Georgia, Palatino), düğmeler için Segoe UI. İnternetsiz çalışması için yalnızca sistem yazı tipleri kullanıldı.
- **Süsler:** Kilim şeridi ve lale motifi kodla (SVG ve CSS) çizildi.
- **Duyarlı tasarım:** Kapaklar bilgisayarda 4'lü, telefonda 2'li sıralanır.
- **Kolay gezinme:** Tüm masallar ana sayfada tek bakışta görünür.

## Masallar ve kaynaklar

Masallar aşağıdaki kaynaklara dayanılarak **kendi cümlelerimizle yeniden yazılmıştır**. Her masalın altında da kaynak satırı bulunur.

1. **Keloğlan ve Dev:** İSEV, "Keloğlan Masalları", "Dev ile Keloğlan", https://www.isev.org.tr/wp-content/uploads/2015/12/keloglan_isev.pdf (erişim: 2 Kasım 2026)
2. **Nasreddin Hoca Fıkraları** (1-10): Akşehir Belediyesi, http://aksehir.bel.tr/fikralar.pdf (erişim: 2 Kasım 2026)
3. **Tepegöz:** "Dede Korkut – Tepegöz", Masal Dünyası, https://masal-dunyasi.vercel.app/masallar/dede-korkut-tepegoz (erişim: 2 Kasım 2026)
4. **Tahir ile Zühre:** Derki, https://derki.net/tr/product/964/tahir-ile-zuhre (erişim: 2 Kasım 2026)
5. **Gökten Üç Elma Düştü:** "Gökten Düşen Üç Elma Masalı", Masal Oku, https://www.masaloku.net/gokten-dusen-uc-elma/ (erişim: 2 Kasım 2026)
6. **Zümrüdüanka:** Bahar Arvasi, "Zümrüdüanka Kuşu", Masal Dergisi, sayı 12, 2022, https://www.masaldergisi.com/sayilar/2022/sayi-12/zumruduanka-kusu/ (erişim: 2 Kasım 2026). Yazarın dayandığı kaynaklar: Tahir Alangu, Billur Köşk Masalları, YKY, 2022; Eflatun Cem Güney, Zümrütanka, Yelkovan Dizisi, 2007.
7. **Altın Saçlı Kız:** "Altın Saçlı Kız Masalı", Masal Oku, https://www.masaloku.net/altin-sacli-kiz-masali/ (erişim: 2 Kasım 2026)
8. **Karagöz ile Hacivat:** "Perde Gazeli", "Bayramlaşma Bayramı", "Kolay Şiir", Masal Oku, https://www.masaloku.net/kategori/karagoz-ve-hacivat/ (erişim: 2 Kasım 2026)

## Yapay zekâ kullanımı

- **Kod:** Sayfanın HTML, CSS ve JavaScript kodunun yazımında Claude (Anthropic) yardımından yararlanıldı; kodun işleyişi tarafımdan açıklanabilmektedir.
- **Masal metinleri:** Yukarıdaki kaynaklardaki hikâyeler Claude yardımıyla yeniden yazıldı.
- **Görseller:** Masal kapak görselleri yapay zekâ ile üretildi. Kullanılan araç, istemler (prompt) ve görsellerin sayfadaki yerleri raporda yer almaktadır.
