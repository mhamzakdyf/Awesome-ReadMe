# 🔗 Linkler ve Bağlantılar Rehberi (`Links`)

Bu rehber, Markdown belgelerinizi interaktif hale getiren ve farklı bilgi kaynaklarını birbirine bağlayan **linklerin** nasıl oluşturulacağını detaylı bir şekilde açıklamaktadır. Linkler, kullanıcıları harici web sitelerine, belgenin farklı bölümlerine veya reponuzdaki diğer dosyalara yönlendirmenin temel yoludur.

## İçindekiler

1.  [Link Nedir ve Neden Önemlidir?](#1-link-nedir-ve-neden-önemlidir)
2.  [Harici Linkler (External Links)](#2-harici-linkler-external-links)
3.  [Dahili Linkler (Internal/Anchor Links)](#3-dahili-linkler-internalanchor-links)
4.  [Göreceli Linkler (Relative Links)](#4-göreceli-linkler-relative-links)
5.  [Gelişmiş Link Teknikleri](#5-gelişmiş-link-teknikleri)
6.  [En İyi Kullanım Pratikleri](#6-en-i̇yi-kullanım-pratikleri)

-----

## 1\. Link Nedir ve Neden Önemlidir?

Link (veya bağlantı), tıklandığında sizi başka bir hedefe götüren bir metin veya görsel parçasıdır. `README` dosyalarında linkler şu amaçlarla kullanılır:

  - **Kaynak gösterme:** Kullanılan bir kütüphanenin, aracın veya makalenin web sitesine bağlantı vermek.
  - **Navigasyon:** Kullanıcıların belgenin farklı bölümleri arasında kolayca gezinmesini sağlamak (İçindekiler Tablosu gibi).
  - **İlişkili Dosyalar:** Projedeki diğer önemli dosyalara (`CONTRIBUTING.md`, `LICENSE` vb.) yönlendirme yapmak.
  - **Etkileşim:** Demo linkleri, iletişim adresleri veya sosyal medya profillerine bağlantı vermek.

## 2\. Harici Linkler (External Links)

Harici linkler, sizi mevcut belgenin dışındaki bir web sitesine yönlendirir.

### Temel Yazım Kuralları (Syntax)

Bir link oluşturmak için `[Görünen Metin](URL)` yapısı kullanılır.

  - `[Görünen Metin]`: Kullanıcının göreceği ve tıklayacağı metindir.
  - `(URL)`: Tıklandığında gidilecek web adresidir.

<!-- end list -->

```markdown
Projemiz [Google](https://www.google.com) arama motorunu kullanmaktadır.
Daha fazla bilgi için [Markdown Rehberi](https://www.markdownguide.org)'ni ziyaret edebilirsiniz.
```

### Sonuç:

Projemiz [Google](https://www.google.com) arama motorunu kullanmaktadır.
Daha fazla bilgi için [Markdown Rehberi](https://www.markdownguide.org)'ni ziyaret edebilirsiniz.

### Başlık (Title) Eklemek

Linkin üzerine fare ile gelindiğinde küçük bir açıklama kutucuğu (tooltip) çıkmasını isterseniz, URL'den sonra tırnak içinde bir başlık ekleyebilirsiniz.

```markdown
[GitHub](https://github.com "GitHub'un ana sayfasına gider")
```

**Sonuç:** [GitHub](https://github.com "GitHub'un ana sayfasına gider") (Farenizi üzerine getirin)

-----

## 3\. Dahili Linkler (Internal/Anchor Links)

Dahili linkler (çapa linkler), kullanıcıyı aynı belgenin içindeki farklı bir başlığa yönlendirir. Uzun belgelerde gezinmeyi kolaylaştırmak için, özellikle **İçindekiler Tablosu** oluştururken hayati öneme sahiptir.

### Yazım Kuralları (Syntax)

`[Görünen Metin](#hedef-başlığın-link-versiyonu)` yapısı kullanılır. `#` işareti, linkin aynı sayfa içinde olduğunu belirtir.

GitHub, başlıklarınızdan otomatik olarak bir link versiyonu oluşturur. Kurallar şunlardır:

1.  Tüm harfler küçük harfe çevrilir.
2.  Boşluklar tire (`-`) işaretiyle değiştirilir.
3.  Emoji ve özel karakterler (`?`, `!`, `.` vb.) kaldırılır.

**Örnek:**
`## 5. Gelişmiş Link Teknikleri` başlığına link vermek için:

```markdown
[Gelişmiş tekniklere git](#5-gelişmiş-link-teknikleri)
```

**Sonuç:** [Gelişmiş tekniklere git](#5-gelişmiş-link-teknikleri)

-----

## 4\. Göreceli Linkler (Relative Links)

Göreceli linkler, projenizin (reponuzun) içindeki diğer dosyalara bağlantı vermek için kullanılır. Bu, projenizi bütün halinde tutar ve linklerin projeniz nereye kopyalanırsa kopyalansın çalışmasını sağlar.

### Aynı Klasördeki Dosyaya Link

```markdown
Katkıda bulunma kuralları için lütfen [`CONTRIBUTING.md`](./CONTRIBUTING.md) dosyasını okuyun.
```

### Farklı Klasördeki Dosyaya Link

```markdown
Kurulum talimatları [`docs/INSTALL.md`](./docs/INSTALL.md) dosyasında bulunmaktadır.
```

-----

## 5\. Gelişmiş Link Teknikleri

### Görsel Linkleri (Image Links)

Bir görseli tıklanabilir bir link haline getirmek için, normal bir görsel tanımını (`![Alt Metin](resim-url)`) bir link tanımının içine yerleştirmeniz yeterlidir.

```markdown
[![Google Logosu](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)](https://google.com)
```

**Sonuç:** (Aşağıdaki resme tıklayabilirsiniz)

[](https://google.com)

### E-posta Linkleri (Mailto Links)

Kullanıcının varsayılan e-posta uygulamasını açan bir link oluşturmak için `mailto:` kullanılır.

```markdown
Sorularınız için [bize e-posta gönderin](mailto:ornek@mail.com).
```

**Sonuç:** Sorularınız için [bize e-posta gönderin](mailto:ornek@mail.com).

-----

## 6\. En İyi Kullanım Pratikleri

  - **Açıklayıcı Olun:** Link metni, linkin nereye gittiğini açıkça belirtmelidir. "Buraya tıklayın" gibi belirsiz ifadelerden kaçının.
      - **Kötü:** Detaylar için \<u\>buraya tıklayın\</u\>.
      - **İyi:** Detaylar için \<u\>kurulum rehberimizi\</u\> okuyun.
  - **Kısa ve Net:** Linkleri mümkün olduğunca kısa ve anlaşılır tutun.
  - **Kontrol Edin:** Belgenizi yayınlamadan önce tüm linklerin doğru çalıştığından emin olun. Kırık linkler profesyonel olmayan bir izlenim bırakır.