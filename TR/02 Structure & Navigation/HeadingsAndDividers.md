# 🏛️ Başlıklar ve Bölücüler Rehberi (`Headings & Dividers`)

Bu rehber, Markdown belgelerinize yapısal bir iskelet kazandırmak için kullanılan en temel iki aracı açıklamaktadır: **Başlıklar (Headings)** ve **Bölücüler (Dividers)**. Bu öğeler, içeriğinizi mantıksal bölümlere ayırarak okunabilirliği ve gezinilebilirliği kökten iyileştirir.

## İçindekiler

1.  [Başlıklar (Headings) Nedir?](#1-başlıklar-headings-nedir)
2.  [Başlık Seviyeleri ve Yazım Kuralları](#2-başlık-seviyeleri-ve-yazım-kuralları)
3.  [Yatay Bölücüler (Horizontal Dividers)](#3-yatay-bölücüler-horizontal-dividers)
4.  [En İyi Kullanım Pratikleri](#4-en-i̇yi-kullanım-pratikleri)

-----

## 1\. Başlıklar (Headings) Nedir?

Başlıklar, belgenizin ana hatlarını ve hiyerarşisini oluşturmak için kullanılır. Bir kitabın bölümleri ve alt bölümleri gibi, başlıklar da okuyucunun belgenin yapısını bir bakışta anlamasını sağlar. Ayrıca, GitHub gibi platformlar bu başlıkları otomatik olarak belge içinde gezinmeyi sağlayan "anchor link'lere" (çapa linklere) dönüştürür.

Metni sadece **kalın** veya büyük yazmak yerine başlıkları kullanmak, belgenize anlamsal bir yapı kazandırdığı için çok daha doğrudur.

## 2\. Başlık Seviyeleri ve Yazım Kuralları

Markdown, `<h1>`'den `<h6>`'ya kadar 6 seviye başlık destekler. Bir başlık oluşturmak için satırın başına diyez (`#`) işareti koymanız yeterlidir. Diyez sayısı, başlığın seviyesini belirler.

### Başlık 1 (`#`)

En üst seviye başlıktır. Genellikle bir belgenin ana başlığı olarak **sadece bir kez** kullanılır.

```markdown
# Bu Başlık Seviye 1'dir
```

# Bu Başlık Seviye 1'dir

### Başlık 2 (`##`)

Ana bölümleri (örneğin "Kurulum", "Kullanım", "Özellikler") belirtmek için kullanılır.

```markdown
## Bu Başlık Seviye 2'dir
```

## Bu Başlık Seviye 2'dir

### Başlık 3 (`###`)

Ana bölümlerin alt başlıklarını oluşturmak için kullanılır. (örneğin "Kurulum" altındaki "Gereksinimler", "Adım Adım Kurulum").

```markdown
### Bu Başlık Seviye 3'tür
```

### Bu Başlık Seviye 3'tür

### Diğer Seviyeler (`####`, `#####`, `######`)

Daha da detaya inmek gerektiğinde bu alt seviyeler kullanılır.

```markdown
#### Başlık 4
##### Başlık 5
###### Başlık 6
```

#### Başlık 4

##### Başlık 5

###### Başlık 6

-----

## 3\. Yatay Bölücüler (Horizontal Dividers)

Yatay bölücüler, içerik olarak birbirinden tamamen farklı olan bölümleri görsel olarak ayırmak için kullanılan tematik bir ayraçtır. Belge içinde keskin bir geçiş olduğunu belirtir.

### Temel Yazım Kuralları (Syntax)

Boş bir satıra üç veya daha fazla tire (`---`), yıldız (`***`) veya alt çizgi (`___`) koyarak bir bölücü oluşturabilirsiniz.

```markdown
---

***

___
```

### Sonuç:

Yukarıdaki üç yazım da aşağıdaki gibi bir yatay çizgi oluşturur:

-----

### Kullanım Örneği

Bir bölümün sonunda ve tamamen yeni bir bölüme başlamadan önce kullanmak idealdir.

```markdown
... önceki bölümün sonu.

---

## Yeni Bir Bölüm

Bu bölümde tamamen farklı bir konuya geçiyoruz...
```

-----

## 4\. En İyi Kullanım Pratikleri

1.  **Tek Bir `H1` Kullanın:** Belgenizin ana başlığı için sadece bir tane `# Başlık 1` kullanın. Bu, hem anlamsal olarak doğrudur hem de kafa karışıklığını önler.
2.  **Hiyerarşiyi Atlamayın:** Mantıksal bir akış için başlık seviyelerini sırayla kullanın. Örneğin, bir `## Başlık 2`'den sonra doğrudan `#### Başlık 4`'e atlamak yerine önce `### Başlık 3` kullanın.
3.  **Boşluk Bırakın:** Diyez (`#`) işareti ile başlık metni arasında her zaman bir boşluk bırakın. `##Başlık` yerine `## Başlık` şeklinde yazılmalıdır.
4.  **Bölücüleri İdareli Kullanın:** Her başlığın altına bir bölücü eklemek gereksizdir. Bölücüleri, sadece tematik olarak büyük bir geçiş yaptığınızda veya görsel olarak güçlü bir ayrım yaratmak istediğinizde kullanın.