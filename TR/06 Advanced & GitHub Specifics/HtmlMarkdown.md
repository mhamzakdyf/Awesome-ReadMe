# 🌐 Markdown İçinde HTML Rehberi (`HTML in Markdown`)

Bu rehber, standart Markdown'ın yetersiz kaldığı durumlarda, belgelerinize daha fazla kontrol ve stil katmak için **HTML etiketlerinin** nasıl kullanılacağını açıklamaktadır. GitHub'ın Markdown yorumlayıcısı, çoğu temel HTML etiketini destekler, bu da size resimleri boyutlandırma, metni daha hassas hizalama ve gelişmiş yapılar oluşturma gibi imkanlar tanır.

## İçindekiler

1.  [Neden Markdown İçinde HTML Kullanılır?](#1-neden-markdown-i̇çinde-html-kullanılır)
2.  [Temel Metin Biçimlendirme](#2-temel-metin-biçimlendirme)
3.  [Gelişmiş Resim Kontrolü](#3-gelişmiş-resim-kontrolü)
4.  [Katlanabilir Bölümler (Detaylar ve Özet)](#4-katlanabilir-bölümler-detaylar-ve-özet)
5.  [Klavye Kısayolları Gösterme](#5-klavye-kısayolları-gösterme)
6.  [Markdown ile HTML'i Birleştirmek](#6-markdown-ile-htmli-birleştirmek)
7.  [En İyi Kullanım Pratikleri ve Sınırlamalar](#7-en-i̇yi-kullanım-pratikleri-ve-sınırlamalar)

-----

## 1\. Neden Markdown İçinde HTML Kullanılır?

Markdown, basitliği ve okunabilirliği ile bilinir. Ancak bazen daha fazlasına ihtiyaç duyarsınız:

  - **Boyutlandırma ve Hizalama:** Bir resmi ortalamak veya boyutunu ayarlamak.
  - **İnce Ayar Biçimlendirme:** Altı çizili metin oluşturmak veya zorunlu bir satır atlama eklemek.
  - **İnteraktif Öğeler:** `details` etiketi gibi katlanabilir menüler oluşturmak.
  - **Özel Yapılar:** Standart Markdown'ın desteklemediği daha karmaşık yapılar.

Bu gibi durumlarda, doğrudan Markdown dosyanızın içine HTML kodları yazabilirsiniz.

## 2\. Temel Metin Biçimlendirme

Markdown'da bulunmayan bazı temel metin stilleri için HTML kullanabilirsiniz.

### Altı Çizili Metin (`<u>`)

```html
Bu <u>altı çizili</u> bir metindir.
```

**Sonuç:** Bu \<u\>altı çizili\</u\> bir metindir.

### Satır Atlama (`<br>`)

Markdown'da yeni bir satıra geçmek için genellikle boş bir satır bırakmanız gerekir. Ancak bazen metnin hemen alt satırdan devam etmesini istersiniz. `<br>` etiketi tam olarak bunu yapar.

```markdown
Bu birinci satır.<br>Bu ise hemen altındaki satır.
```

**Sonuç:**
Bu birinci satır.<br>Bu ise hemen altındaki satır.

## 3\. Gelişmiş Resim Kontrolü

Bu, HTML'in en yaygın kullanıldığı alanlardan biridir. Standart Markdown `![alt](src)` sözdizimi, resim boyutunu veya hizalamasını kontrol etmenize izin vermez.

### Resmi Boyutlandırma

`<img>` etiketinin `width` veya `height` özelliklerini kullanarak resmin boyutunu piksel cinsinden ayarlayabilirsiniz.

```html
<img src="./assets/logo.png" alt="Proje Logosu" width="100">
```

### Resmi Hizalama

Bir resmi ortalamak veya sağa yaslamak için onu `align` özelliğine sahip bir `<p>` veya `<div>` etiketi içine alabilirsiniz.

**Ortalanmış Resim:**

```html
<p align="center">
  <img src="./assets/logo.png" alt="Proje Logosu" width="200">
</p>
```

**Sağa Yaslanmış Resim:**

```html
<p align="right">
  <img src="./assets/logo.png" alt="Proje Logosu" width="100">
</p>
```

## 4\. Katlanabilir Bölümler (Detaylar ve Özet)

Daha önceki rehberde de bahsedildiği gibi, `<details>` ve `<summary>` etiketleri, `README` dosyalarınıza interaktif, açılır/kapanır bölümler eklemenin en iyi yoludur.

```html
<details>
  <summary>🚀 Gelişmiş Kurulum Adımları</summary>

  Buraya normalde gizli olan detaylı kurulum adımlarını veya kod bloklarını ekleyebilirsiniz.
</details>
```

## 5\. Klavye Kısayolları Gösterme

Dokümantasyonunuzda klavye kısayollarını belirtmek için `<kbd>` (keyboard) etiketi harikadır. Tarayıcılar bu etiketi genellikle bir tuş gibi görünen özel bir fontla stilize eder.

```html
Dosyayı kaydetmek için <kbd>Ctrl</kbd> + <kbd>S</kbd> tuş kombinasyonunu kullanın.
```

**Sonuç:**
Dosyayı kaydetmek için \<kbd\>Ctrl\</kbd\> + \<kbd\>S\</kbd\> tuş kombinasyonunu kullanın.

## 6\. Markdown ile HTML'i Birleştirmek

HTML etiketlerinin içindeki içerik, çoğu zaman yine Markdown olarak yorumlanabilir. Bunun için HTML bloğunuzun başlangıç ve bitiş etiketlerinden sonra birer boş satır bırakmanız gerekir.

```html
<p align="center">
  
  _Bu metin hem ortalanmış hem de **italik ve kalın**._

  `Bu da bir kod parçası.`

</p>
```

**Sonuç:**

\<p align="center"\>

*Bu metin hem ortalanmış hem de **italik ve kalın**.*

`Bu da bir kod parçası.`

\</p\>

## 7\. En İyi Kullanım Pratikleri ve Sınırlamalar

  - **Gereksiz Kullanımdan Kaçının:** Eğer bir şeyi standart Markdown ile yapabiliyorsanız, onu tercih edin. HTML, okunabilirliği azaltabilir. Sadece Markdown'ın yeteneklerinin bittiği yerde HTML kullanın.
  - **Güvenlik Sınırlamaları:** GitHub, güvenlik nedeniyle tehlikeli olabilecek HTML etiketlerini ve özelliklerini (`<script>`, `<iframe>`, `style` vb.) engeller. Sadece temel biçimlendirme ve yapı etiketlerini kullanabilirsiniz.
  - **Uyumluluk:** Yazdığınız HTML'in farklı Markdown yorumlayıcılarında (örneğin başka bir Git platformu veya statik site üreteci) aynı şekilde görünmeyebileceğini unutmayın.
  - **Okunabilirlik:** Karmaşık HTML yapıları, ham `.md` dosyasının okunmasını zorlaştırabilir. Kodunuzu temiz ve düzenli tutun.