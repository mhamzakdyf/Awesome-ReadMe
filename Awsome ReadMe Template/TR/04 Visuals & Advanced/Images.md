# 🖼️ Görseller ve Medya Rehberi (`Images & Media`)

Bu rehber, `README` dosyalarınıza resim, GIF ve hatta video gibi görsel öğeleri nasıl ekleyeceğinizi detaylı bir şekilde açıklamaktadır. Görsel medya, projenizin ne yaptığını göstermenin, karmaşık fikirleri basitleştirmenin ve belgenizi daha ilgi çekici hale getirmenin en etkili yoludur.

## İçindekiler

1.  [Neden Görsel Medya Kullanmalıyız?](#1-neden-görsel-medya-kullanmalıyız)
2.  [Temel Resim Ekleme (Syntax)](#2-temel-resim-ekleme-syntax)
3.  [Resim Kaynakları: Nereden Yüklemeli?](#3-resim-kaynakları-nereden-yüklemeli)
4.  [Gelişmiş Teknikler: Boyutlandırma ve Hizalama](#4-gelişmiş-teknikler-boyutlandırma-ve-hizalama)
5.  [Hareketli GIF'ler Ekleme](#5-hareketli-gifler-ekleme)
6.  [Video Ekleme (YouTube Örneği)](#6-video-ekleme-youtube-örneği)
7.  [En İyi Kullanım Pratikleri](#7-en-i̇yi-kullanım-pratikleri)

-----

## 1\. Neden Görsel Medya Kullanmalıyız?

Bir resim bin kelimeye bedeldir. `README` dosyanızda görseller kullanmak:

  - **Projenizi Sergiler:** Projenizin arayüzünün ekran görüntüleri, nasıl çalıştığını metinden çok daha hızlı anlatır.
  - **Anlaşılırlığı Artırır:** Karmaşık mimari diyagramları veya akış şemaları, metinsel açıklamalardan daha kolay anlaşılır.
  - **İlgi Çeker:** Görseller, metin duvarlarını kırarak belgenizin daha az göz korkutucu ve daha ilgi çekici görünmesini sağlar.
  - **Profesyonel Bir İmaj Yaratır:** İyi seçilmiş ve yerleştirilmiş görseller, projenizin kalitesini ve üzerine harcanan emeği gösterir.

## 2\. Temel Resim Ekleme (Syntax)

Markdown'da bir resim eklemenin temel sözdizimi bir linke çok benzer, ancak başında bir ünlem işareti (`!`) bulunur.

`![Alt Metin](Resim URL'si veya Dosya Yolu)`

  - `!`: Bu ifadenin bir resim olduğunu belirtir.
  - `![Alt Metin]`: "Alternatif metin" anlamına gelir. Resim yüklenemezse veya ekran okuyucu kullanan biri belgeyi incelerse bu metin görünür/okunur.
  - `(Resim URL'si veya Dosya Yolu)`: Resmin bulunduğu yer.

## 3\. Resim Kaynakları: Nereden Yüklemeli?

Resimlerinizi `README`'nize eklemenin iki ana yolu vardır:

### Yöntem 1: Proje İçinden (Göreceli Yol - Relative Path)

En güvenilir yöntem, resim dosyalarını doğrudan projenizin reposuna yüklemektir. Genellikle bunun için bir `assets`, `images` veya `docs` klasörü oluşturulur.

**Örnek Klasör Yapısı:**

```
proje/
├── README.md
└── assets/
    └── screenshot.png
```

Bu yapıdaki `screenshot.png` resmini `README.md`'ye eklemek için:

```markdown
![Proje Ekran Görüntüsü](./assets/screenshot.png)
```

### Yöntem 2: Harici Bir URL'den (Absolute URL)

Resmi başka bir web sitesinden veya bir resim barındırma servisinden de ekleyebilirsiniz. Tek yapmanız gereken resmin tam URL'sini kullanmaktır.

```markdown
![Harici Resim](https://via.placeholder.com/400x200)
```

> **Uyarı:** Bu yöntem, harici sitenin resmi silmesi veya URL'yi değiştirmesi durumunda resminizin kaybolmasına neden olabilir. Bu nedenle genellikle proje içine yükleme yöntemi tercih edilir.

## 4\. Gelişmiş Teknikler: Boyutlandırma ve Hizalama

Standart Markdown, resim boyutlarını veya hizalamasını kontrol etmek için bir yol sunmaz. Ancak, bu işlemler için temel HTML `<img>` etiketini kullanabilirsiniz.

### Boyutlandırma

Resmin genişliğini (`width`) ve/veya yüksekliğini (`height`) piksel cinsinden ayarlayabilirsiniz.

```html
<img src="./assets/screenshot.png" alt="Ekran Görüntüsü" width="500">
```

### Hizalama

Resmi ortalamak için HTML'in `<p>` veya `<div>` etiketlerini kullanabilirsiniz.

```html
<p align="center">
  <img src="./assets/screenshot.png" alt="Ekran Görüntüsü" width="500">
</p>
```

## 5\. Hareketli GIF'ler Ekleme

Hareketli GIF'ler, projenizin bir özelliğinin nasıl çalıştığını kısa bir animasyonla göstermek için harikadır. GIF eklemek, normal bir resim eklemekle tamamen aynıdır.

```markdown
![Özellik Demosu](./assets/feature-demo.gif)
```

## 6\. Video Ekleme (YouTube Örneği)

Markdown, videoları doğrudan oynatmanıza (`<video>` etiketi gibi) izin vermez. Ancak en yaygın ve etkili çözüm, videonun bir **önizleme resmini (thumbnail)** kullanarak videonun kendisine **link vermektir**.

Kullanıcı videonun resmine tıklar ve yeni bir sekmede (örneğin YouTube'da) video açılır.

### Örnek:

```markdown
[![Proje Tanıtım Videosu](https://img.youtube.com/vi/YOUTUBE_VIDEO_ID/0.jpg)](https://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID)
```

  - `YOUTUBE_VIDEO_ID` kısmını kendi videonuzun kimliğiyle değiştirmeniz yeterlidir (örneğin, URL'deki `v=`'den sonraki kısım).
  - Dıştaki `[]()` yapısı bunu bir linke dönüştürür.
  - İçteki `![]()` yapısı ise linkin içeriğini bir resim yapar.

## 7\. En İyi Kullanım Pratikleri

  - **Dosya Boyutunu Optimize Edin:** `README` dosyanıza eklediğiniz resimlerin dosya boyutlarını (MB yerine KB) küçük tutun. Büyük resimler sayfanın yavaş yüklenmesine neden olur.
  - **Alt Metin Kullanın:** Erişilebilirlik için her zaman açıklayıcı bir "Alt Metin" ekleyin.
  - **Görsel Tutarlılığı Sağlayın:** Kullandığınız görsellerin (ekran görüntüleri, diyagramlar vb.) stil olarak birbiriyle tutarlı olmasına özen gösterin.
  - **Aşırıya Kaçmayın:** Görseller güçlüdür, ancak çok fazla görsel kullanmak `README` dosyanızı dağınık gösterebilir. Sadece amaca hizmet eden görselleri kullanın.