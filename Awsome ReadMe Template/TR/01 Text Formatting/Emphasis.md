# ✍️ Markdown'da Vurgulama

Bu rehber, metinlerinizi daha okunaklı, anlaşılır ve etkili hale getirmek için kullanabileceğiniz tüm temel ve gelişmiş vurgulama tekniklerini içermektedir. Doğru vurgulama, okuyucunun dikkatini önemli noktalara çekmenin ve belgenizin genel kalitesini artırmanın anahtarıdır.

## İçindekiler

1.  [İtalik (Eğik) Yazı](#1-i̇talik-eğik-yazı)
2.  [Kalın (Bold) Yazı](#2-kalın-bold-yazı)
3.  [Kalın ve İtalik Yazı](#3-kalın-ve-i̇talik-yazı)
4.  [Üstü Çizili (Strikethrough) Metin](#4-üstü-çizili-strikethrough-metin)
5.  [Satır İçi Kod (Inline Code)](#5-satır-i̇çi-kod-inline-code)
6.  [Vurgulanan Metin (Highlight)](#6-vurgulanan-metin-highlight)
7.  [Altı Çizili Metin (Underline)](#7-altı-çizili-metin-underline)
8.  [Alıntı Blokları (Blockquotes)](#8-alıntı-blokları-blockquotes)

-----

## 1\. İtalik (Eğik) Yazı

Hafif bir vurgu yapmak, terimleri, kitap adlarını veya bir düşünceyi belirtmek için kullanılır. Metni ana akıştan nazikçe ayırır.

### Yazım Kuralları (Syntax)

Metni tek yıldız (`*`) veya tek alt çizgi (`_`) arasına alarak italik yapabilirsiniz.

```markdown
*Bu metin italiktir.*
_Bu metin de italiktir._
```

### Kullanım Örnekleri

  - Bir düşünceyi belirtirken: *Acaba bu özelliği eklesek mi?*
  - Kitap veya film adlarında: En sevdiğim kitap *Simyacı*'dır.
  - Hafif vurgu için: Bu işlemi yapmadan önce *lütfen* yedek aldığınızdan emin olun.

## 2\. Kalın (Bold) Yazı

Güçlü bir vurgu yapmak, önemli uyarıları, anahtar kelimeleri veya dikkat çekilmesi gereken kritik bilgileri belirtmek için kullanılır.

### Yazım Kuralları (Syntax)

Metni çift yıldız (`**`) veya çift alt çizgi (`__`) arasına alarak kalın yapabilirsiniz.

```markdown
**Bu metin kalındır.**
__Bu metin de kalındır.__
```

### Kullanım Örnekleri

  - Uyarılar için: **DİKKAT:** Bu işlem geri alınamaz.
  - Anahtar kelimeler için: Projenin çalışması için **Node.js** sürüm 18 veya üzeri gereklidir.
  - Önemli adımlar için: Önce **"Kaydet"** butonuna basmayı unutmayın.

## 3\. Kalın ve İtalik Yazı

Mevcut en güçlü vurgulama yöntemidir. Çok kritik uyarılar veya metin içinde aşırı derecede dikkat çekmesi gereken ifadeler için kullanılır.

### Yazım Kuralları (Syntax)

Metni üç yıldız (`***`) veya üç alt çizgi (`___`) arasına alarak hem kalın hem de italik yapabilirsiniz.

```markdown
***Bu metin hem kalın hem de italiktir.***
___Bu metin de hem kalın hem de italiktir.___
```

### Kullanım Örnekleri

  - En kritik uyarılar için: Bu komutu çalıştırmak ***tüm veritabanını kalıcı olarak silecektir\!***
  - Abartılı bir vurgu için: Bu özelliği geliştirmek ***aylarımızı*** aldı.

## 4\. Üstü Çizili (Strikethrough) Metin

Artık geçerli olmayan, güncelliğini yitirmiş bilgileri, tamamlanmış görevleri veya bir fikrin alternatifini belirtmek için kullanılır.

### Yazım Kuralları (Syntax)

Metni iki yaklaşık işareti (`~~`) arasına alarak üstünü çizebilirsiniz.

```markdown
~~Bu metin üstü çizilidir.~~
```

### Kullanım Örnekleri

  - Güncelliğini yitirmiş bilgi: Gereksinimler: \~\~Python 2.7\~\~ Python 3.8 veya üstü.
  - İndirimli fiyat gösterimi: Fiyat: \~\~100 TL\~\~ **75 TL**
  - Tamamlanan görevler: Yapılacaklar: \~\~Kurulum rehberini yaz\~\~

## 5\. Satır İçi Kod (Inline Code)

Teknik terimleri, dosya adlarını, değişken isimlerini, kısa kod parçacıklarını veya komutları metnin geri kalanından ayırmak için kullanılır. Bu, teknik belgeler için en önemli vurgulama araçlarından biridir.

### Yazım Kuralları (Syntax)

Metni tekil ters tırnak (`` ` ``) arasına alarak satır içi kod olarak biçimlendirebilirsiniz.

```markdown
`Bu metin satır içi koddur.`
```

### Kullanım Örnekleri

  - Dosya adları: Ayarlarınızı `.env` dosyasında yapılandırın.
  - Fonksiyon adları: `getUserData()` fonksiyonu kullanıcı verilerini döndürür.
  - Komutlar: Projeyi başlatmak için terminale `npm run start` yazın.
  - Değişkenler: `API_KEY` değişkenini boş bırakmamalısınız.

## 6\. Vurgulanan Metin (Highlight)

Metnin bir bölümünü fosforlu kalemle çizmiş gibi görsel olarak öne çıkarmak için kullanılır. Bu özellik standart Markdown'da olmasa da GitHub gibi birçok platform tarafından desteklenir.

### Yazım Kuralları (Syntax)

Metni çift eşittir işareti (`==`) arasına alarak vurgulayabilirsiniz.

```markdown
==Bu metin vurgulanmıştır.==
```

### Kullanım Örnekleri

  - Bir sonuç cümlesini öne çıkarmak için: Analiz sonucunda, ==performansın %30 arttığı== tespit edildi.
  - Okuyucunun odaklanması gereken bir bölümü belirtmek için: ==Bu bölümü atlamadan önce dikkatlice okuyun.==

## 7\. Altı Çizili Metin (Underline)
Yazının bir bölümünün altını çizerek dikkat çekmek için kullanılır. Standart Markdown'da yoktur ancak Github tarafından desteklenir.

### Yazım Kuralları (Syntax)

Metni <ins> </ins> arasına alarak altını çizebilirsiniz.

```markdown
<ins>Bu metnin altı çizilidir.</ins>
```

### Kullanım Örnekleri

  - Metnin bir başka bölümüne dikkat çekmek için: Linux kullancılarının <ins>Linux Kurulum Rehberi</ins>ni okumaları önerilir.
  - Okuyucunun dikkat etmesi gereken bir bölümü belirtmek için: Bu özellik <ins>2.3</ins> sürümünde eklenmiştir.

## 8\. Alıntı Blokları (Blockquotes)

Doğrudan bir vurgulama olmasa da, bir metin bloğunu girintili hale getirerek dikkat çekici bir not, ipucu veya alıntı olarak sunar. Bu nedenle etkili bir vurgu aracıdır.

### Yazım Kuralları (Syntax)

Satırın başına büyüktür işareti (`>`) koyarak alıntı bloğu oluşturabilirsiniz.

```markdown
> Bu bir alıntı bloğudur. Önemli notları veya ipuçlarını bu şekilde belirtebilirsiniz.
```

### Kullanım Örnekleri

> **İpucu:** Daha iyi performans için, veritabanı sorgularınızı döngülerin dışında çalıştırmaya özen gösterin.
