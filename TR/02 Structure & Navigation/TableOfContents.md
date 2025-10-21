# 🗺️ İçindekiler Tablosu Rehberi (`Table of Contents`)

Bu rehber, özellikle uzun ve detaylı `README` dosyalarında gezinmeyi kolaylaştırmak için hayati bir araç olan **İçindekiler Tablosu (Table of Contents - ToC)** oluşturmanın adımlarını açıklamaktadır. İyi yapılandırılmış bir ToC, belgenizin bir yol haritası görevi görür ve kullanıcıların aradıkları bilgiye anında ulaşmasını sağlar.

## İçindekiler

1.  [Neden İçindekiler Tablosu Kullanmalıyız?](#1-neden-i̇çindekiler-tablosu-kullanmalıyız)
2.  [Nasıl Çalışır? Anchor Link Mantığı](#2-nasıl-çalışır-anchor-link-mantığı)
3.  [Hedef Link Oluşturma Kuralları](#3-hedef-link-oluşturma-kuralları)
4.  [İçindekiler Tablosunu Oluşturmak](#4-i̇çindekiler-tablosunu-oluşturmak)
5.  [Kapsamlı Bir Örnek](#5-kapsamlı-bir-örnek)
6.  [En İyi Kullanım Pratikleri](#6-en-i̇yi-kullanım-pratikleri)

-----

## 1\. Neden İçindekiler Tablosu Kullanmalıyız?

Projeniz büyüdükçe, `README` dosyanız da doğal olarak uzayacaktır. Bir kullanıcı sadece "Kurulum" bölümünü arıyorsa, tüm belgeyi aşağı kaydırmak zorunda kalmamalıdır. İçindekiler Tablosu:

  - **Kullanıcı Deneyimini İyileştirir:** Aranan bilgiye tek tıkla ulaşım sağlar.
  - **Profesyonel Bir Görünüm Katar:** Belgenizin ne kadar organize ve iyi planlanmış olduğunu gösterir.
  - **Belge Yapısını Özetler:** Kullanıcıya belgenin genelinde hangi konuların yer aldığı hakkında hızlı bir fikir verir.

## 2\. Nasıl Çalışır? Anchor Link Mantığı

İçindekiler Tablosu, daha önceki rehberde öğrendiğimiz **Dahili Linklerin (Anchor Links)** yapısal bir listesidir. Temel mantık şudur:

1.  Belgenizdeki her bir başlık (`## Başlık`, `### Alt Başlık` vb.), GitHub tarafından otomatik olarak görünmez bir "çapa" (anchor) veya "kimlik" (ID) ile etiketlenir.
2.  Biz, bu çapalara yönlendiren özel linkler oluştururuz.
3.  Bu linkleri düzenli bir liste halinde sunarak İçindekiler Tablosu'nu oluştururuz.

## 3\. Hedef Link Oluşturma Kuralları

Bir başlığın çapa linkini doğru bir şekilde oluşturmak için uymanız gereken 3 basit kural vardır. Linki `[Görünen Metin](#hedef-link)` yapısındaki `#` işaretinden sonra gelen kısım için oluştururuz.

1.  **Tüm Harfleri Küçük Harfe Çevirin:** Başlıktaki `Proje Kurulumu` ifadesi `proje kurulumu` olur.
2.  **Boşlukları Tire (`-`) ile Değiştirin:** `proje kurulumu` ifadesi `proje-kurulumu` olur.
3.  **Özel Karakterleri Kaldırın:** Başlıktaki emoji (🎯), noktalama işaretleri (`?`, `!`, `.`), parantezler (`()`) gibi alfanümerik olmayan tüm karakterleri linkten silin.

#### Örnekler:

  - Başlık: `## 🚀 Proje Hakkında`

      - Link: `#-proje-hakkında` (Emoji kaldırıldı)

  - Başlık: `### Adım Adım Kurulum (Windows)`

      - Link: `#adım-adım-kurulum-windows` (Parantezler kaldırıldı)

  - Başlık: `### Sıkça Sorulan Sorular (SSS)`

      - Link: `#sıkça-sorulan-sorular-sss`

## 4\. İçindekiler Tablosunu Oluşturmak

Bu linkleri standart bir sırasız liste (`-`) halinde kullanarak tablonuzu oluşturabilirsiniz. Belgenizin hiyerarşisini yansıtmak için alt başlıkları (örneğin `###` seviyesindekileri) girintili yazmak en iyi pratiktir.

```markdown
- [Ana Başlık 1](#ana-başlık-1)
  - [Alt Başlık 1.1](#alt-başlık-11)
  - [Alt Başlık 1.2](#alt-başlık-12)
- [Ana Başlık 2](#ana-başlık-2)
```

## 5\. Kapsamlı Bir Örnek

Aşağıda tipik bir `README` yapısı ve onun için oluşturulmuş İçindekiler Tablosu bulunmaktadır.

#### Örnek Belge Yapısı:

```markdown
# Proje Adı

...kısa açıklama...

## 📜 Hakkında
...

## ✨ Özellikler
...

## 🛠️ Teknoloji Yığını
...

## 🚀 Kurulum
### Gereksinimler
### Adım Adım Kurulum

## 💻 Kullanım
...

## 🤝 Katkıda Bulunma
...
```

#### Bu yapı için oluşturulacak İçindekiler Tablosu:

```markdown
- [Hakkında](#-hakkında)
- [Özellikler](#-özellikler)
- [Teknoloji Yığını](#-teknoloji-yığını)
- [Kurulum](#-kurulum)
  - [Gereksinimler](#gereksinimler)
  - [Adım Adım Kurulum](#adım-adım-kurulum)
- [Kullanım](#-kullanım)
- [Katkıda Bulunma](#-katkıda-bulunma)
```
- [Hakkında](#-hakkında)
- [Özellikler](#-özellikler)
- [Teknoloji Yığını](#-teknoloji-yığını)
- [Kurulum](#-kurulum)
  - [Gereksinimler](#gereksinimler)
  - [Adım Adım Kurulum](#adım-adım-kurulum)
- [Kullanım](#-kullanım)
- [Katkıda Bulunma](#-katkıda-bulunma)


## 6\. En İyi Kullanım Pratikleri

  - **Konumlandırma:** İçindekiler Tablosu'nu genellikle projenin kısa açıklamasından hemen sonra, ilk ana bölümden ise önce yerleştirin.
  - **Seviye Seçimi:** Genellikle sadece 2. (`##`) ve 3. (`###`) seviye başlıkları tabloya eklemek yeterlidir. Daha alt seviyeleri (örn: `####`) eklemek tabloyu çok kalabalık ve okunaksız hale getirebilir.
  - **Tutarlılık:** Tablodaki link metninin, yönlendirdiği başlık metniyle tam olarak aynı olduğundan emin olun.
  - **Otomatik Araçlar:** Uzun belgeler için bu işlemi manuel yapmak yorucu olabilir. VS Code gibi editörlerde "Markdown All in One" gibi eklentiler, belgeniz için otomatik olarak bir İçindekiler Tablosu oluşturabilir.