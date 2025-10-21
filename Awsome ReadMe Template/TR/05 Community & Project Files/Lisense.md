# ⚖️ Lisanslama Rehberi (`LICENSE`)

Bu rehber, açık kaynaklı bir projenin en temel yasal belgesi olan **LISANS (LICENSE)** dosyasının neden bu kadar önemli olduğunu, popüler lisans türlerinin ne anlama geldiğini ve projenize nasıl bir lisans ekleyeceğinizi açıklamaktadır.

## İçindekiler

1.  [Lisans Nedir ve Neden Mutlaka Olmalıdır?](#1-lisans-nedir-ve-neden-mutlaka-olmalıdır)
2.  [Lisans Olmazsa Ne Olur?](#2-lisans-olmazsa-ne-olur)
3.  [Popüler Açık Kaynak Lisansları](#3-popüler-açık-kaynak-lisansları)
4.  [Hangi Lisansı Seçmeliyim?](#4-hangi-lisansı-seçmeliyim)
5.  [Projeye Lisans Nasıl Eklenir?](#5-projeye-lisans-nasıl-eklenir)

-----

## 1\. Lisans Nedir ve Neden Mutlaka Olmalıdır?

Yazılım lisansı, projenizin kaynak kodunu yayınlayan kişi olarak, başkalarına bu kodla neler yapıp yapamayacaklarını bildiren yasal bir belgedir. Bir lisans, kullanıcılara şu konularda net kurallar sunar:

  - **Kullanım:** Kodunuzu kendi projelerinde kullanabilirler mi?
  - **Değiştirme:** Kodunuzu değiştirebilirler mi?
  - **Dağıtım:** Kodunuzun orijinal veya değiştirilmiş versiyonlarını başkalarına dağıtabilirler mi?
  - **Ticari Kullanım:** Kodunuzu ticari bir ürün içinde kullanabilirler mi?
  - **Sorumluluk:** Kodunuz bir hata içeriyorsa kimin sorumlu olduğu.

Kısacası lisans, projenizin yasal korumasını sağlar ve hem sizin hem de kullanıcıların haklarını net bir şekilde belirler.

## 2\. Lisans Olmazsa Ne Olur?

**Bu en kritik noktadır:** Eğer projenizde bir `LICENSE` dosyası yoksa, varsayılan telif hakkı yasaları geçerli olur. Bu şu anlama gelir:

> **Kodunuzun tüm hakları size aittir ve kimsenin kodunuzu kullanma, kopyalama, değiştirme veya dağıtma izni yoktur.**

Yani, lisans eklemezseniz, projeniz "açık kaynak" olmaz. İnsanlar kodunuzu görebilir ama yasal olarak kullanamazlar. Bu nedenle, başkalarının projenizi kullanmasını ve ona katkıda bulunmasını istiyorsanız, bir açık kaynak lisansı seçmek **zorunludur**.

## 3\. Popüler Açık Kaynak Lisansları

Lisanslar genellikle "izin veren" (permissive) ve "kopyalamayı zorunlu kılan" (copyleft) olarak ikiye ayrılır. İşte en popüler üç lisansın basit açıklamaları:

### a. MIT Lisansı (Çok İzin Veren)

En basit ve en popüler lisanslardan biridir.

  - **Ne yapabilirler?:** Kodunuzla neredeyse her şeyi yapabilirler (kullanma, kopyalama, değiştirme, birleştirme, yayınlama, dağıtma, alt lisanslama ve/veya satma).
  - **Tek Şartı Nedir?:** Kodunuzu kullandıkları her yerde orijinal telif hakkı notunuzu ve lisans metnini eklemek zorundadırlar.
  - **Özellik:** Kodunuzu alıp kapalı kaynaklı (ticari) bir projede kullanabilirler.

**Kimler kullanır?** React, Angular, .NET, Node.js gibi projeler.

### b. Apache 2.0 Lisansı (İzin Veren ve Patent Korumalı)

MIT'ye benzer şekilde izin vericidir ancak daha detaylıdır ve ek korumalar sağlar.

  - **Ne yapabilirler?:** MIT'deki gibi neredeyse her şeyi yapabilirler.
  - **Şartları Nelerdir?:**
    1.  Orijinal telif hakkı ve lisans metnini eklemek zorundadırlar.
    2.  Kodda önemli bir değişiklik yaptılarsa, bunu belirtmek zorundadırlar.
    3.  **Patent Hakları:** Bu lisans, katkıda bulunanların patent haklarını kullanıcılara lisanslamasını sağlar, bu da şirketler için ek bir yasal koruma anlamına gelir.

**Kimler kullanır?** Android, Swift, Kubernetes, TensorFlow gibi büyük projeler.

### c. GNU GPLv3 Lisansı (Güçlü Copyleft)

"Özgür Yazılım" felsefesini en güçlü şekilde yansıtan lisanstır.

  - **Ne yapabilirler?:** Kodu kullanabilir, değiştirebilir ve dağıtabilirler.
  - **En Önemli Şartı Nedir?:** Eğer kodunuzu değiştirip yeni bir yazılım oluşturur ve bu yazılımı dağıtırlarsa, yeni yazılımın kaynak kodunu da **aynı GPLv3 lisansıyla açmak zorundadırlar.** Buna "copyleft" veya "viral lisans" denir.
  - **Özellik:** Bu lisans, kodunuzun ve ondan türetilen tüm çalışmaların her zaman açık kaynak kalmasını garanti eder.

**Kimler kullanır?** Linux Kernel (GPLv2), Git, GIMP, WordPress gibi projeler.

## 4\. Hangi Lisansı Seçmeliyim?

  - **"İnsanlar kodumla istediklerini yapsın, yeter ki benim adımı geçirsinler."** diyorsanız → **MIT Lisansı**
  - **"İnsanlar kodumla istediklerini yapsın ama büyük şirketler için patent koruması da olsun."** diyorsanız → **Apache 2.0 Lisansı**
  - **"Benim kodumu kullanan herkes, kendi projesini de açık kaynak yapmak zorunda kalsın. Özgürlük paylaştıkça çoğalır."** diyorsanız → **GNU GPLv3 Lisansı**

Yardıma ihtiyacınız varsa, GitHub'ın **[choosealicense.com](https://choosealicense.com/)** sitesi size adım adım doğru lisansı seçmenizde yardımcı olacaktır.

## 5\. Projeye Lisans Nasıl Eklenir?

GitHub, bu işlemi çok kolay hale getirmiştir:

1.  Projenizin ana sayfasına gidin.
2.  **`Add file`** (Dosya Ekle) butonuna tıklayın ve **`Create new file`** (Yeni dosya oluştur) seçeneğini seçin.
3.  Dosya adı alanına büyük harflerle `LICENSE` veya `LICENSE.md` yazın.
4.  Dosya adı alanının sağ tarafında **`Choose a license template`** (Bir lisans şablonu seç) butonu belirecektir. Bu butona tıklayın.
5.  Açılan sayfada, soldaki listeden istediğiniz lisansı (MIT, Apache 2.0, GPLv3 vb.) seçin.
6.  GitHub, sizin için lisans metnini otomatik olarak dolduracaktır. Genellikle sadece `[year]` (yıl) ve `[fullname]` (tam ad) alanlarını kontrol etmeniz yeterlidir.
7.  **`Review and submit`** (İncele ve gönder) butonuna tıklayın ve ardından değişiklikleri `commit`'leyin.

İşte bu kadar\! Projenizin artık yasal bir çerçevesi var ve resmi olarak açık kaynaklıdır.