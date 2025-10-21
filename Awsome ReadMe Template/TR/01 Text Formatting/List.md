# 📋 Listeler Rehberi (`Lists`)

Bu rehber, metinlerinizi organize etmek ve bilgiyi yapısal bir düzende sunmak için kullanabileceğiniz temel liste türlerini (Sırasız ve Sıralı) detaylı bir şekilde açıklamaktadır. Listeler, okunabilirliği artırmanın ve karmaşık bilgileri basitleştirmenin en etkili yollarından biridir.

## İçindekiler

1.  [Sırasız Listeler (Unordered Lists)](#1-sırasız-listeler-unordered-lists)
2.  [Sıralı Listeler (Ordered Lists)](#2-sıralı-listeler-ordered-lists)
3.  [İç İçe Listeler (Nested Lists)](#3-i̇ç-i̇çe-listeler-nested-lists)
4.  [Pratik Kullanım İpuçları](#4-pratik-kullanım-i̇puçları)

-----

## 1\. Sırasız Listeler (Unordered Lists)

Maddelerin belirli bir sıraya sahip olmadığı durumlar için kullanılır. Genellikle proje özelliklerini, bir konunun ana hatlarını, notları veya seçenekleri belirtmek için idealdir.

### Temel Yazım Kuralları (Syntax)

Bir satırın başına tire (`-`), yıldız (`*`) veya artı (`+`) işareti koyarak sırasız liste oluşturabilirsiniz. Bu üç karakter de görsel olarak aynı sonucu verir, bu nedenle tutarlılık için genellikle birini (çoğunlukla `-`) tercih etmek en iyisidir.

```markdown
- Madde A
- Madde B

* Madde C
* Madde D

+ Madde E
+ Madde F
```

### Sonuç:

  - Madde A
  - Madde B

<!-- end list -->

  * Madde C
  * Madde D

<!-- end list -->

  + Madde E
  + Madde F

### Kullanım Alanları

  - Proje özelliklerini listelemek
  - Bir beyin fırtınası notlarını düzenlemek
  - Bir konuda alınacak notları maddelendirmek

-----

## 2\. Sıralı Listeler (Ordered Lists)

Belirli bir sırayı takip etmesi gereken adımları göstermek için kullanılır. Kurulum talimatları, bir algoritmanın adımları veya önem sırasına göre bir liste oluşturmak için mükemmeldir.

### Temel Yazım Kuralları (Syntax)

Bir satırın başına sayı ve ardından nokta (`1.`) koyarak sıralı liste oluşturabilirsiniz.

**Önemli Bir Kolaylık:** Markdown, sayıları sizin için otomatik olarak doğru sırada işler. Bu nedenle, listenizdeki her maddeye `1.` yazsanız bile, sonuçta `1., 2., 3.` şeklinde doğru bir sıralama elde edersiniz. Bu, listeye yeni bir madde eklemeyi veya çıkarmayı çok kolaylaştırır.

```markdown
1. İlk adım: Depoyu klonla.
1. İkinci adım: Bağımlılıkları yükle.
1. Üçüncü adım: Projeyi başlat.
```

### Sonuç:

1.  İlk adım: Depoyu klonla.
2.  İkinci adım: Bağımlılıkları yükle.
3.  Üçüncü adım: Projeyi başlat.

### Kullanım Alanları

  - Kurulum ve yapılandırma talimatları
  - Bir tarifin veya sürecin adımları
  - En iyi 10 listesi gibi sıralamalar

-----

## 3\. İç İçe Listeler (Nested Lists)

Daha karmaşık ve hiyerarşik yapılar oluşturmak için listeleri iç içe kullanabilirsiniz. Bir alt madde oluşturmak için satırın başına birkaç boşluk (genellikle 2 veya 4 boşluk bir girinti seviyesidir) eklemeniz yeterlidir. Hem sıralı hem de sırasız listeleri bir arada iç içe kullanabilirsiniz.

### Örnek Yazım

```markdown
- Meyveler
  - Elma
  - Armut
- Sebzeler
  1. Havuç
  2. Brokoli
     - Yeşil Brokoli
     - Mor Brokoli
```

### Sonuç:

  - Meyveler
      - Elma
      - Armut
  - Sebzeler
    1.  Havuç
    2.  Brokoli
          - Yeşil Brokoli
          - Mor Brokoli

-----

## 4\. Pratik Kullanım İpuçları

  - **Tutarlılık:** Bir belge boyunca aynı liste işaretçisini (örneğin sadece `-`) kullanmak, `README` dosyanızın daha temiz ve profesyonel görünmesini sağlar.
  - **Boşluklar:** Listeler arasında bir satır boşluk bırakmak, okunabilirliği artırır.
  - **Diğer Öğeler:** Liste maddelerinin içine kalın, italik metinler veya satır içi kod gibi diğer Markdown öğelerini ekleyebilirsiniz.
    ```markdown
    - **Adım 1:** `config.js` dosyasını açın.
    - *Adım 2:* `API_KEY` değişkenini güncelleyin.
    ```