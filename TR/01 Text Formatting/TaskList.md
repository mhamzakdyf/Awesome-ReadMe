# ✅ Markdown'da Görev Listeleri (Task Lists)

Bu rehber, GitHub Flavored Markdown (GFM) kullanarak interaktif görev listeleri oluşturmanın tüm detaylarını açıklamaktadır. Görev listeleri, yapılacak işleri (`To-Do List`), projenin ilerleme durumunu veya bir dizi gereksinimin tamamlanıp tamamlanmadığını takip etmek için mükemmel bir araçtır.

## İçindekiler

1. [Görev Listesi Tanımı](#1-görev-listesi-nedir)
2. [Temel Yazım Kuralları](#2-temel-yazım-kuralları-syntax)
3. [Pratik Kullanım Alanları](#3-pratik-kullanım-alanları)

---
## 1\. Görev Listesi Nedir?

Görev listesi, her bir maddesi tıklanabilir bir onay kutusuna (`checkbox`) sahip olan özel bir Markdown listesidir. GitHub'da bu listeler statik metinlerden daha fazlasıdır; doğrudan `README` dosyası, `Issue` veya `Pull Request` açıklaması üzerinden kutucukları işaretleyerek görevlerin durumunu güncelleyebilirsiniz.

## 2\. Temel Yazım Kuralları (Syntax)

Bir görev listesi oluşturmak çok basittir. Standart bir sırasız listenin (`-`, `*` veya `+` ile başlayan) her bir maddesinin başına `[ ]` (tamamlanmamış) veya `[x]` (tamamlanmış) eklemeniz yeterlidir.

### Tamamlanmamış Görev

Boş bir onay kutusu için köşeli parantezlerin arasına bir boşluk bırakın.

```markdown
- [ ] Bu görev henüz tamamlanmadı.
* [ ] Bu da tamamlanmadı.
```

**Sonuç:**

  - [ ] Bu görev henüz tamamlanmadı.
  - [ ] Bu da tamamlanmadı.

### Tamamlanmış Görev

Tamamlanmış bir görev için köşeli parantezlerin arasına küçük harfle `x` yazın.

```markdown
- [x] Bu görev tamamlandı.
* [x] Bu görev de başarıyla bitti.
```

**Sonuç:**

  - [x] Bu görev tamamlandı.
  - [x] Bu görev de başarıyla bitti.


## 3\. Pratik Kullanım Alanları

  - **Proje Yol Haritası (Roadmap):** `README.md` dosyanızda projenin gelecek versiyonları için planlanan özellikleri bir görev listesi olarak sunabilirsiniz.
  - **Pull Request (PR) Şablonları:** Bir PR açıldığında geliştiricinin tamamlaması gereken adımları (testleri çalıştırma, dokümantasyonu güncelleme vb.) bir görev listesi olarak şablona ekleyebilirsiniz. Bu, kod kalitesini artırır.
  - **Issue Takibi:** Bir hata veya özellik talebi (`Issue`) oluşturulduğunda, çözüm için gereken adımları bir görev listesi olarak belirtebilirsiniz.
  - **Kişisel Notlar:** Kendi `TODO` listenizi bir Markdown dosyasında kolayca tutabilirsiniz.