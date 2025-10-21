# 📊 Tablolar Rehberi (`Tables`)

Bu rehber, verileri yapısal ve düzenli bir şekilde sunmak için kullanılan **Markdown tablolarının** nasıl oluşturulacağını ve biçimlendirileceğini detaylıca açıklamaktadır. Tablolar, özellikleri karşılaştırmak, API parametrelerini listelemek veya yapılandırma seçeneklerini göstermek gibi durumlar için mükemmel bir araçtır.

## İçindekiler

1.  [Tablolar Neden Kullanışlıdır?](#1-tablolar-neden-kullanışlıdır)
2.  [Temel Tablo Oluşturma (Syntax)](#2-temel-tablo-oluşturma-syntax)
3.  [Sütunları Hizalama (Alignment)](#3-sütunları-hizalama-alignment)
4.  [Tablo İçinde Biçimlendirme](#4-tablo-i̇çinde-biçimlendirme)
5.  [En İyi Kullanım Pratikleri](#5-en-i̇yi-kullanım-pratikleri)

-----

## 1\. Tablolar Neden Kullanışlıdır?

Listeler veya normal metinlerin yetersiz kaldığı durumlarda tablolar devreye girer. Başlıca faydaları şunlardır:

  - **Karşılaştırma:** Farklı öğelerin özelliklerini yan yana kolayca karşılaştırmayı sağlar.
  - **Yapısal Veri:** Parametreler, seçenekler, tanımlar gibi "anahtar-değer" çiftlerini sunmak için idealdir.
  - **Okunabilirlik:** Bilgiyi satır ve sütunlara ayırarak taranmasını ve anlaşılmasını kolaylaştırır.
  - **Profesyonel Görünüm:** Teknik dokümantasyona düzenli ve profesyonel bir hava katar.

## 2\. Temel Tablo Oluşturma (Syntax)

Markdown'da tablo oluşturmanın temel mantığı oldukça basittir ve üç ana bileşenden oluşur:

1.  **Başlık Satırı (Header Row):** Sütun başlıklarını içerir. Hücreler dikey çizgi (`|`) ile ayrılır.
2.  **Ayırıcı Satır (Delimiter Row):** Başlıkları tablonun geri kalanından ayırır. Her sütun için en az üç tire (`---`) kullanılır.
3.  **İçerik Satırları (Content Rows):** Tablonun verilerini içerir. Hücreler yine `|` ile ayrılır.

### Temel Örnek

```markdown
| Başlık 1 | Başlık 2 | Başlık 3 |
|---|---|---|
| Satır 1, Sütun 1 | Satır 1, Sütun 2 | Satır 1, Sütun 3 |
| Satır 2, Sütun 1 | Satır 2, Sütun 2 | Satır 2, Sütun 3 |
| Satır 3, Sütun 1 | Satır 3, Sütun 2 | Satır 3, Sütun 3 |
```

### Sonuç:

| Başlık 1 | Başlık 2 | Başlık 3 |
|---|---|---|
| Satır 1, Sütun 1 | Satır 1, Sütun 2 | Satır 1, Sütun 3 |
| Satır 2, Sütun 1 | Satır 2, Sütun 2 | Satır 2, Sütun 3 |
| Satır 3, Sütun 1 | Satır 3, Sütun 2 | Satır 3, Sütun 3 |

-----

## 3\. Sütunları Hizalama (Alignment)

Tablodaki metinleri sola, sağa veya ortaya hizalamak için ayırıcı satıra iki nokta üst üste (`:`) ekleyebilirsiniz.

  - **Sola Hizala (Varsayılan):** `:---`
  - **Ortala:** `:---:`
  - **Sağa Hizala:** `---:`

### Hizalama Örneği

```markdown
| Komut | Açıklama | Gerekli mi? |
|:---|:---:|---:|
| `git clone` | Projeyi bilgisayarınıza kopyalar. | Evet |
| `npm install` | Gerekli paketleri yükler. | Evet |
| `npm test` | Testleri çalıştırır. | Hayır |
```

### Sonuç:

| Komut | Açıklama | Gerekli mi? |
|:---|:---:|---:|
| `git clone` | Projeyi bilgisayarınıza kopyalar. | Evet |
| `npm install` | Gerekli paketleri yükler. | Evet |
| `npm test` | Testleri çalıştırır. | Hayır |

-----

## 4\. Tablo İçinde Biçimlendirme

Tablo hücrelerinin içine diğer Markdown öğelerini ekleyebilirsiniz. Bu, tablolarınızı daha zengin ve bilgilendirici hale getirir.

  - Satır içi kod (`` ` ``)
  - Linkler (`[]()`)
  - Kalın veya italik metin (`**bold**`, `*italic*`)
  - Üstü çizili metin (`~~strikethrough~~`)

### Biçimlendirme Örneği

```markdown
| Parametre | Tip | Açıklama |
|---|---|---|
| `userId` | *string* | Bilgileri alınacak kullanıcının **benzersiz** ID'si. |
| `isActive` | *boolean* | Sadece aktif kullanıcıları listelemek için kullanılır. |
| `apiKey` | `string` | ~~Artık kullanılmıyor.~~ Bunun yerine token kullanın. |
| `docs` | [Link](https://...) | İlgili dokümantasyon sayfası. |
```

### Sonuç:

| Parametre | Tip | Açıklama |
|---|---|---|
| `userId` | *string* | Bilgileri alınacak kullanıcının **benzersiz** ID'si. |
| `isActive` | *boolean* | Sadece aktif kullanıcıları listelemek için kullanılır. |
| `apiKey` | `string` | \~\~Artık kullanılmıyor.\~\~ Bunun yerine token kullanın. |
| `docs` | [Link](https://www.google.com/search?q=https://...) | İlgili dokümantasyon sayfası. |

-----

## 5\. En İyi Kullanım Pratikleri

  - **Ham Kodu Okunabilir Yapın:** Markdown dosyasını düzenlerken de tablonun düzgün görünmesi için dikey çizgileri (`|`) alt alta hizalamak iyi bir pratiktir. Bu, render edilmiş sonucu etkilemez ama kaynak kodun okunabilirliğini artırır.
  - **Tabloları Basit Tutun:** Çok fazla sütun içeren geniş tablolar mobil cihazlarda iyi görünmeyebilir. Mümkünse tablolarınızı dar ve odaklanmış tutun.
  - **Boş Hücreler:** Bir hücreyi boş bırakmak istiyorsanız, dikey çizgiler (`|`) arasını boş bırakmanız yeterlidir.
  - **Gereksiz Kullanımdan Kaçının:** Basit bir listeyle anlatılabilecek bir şeyi tabloya dönüştürmeye gerek yoktur. Sadece yapısal veriler için kullanın.