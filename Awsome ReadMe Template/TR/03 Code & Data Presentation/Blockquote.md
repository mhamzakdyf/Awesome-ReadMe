# 🗨️ Alıntılar ve Notlar Rehberi (`Blockquotes`)

Bu rehber, metin içinde önemli notları, ipuçlarını, uyarıları veya başka bir kaynaktan yapılan alıntıları vurgulamak için kullanılan **Alıntı Blokları (Blockquotes)** özelliğini detaylıca açıklamaktadır. Alıntılar, metnin bir bölümünü görsel olarak ayırarak okuyucunun dikkatini belirli bir mesaja çekmenin etkili bir yoludur.

## İçindekiler

1.  [Alıntı Bloğu Nedir ve Neden Kullanılır?](#1-alıntı-bloğu-nedir-ve-neden-kullanılır)
2.  [Temel Alıntı Bloğu Oluşturma (Syntax)](#2-temel-alıntı-bloğu-oluşturma-syntax)
3.  [Gelişmiş Kullanım Teknikleri](#3-gelişmiş-kullanım-teknikleri)
4.  [GitHub'a Özel: Modern Uyarı Blokları (Alerts)](#4-githuba-özel-modern-uyarı-blokları-alerts)
5.  [En İyi Kullanım Pratikleri](#4-githuba-özel-modern-uyarı-blokları-alerts)

-----

## 1\. Alıntı Bloğu Nedir ve Neden Kullanılır?

Alıntı bloğu, bir veya daha fazla paragrafı girintili hale getirerek ve genellikle soluna dikey bir çizgi ekleyerek metnin geri kalanından ayıran bir biçimlendirme elementidir. Başlıca kullanım amaçları şunlardır:

  - **Önemli Notlar:** Kullanıcının gözden kaçırmaması gereken bilgileri vurgulamak.
  - **İpuçları (Tips):** Kullanıcıya faydalı bir tavsiye veya kısa yol sunmak.
  - **Uyarılar (Warnings):** Potansiyel bir riske veya kritik bir adıma dikkat çekmek.
  - **Alıntılar:** Başka bir dokümandan, kişiden veya kaynaktan alıntı yapılan metinleri belirtmek.

## 2\. Temel Alıntı Bloğu Oluşturma (Syntax)

Bir alıntı bloğu oluşturmak son derece basittir. Vurgulamak istediğiniz satırın veya paragrafın başına büyüktür işareti (`>`) ve bir boşluk koymanız yeterlidir.

```markdown
> Bu bir alıntı bloğudur. Bu metin, normal metin akışından görsel olarak ayrılacaktır.
```

### Sonuç:

> Bu bir alıntı bloğudur. Bu metin, normal metin akışından görsel olarak ayrılacaktır.

#### Çok Satırlı Alıntılar

Uzun paragraflar için her satırın başına `>` koyabilirsiniz. Ancak çoğu Markdown yorumlayıcısı, sadece paragrafın ilk satırına `>` koymanızı yeterli görür.

```markdown
> Bu birinci satır.
> Bu ikinci satır.
>
> Bu da arada bir boşluk bıraktıktan sonraki paragraf.
```

### Sonuç:

> Bu birinci satır.
> Bu ikinci satır.
>
> Bu da arada bir boşluk bıraktıktan sonraki paragraf.

-----

## 3\. Gelişmiş Kullanım Teknikleri

### İç İçe Alıntılar

Alıntı bloklarını iç içe kullanarak daha derin bir hiyerarşi oluşturabilirsiniz. Bunun için ikinci seviye için `>>` kullanmanız yeterlidir.

```markdown
> Bu birinci seviye alıntı.
> > Bu da ikinci seviye, daha girintili bir alıntı.
> Geri birinci seviyeye döndük.
```

### Sonuç:

> Bu birinci seviye alıntı.
>
> > Bu da ikinci seviye, daha girintili bir alıntı.
> > Geri birinci seviyeye döndük.

### Alıntı İçinde Diğer Biçimlendirmeler

Alıntı bloklarının içine başlık, liste, kalın metin veya kod gibi diğer Markdown öğelerini ekleyerek zengin not kutuları oluşturabilirsiniz.

```markdown
> #### 📝 Önemli Not
>
> - Projeyi çalıştırmadan önce **mutlaka** `.env` dosyasını oluşturun.
> - `API_KEY` değişkeninin boş olmadığından emin olun.
> - Detaylar için `config.js` dosyasına bakın.
```

### Sonuç:

> #### 📝 Önemli Not
>
>   - Projeyi çalıştırmadan önce **mutlaka** `.env` dosyasını oluşturun.
>   - `API_KEY` değişkeninin boş olmadığından emin olun.
>   - Detaylar için `config.js` dosyasına bakın.

-----

## 4\. GitHub'a Özel: Modern Uyarı Blokları (Alerts)

GitHub, yakın zamanda alıntı bloklarını kullanarak daha belirgin ve standartlaşmış not kutuları oluşturmak için özel bir "Alert" formatı duyurdu. Bu, notlarınızı daha anlaşılır ve görsel olarak çekici hale getirir.

### Yazım Kuralı

Normal bir alıntı bloğunun ilk satırına `**Note**`, `**Warning**` gibi özel bir anahtar kelime eklemeniz yeterlidir.

#### Not Bloğu

```markdown
> [!NOTE]
> Bu, genel bir bilgiyi veya hatırlatmayı vurgulamak için kullanılır.
```

> [\!NOTE]
> Bu, genel bir bilgiyi veya hatırlatmayı vurgulamak için kullanılır.

#### İpucu Bloğu

```markdown
> [!TIP]
> Bu, kullanıcılara faydalı bir ipucu veya en iyi pratik önerisi sunmak için kullanılır.
```

> [\!TIP]
> Bu, kullanıcılara faydalı bir ipucu veya en iyi pratik önerisi sunmak için kullanılır.

#### Uyarı Bloğu

```markdown
> [!WARNING]
> Bu, dikkatli olunması gereken veya beklenmedik sonuçlar doğurabilecek durumlar için kullanılır.
```

> [\!WARNING]
> Bu, dikkatli olunması gereken veya beklenmedik sonuçlar doğurabilecek durumlar için kullanılır.

> **Diğer Tipler:** `[!IMPORTANT]` (önemli bilgiler için) ve `[!CAUTION]` (kritik riskler için) gibi başka türler de mevcuttur.

-----

## 5\. En İyi Kullanım Pratikleri

  - **Kısa ve Öz Olun:** Alıntı blokları dikkat çekmek içindir. Çok uzun metinler bu etkiyi azaltır.
  - **Aşırı Kullanımdan Kaçının:** Belgenizin her yerini alıntı bloklarıyla doldurmak, onların vurgulayıcı etkisini ortadan kaldırır. Sadece gerçekten önemli noktalar için kullanın.
  - **GitHub Alerts'i Tercih Edin:** Eğer dokümantasyonunuz öncelikli olarak GitHub içinse, standart `>` yerine GitHub'un yeni `[!NOTE]` gibi "Alert" formatlarını kullanmak, notlarınızı daha modern ve anlaşılır kılacaktır.