# 🤝 Katkıda Bulunma Rehberi (`CONTRIBUTING.md`)

Bu rehber, projenize katkıda bulunmak isteyenler için bir yol haritası sunan standart `CONTRIBUTING.md` dosyasının nasıl oluşturulacağını açıklamaktadır. Bu dosya, topluluğunuzu büyütmenin, projenizin kalitesini artırmanın ve dışarıdan gelen katkıları düzenli bir şekilde yönetmenin anahtarıdır.

## İçindekiler

1.  [`CONTRIBUTING.md` Nedir ve Neden Hayatidir?](#1-contributingmd-nedir-ve-neden-hayatidir)
2.  [Katkıda Bulunma Rehberinin Ana Bölümleri](#2-katkıda-bulunma-rehberinin-ana-bölümleri)
3.  [Örnek `CONTRIBUTING.md` Şablonu](#3-örnek-contributingmd-şablonu)
4.  [En İyi Kullanım Pratikleri](#4-en-i̇yi-kullanım-pratikleri)

-----

## 1\. `CONTRIBUTING.md` Nedir ve Neden Hayatidir?

`CONTRIBUTING.md`, bir projeye nasıl katkı sağlanacağını adım adım anlatan bir belgedir. Potansiyel bir katkıcının bilmesi gereken her şeyi içerir: Hata raporu nasıl oluşturulur, yeni bir özellik nasıl önerilir, kodlama standartları nelerdir ve Pull Request (PR) süreci nasıl işler.

**Neden bu kadar önemli?**

  - **Yol Gösterir:** Katkıda bulunmak isteyen ancak nereden başlayacağını bilmeyen kişilere net bir yol haritası sunar.
  - **Kaliteyi Artırır:** Kodlama standartları ve test gereksinimleri gibi kurallar belirleyerek projenize gelen katkıların kalitesini yükseltir.
  - **Zaman Kazandırır:** Proje yöneticilerinin, her yeni katkıcıya süreci tekrar tekrar açıklamasını engeller.
  - **Topluluğu Teşvik Eder:** Açık ve davetkar bir katkı süreci, daha fazla insanın projeye dahil olmasını teşvik eder.

## 2\. Katkıda Bulunma Rehberinin Ana Bölümleri

İyi bir `CONTRIBUTING.md` dosyası genellikle şu bölümleri içerir:

1.  **Giriş:** Katkıda bulunma niyetiniz için bir teşekkür ve projenin genel hedeflerine kısa bir bakış.
2.  **Davranış Kuralları (`Code of Conduct`):** Proje topluluğunda uyulması gereken saygı ve iletişim kurallarına bir link.
3.  **Nasıl Katkıda Bulunabilirim?:** Katkı türlerinin (hata raporlama, özellik önerme, dokümantasyon yazma vb.) listesi.
4.  **Hata Raporlama (`Reporting Bugs`):** Bir hata raporu oluştururken hangi bilgilerin (sürüm, işletim sistemi, adımlar vb.) verilmesi gerektiğini açıklayan bölüm.
5.  **Özellik Önerme (`Suggesting Enhancements`):** Yeni bir özellik önerisi için izlenmesi gereken adımlar.
6.  **İlk Katkınız (`Your First Contribution`):** Özellikle yeni başlayanlar için projeyi fork'lama, branch oluşturma ve ilk commit'i atma adımları.
7.  **Pull Request Süreci (`Pull Request Process`):** Bir Pull Request açarken uyulması gereken kurallar (başlık formatı, testlerin çalıştırılması, kodun incelenmesi vb.).
8.  **Kodlama Standartları (`Styleguides`):** Projede kullanılan kod stili, isimlendirme kuralları ve diğer teknik standartlar.

## 3\. Örnek `CONTRIBUTING.md` Şablonu

Aşağıda, yukarıdaki bölümleri içeren, kopyalayıp kendi projenize göre düzenleyebileceğiniz genel bir şablon bulunmaktadır.

```markdown
# Proje Adı'na Katkıda Bulunma Rehberi

Projemize katkıda bulunmayı düşündüğünüz için çok teşekkür ederiz! Topluluğumuzun her bir üyesinin katkısı bizim için çok değerli.

Bu rehber, projemize sorunsuz bir şekilde katkıda bulunmanıza yardımcı olmak için hazırlanmıştır.

## Davranış Kuralları

Bu projenin tüm katılımcılarının [Davranış Kurallarımıza (`CODE_OF_CONDUCT.md`)](CODE_OF_CONDUCT.md) uyması beklenmektedir. Lütfen bu kuralları okuyup kabul ettiğinizden emin olun.

## Nasıl Katkıda Bulunabilirim?

Katkıda bulunmak için henüz spesifik bir fikriniz yoksa, projenin [Issues](https://github.com/kullanici/proje/issues) sekmesindeki `good first issue` veya `help wanted` etiketli görevlere göz atabilirsiniz.

### Hata mı Bildirmek İstiyorsunuz?

Hata bildirmeden önce, lütfen mevcut [Issues](https://github.com/kullanici/proje/issues) listesinde benzer bir raporun olup olmadığını kontrol edin. Yeni bir hata raporu oluştururken:
-   **Açık ve anlaşılır bir başlık** kullanın.
-   Hatanın **tekrarlanması için gereken adımları** detaylıca açıklayın.
-   **Beklenen davranış** ile **gerçekte olan davranış** arasındaki farkı belirtin.
-   Mümkünse, hatayı gösteren **ekran görüntüleri** veya GIF'ler ekleyin.

### Yeni Bir Özellik mi Önermek İstiyorsunuz?

Yeni bir özellik önerisi, projenin geleceği için harika bir adımdır! Öneri yapmadan önce:
1.  Benzer bir önerinin daha önce yapılıp yapılmadığını [Issues](https://github.com/kullanici/proje/issues) bölümünde arayın.
2.  Yeni bir "Issue" oluşturun ve önerinizi detaylı bir şekilde açıklayın. Bu, özelliğin projenin vizyonuyla uyumlu olup olmadığını tartışmamıza olanak tanır.

## Pull Request (PR) Süreci

1.  **Fork & Clone:** Projeyi kendi hesabınıza `Fork` edin ve ardından bilgisayarınıza `clone` edin.
2.  **Branch Oluşturma:** Yeni çalışmanız için açıklayıcı bir isme sahip yeni bir `branch` oluşturun (`git checkout -b ozellik/harika-bir-ozellik`).
3.  **Değişiklikleri Yapma:** Kodunuzu yazın ve projenin kodlama standartlarına uyduğunuzdan emin olun.
4.  **Commit Atma:** Değişikliklerinizi anlamlı `commit` mesajları ile kaydedin.
5.  **Push Etme:** Oluşturduğunuz `branch`'i kendi fork'unuza `push` edin (`git push origin ozellik/harika-bir-ozellik`).
6.  **PR Oluşturma:** GitHub üzerinden projemizin ana deposuna bir `Pull Request` oluşturun. PR açıklamasında yaptığınız değişiklikleri ve nedenlerini net bir şekilde açıklayın.

PR'ınız, proje yöneticileri tarafından incelendikten ve gerekli testleri geçtikten sonra ana branch ile birleştirilecektir.

## Kodlama Standartları

-   Tüm kodlar [Prettier](https://prettier.io/) ile formatlanmalıdır.
-   Değişken isimlendirmeleri için `camelCase` kullanın.
-   Eklediğiniz her yeni fonksiyon için yorum satırları eklemeye özen gösterin.

Katkılarınız için şimdiden teşekkürler! 🚀
```

## 4\. En İyi Kullanım Pratikleri

  - **Erişilebilir Olun:** `README.md` dosyanızın en üstüne veya "Katkıda Bulunma" bölümüne `CONTRIBUTING.md` dosyanıza bir link ekleyin.
  - **Basit ve Davetkar Bir Dil Kullanın:** Özellikle yeni başlayanları korkutacak karmaşık bir dil kullanmaktan kaçının.
  - **Şablonlar Kullanın:** Hata raporları ve özellik önerileri için GitHub'ın "Issue Templates" özelliğini kullanarak süreci standartlaştırın.
  - **Güncel Tutun:** Projenizin yapısı veya katkı süreci değiştikçe bu dosyayı güncellemeyi unutmayın.