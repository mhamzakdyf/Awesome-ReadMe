# 🎖️ Rozetler ve Kalkanlar Rehberi (`Badges & Shields`)

Bu rehber, GitHub `README` dosyalarına profesyonel bir görünüm kazandıran ve projenizin durumu hakkında anında bilgi sağlayan **Rozetlerin (Badges)** nasıl ekleneceğini ve kullanılacağını açıklamaktadır. "Shields" (Kalkanlar) olarak da bilinen bu küçük görseller, projenizin teknik durumunu, lisansını ve daha fazlasını bir bakışta özetler.

## İçindekiler

1.  [Rozet Nedir ve Neden Kullanılır?](#1-rozet-nedir-ve-neden-kullanılır)
2.  [Rozet Nasıl Çalışır?](#2-rozet-nasıl-çalışır)
3.  [Rozet Oluşturma: Shields.io](#3-rozet-oluşturma-shieldsio)
4.  [Yaygın Rozet Türleri ve Örnekleri](#4-yaygın-rozet-türleri-ve-örnekleri)
5.  [Rozetleri README Dosyasına Ekleme](#5-rozetleri-readme-dosyasına-ekleme)
6.  [En İyi Kullanım Pratikleri](#6-en-i̇yi-kullanım-pratikleri)

-----

## 1\. Rozet Nedir ve Neden Kullanılır?

Rozetler, genellikle `README` dosyasının en üst kısmında yer alan, küçük, SVG formatında görsellerdir. Her biri, proje hakkında belirli bir metrik veya durumu (genellikle renk kodlu olarak) gösterir.

**Başlıca faydaları:**

  - **Anlık Bilgi:** Kullanıcılara ve potansiyel katkıda bulunanlara projenin mevcut durumu (örneğin, testlerin başarılı olup olmadığı) hakkında hızlı bir genel bakış sunar.
  - **Profesyonel İmaj:** İyi seçilmiş rozetler, projenin aktif olarak geliştirildiğini ve iyi bir şekilde yönetildiğini gösterir.
  - **Güvenilirlik:** Kod kalitesi, test kapsamı gibi metrikleri göstermek, projenin güvenilirliği konusunda olumlu bir izlenim bırakır.
  - **Standardizasyon:** Açık kaynak dünyasında bir standart haline gelmiştir ve projenizin diğer büyük projeler gibi görünmesini sağlar.

## 2\. Rozet Nasıl Çalışır?

Bir rozet, aslında basit bir **görsel linkidir**. Genellikle iki bölümden oluşur:

1.  **Görsel:** Projenin durumunu gösteren, dinamik olarak oluşturulmuş bir resim (`.svg` veya `.png`).
2.  **Link:** Bu görsele tıklandığında kullanıcıyı yönlendireceği hedef URL (örneğin, projenin test sonuçlarını gösteren detay sayfası).

Markdown sözdizimi şöyledir: `[![Rozet Metni](ROZET_GORSEL_URL)](HEDEF_URL)`

## 3\. Rozet Oluşturma: Shields.io

Rozet oluşturmak için en popüler ve kapsamlı servis **[Shields.io](https://shields.io/)**'dur. Bu servis, yüzlerce farklı platform (GitHub, npm, PyPI vb.) ile entegre olarak projeniz hakkında dinamik rozetler oluşturmanıza olanak tanır.

**Shields.io'yu kullanarak rozet oluşturmak için:**

1.  [Shields.io](https://shields.io/) web sitesine gidin.
2.  İhtiyacınız olan rozet türünü arayın (örneğin, "license", "GitHub issues").
3.  İlgili formu doldurun (genellikle GitHub kullanıcı adınız ve repo adınız istenir).
4.  Oluşturulan rozetin Markdown kodunu kopyalayın.

Ayrıca, statik rozetler de oluşturabilirsiniz. Örneğin:
`https://img.shields.io/badge/Proje-Aktif-brightgreen` linki şu rozeti oluşturur: 

## 4\. Yaygın Rozet Türleri ve Örnekleri

Aşağıda en sık kullanılan rozet türlerinden bazıları ve açıklamaları yer almaktadır.

| Tür | Açıklama | Örnek Rozet |
| :--- | :--- | :--- |
| **Build Status** | Projenin en son derleme (build) ve test durumunu gösterir. (Örn: GitHub Actions, Travis CI) |  |
| **License** | Projenin hangi açık kaynak lisansına sahip olduğunu belirtir. |  |
| **Version** | Projenin güncel sürümünü paket yöneticilerinden (npm, PyPI vb.) çeker. |  |
| **Code Coverage** | Testlerin kodun yüzde kaçını kapsadığını gösterir. (Örn: Codecov, Coveralls) |  |
| **Downloads** | Projenin ne kadar indirildiğini gösterir. |  |
| **Issues** | Açık olan "issue" (sorun/talep) sayısını gösterir. |  |
| **Social** | Projenin sosyal medya hesaplarına veya iletişim kanallarına link verir. |  |
| **Contributors** | Projeye katkıda bulunan kişi sayısını gösterir. |  |

## 5\. Rozetleri README Dosyasına Ekleme

Rozetler genellikle projenin ana başlığının hemen altına, yan yana hizalanmış bir şekilde eklenir.

```markdown
# Proje Adı

[![Build Status](...URL...)](...URL...) [![License](...URL...)](...URL...) [![Version](...URL...)](...URL...)

Projenin kısa açıklaması burada yer alır...
```

**Temiz bir görünüm için:** Rozetler arasına bir boşluk koyarak onları yan yana dizebilirsiniz.

## 6\. En İyi Kullanım Pratikleri

  - **Abartmayın:** `README` dosyanızı bir rozet panayırına çevirmekten kaçının. Sadece projeniz için gerçekten anlamlı ve önemli olan metrikleri gösteren rozetleri seçin. Genellikle 4 ila 8 arası rozet idealdir.
  - **Konumlandırma:** Rozetleri her zaman `README` dosyasının en üstüne, başlık ve kısa açıklamadan sonra yerleştirin. Bu standart bir pratiktir.
  - **Linkleri Ekleyin:** Rozetlerin sadece birer görsel olmasını önleyin. İlgili detay sayfasına link vermeleri, onları çok daha işlevsel hale getirir.
  - **Tutarlı Stil:** Mümkünse, [Shields.io](https://shields.io/)'nun sunduğu stil seçeneklerini (`style=flat`, `style=flat-square`, `style=plastic` vb.) kullanarak tüm rozetlerinizde tutarlı bir görünüm sağlayın.