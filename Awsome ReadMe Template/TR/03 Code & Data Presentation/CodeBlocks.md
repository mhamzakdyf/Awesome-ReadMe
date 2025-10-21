# 💻 Kod Gösterimi Rehberi (`Code Blocks`)

Bu rehber, teknik `README` dosyalarının en temel bileşeni olan **Kod Blokları (Code Blocks)** ve **Satır İçi Kod (Inline Code)** oluşturmayı detaylıca açıklamaktadır. Bu araçlar, kod parçacıklarını, komutları ve teknik terimleri normal metinden ayırarak okunabilirliği ve anlaşılırlığı en üst düzeye çıkarır.

## İçindekiler

1.  [Neden Kod Gösterimi Önemlidir?](#1-neden-kod-gösterimi-önemlidir)
2.  [Satır İçi Kod (Inline Code)](#2-satır-i̇çi-kod-inline-code)
3.  [Kod Blokları (Fenced Code Blocks)](#3-kod-blokları-fenced-code-blocks)
4.  [Sözdizimi Vurgulama (Syntax Highlighting)](#4-sözdizimi-vurgulama-syntax-highlighting)
5.  [En İyi Kullanım Pratikleri](#5-en-i̇yi-kullanım-pratikleri)

-----

## 1\. Neden Kod Gösterimi Önemlidir?

Teknik bir dokümanda, normal metin ile komutları veya kodları birbirinden ayırmak hayati önem taşır. Kod gösterimi:

  - **Okunabilirlik Sağlar:** Kodu özel bir fontla ve arka planla biçimlendirerek metnin geri kalanından ayırır.
  - **Kopyalamayı Kolaylaştırır:** GitHub gibi platformlar, kod bloklarının köşesine tek tıkla kopyalama butonu ekler.
  - **Anlamı Korur:** Kod içindeki girintileri, boşlukları ve özel karakterleri olduğu gibi korur.
  - **Hataları Önler:** Bir kullanıcının bir komutu yanlış yazmasını veya eksik kopyalamasını engeller.

## 2\. Satır İçi Kod (Inline Code)

Cümle içerisinde geçen tek bir komut, değişken adı, dosya yolu, fonksiyon adı veya kısa bir kod parçası gibi ifadeleri belirtmek için kullanılır.

### Temel Yazım Kuralları (Syntax)

Metni **tekil ters tırnak** (`` ` ``) arasına almanız yeterlidir. Bu karakter genellikle klavyede `Esc` tuşunun altında bulunur.

```markdown
Projenin çalışması için `npm install` komutunu çalıştırın. Ana yapılandırma dosyası `.env` olarak adlandırılmıştır. `getUser()` fonksiyonu kullanıcı bilgilerini getirir.
```

### Sonuç:

Projenin çalışması için `npm install` komutunu çalıştırın. Ana yapılandırma dosyası `.env` olarak adlandırılmıştır. `getUser()` fonksiyonu kullanıcı bilgilerini getirir.

## 3\. Kod Blokları (Fenced Code Blocks)

Birden çok satırdan oluşan uzun kod parçacıkları, yapılandırma dosyası örnekleri veya komut satırı çıktıları için kullanılır.

### Temel Yazım Kuralları (Syntax)

Kodunuzu **üçlü ters tırnak** (\`\`\`\`\`\`) satırları arasına yazmanız gerekir.

````markdown
```
Bu bir kod bloğudur.
Buradaki tüm satırlar
ve boşluklar korunur.
```
````

### Sonuç:

```
Bu bir kod bloğudur.
Buradaki tüm satırlar
ve boşluklar korunur.
```

## 4\. Sözdizimi Vurgulama (Syntax Highlighting)

Kod bloklarının en güçlü özelliği, kodu yazıldığı programlama diline göre renklendirebilmesidir. Bu, kodun okunabilirliğini inanılmaz derecede artırır.

Bunu yapmak için, başlangıçtaki üçlü ters tırnaktan hemen sonra dilin adını küçük harflerle belirtmeniz yeterlidir.

### JavaScript Örneği

````markdown
```javascript
function sayHello(name) {
  console.log(`Hello, ${name}!`);
}

sayHello('World');
```
````

**Sonuç:**

```javascript
function sayHello(name) {
  console.log(`Hello, ${name}!`);
}

sayHello('World');
```

### Python Örneği

````markdown
```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)

print(factorial(5))
```
````

**Sonuç:**

```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)

print(factorial(5))
```

### Komut Satırı Örneği (`shell` veya `bash`)

Terminal komutlarını göstermek için `shell` veya `bash` kullanmak standart bir pratiktir. Bu, satırların çalıştırılabilir komutlar olduğunu belirtir.

````markdown
```shell
# Projeyi klonla
git clone [https://github.com/user/repo.git](https://github.com/user/repo.git)

# Dizine gir
cd repo

# Bağımlılıkları yükle
npm install
```
````

**Sonuç:**

```shell
# Projeyi klonla
git clone https://github.com/user/repo.git

# Dizine gir
cd repo

# Bağımlılıkları yükle
npm install
```

## 5\. En İyi Kullanım Pratikleri

  - **Doğru Dili Belirtin:** Kodunuzun okunabilirliği için her zaman doğru dil tanımlayıcısını (`javascript`, `python`, `java`, `csharp`, `html`, `css` vb.) kullanın.
  - **Kısa ve Öz Olun:** Kod bloklarında sadece konuyu anlatmak için gerekli olan kod parçacığını gösterin. Yüzlerce satır kodu yapıştırmaktan kaçının.
  - **Açıklama Ekleyin:** Kod bloğundan önce veya sonra, bu kodun ne yaptığını ve neden önemli olduğunu açıklayan kısa bir metin ekleyin. Kullanıcıya bağlam sunun.
  - **Dil Belirtmeden Kaçının:** Eğer sadece basit bir metni veya bir komut çıktısını biçimlendirmek istiyorsanız, dil belirtmeden de kod bloğu kullanabilirsiniz. Bu, `plaintext` olarak kabul edilir.