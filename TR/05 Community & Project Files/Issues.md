# 📄 Şablonlar Rehberi (`Issue & PR Templates`)

Bu rehber, projenize gelen hata bildirimlerini (Issues) ve kod katkılarını (Pull Requests) standartlaştırmak için kullanılan **Şablonların (Templates)** nasıl oluşturulacağını ve kullanılacağını açıklamaktadır. Bu şablonlar, katkıda bulunanları doğru bilgileri sağlamaya yönlendirir ve proje bakımını çok daha verimli hale getirir.

## İçindekiler

1.  [Şablonlar Nedir ve Neden Çok Önemlidir?](#1-şablonlar-nedir-ve-neden-çok-önemlidir)
2.  [Nasıl Çalışırlar? `.github` Klasörünün Rolü](#2-nasıl-çalışırlar-github-klasörünün-rolü)
3.  [Issue Şablonları Oluşturma](#3-issue-şablonları-oluşturma)
4.  [Pull Request Şablonu Oluşturma](#4-pull-request-şablonu-oluşturma)
5.  [En İyi Kullanım Pratikleri](#5-en-i̇yi-kullanım-pratikleri)

-----

## 1\. Şablonlar Nedir ve Neden Çok Önemlidir?

Issue ve Pull Request (PR) şablonları, bir kullanıcı yeni bir issue veya PR oluşturmaya başladığında, açıklama alanına otomatik olarak yüklenen önceden hazırlanmış Markdown metinleridir.

**Başlıca faydaları:**

  - **Eksiksiz Bilgi:** Kullanıcıları, sorunu anlamak için gereken tüm temel bilgileri (sürüm, işletim sistemi, adımlar vb.) sağlamaya teşvik eder. "Çalışmıyor" gibi yetersiz bildirimleri engeller.
  - **Standardizasyon:** Tüm bildirimlerin ve katkıların aynı formatta gelmesini sağlayarak onları incelemeyi ve yönetmeyi kolaylaştırır.
  - **Zaman Verimliliği:** Proje yöneticilerinin, her seferinde aynı temel soruları sormak için harcadığı zamandan tasarruf etmesini sağlar.
  - **Süreci Yönlendirme:** Bir PR şablonu, katkıda bulunanlara testleri çalıştırıp çalıştırmadıkları veya dokümantasyonu güncelleyip güncellemedikleri gibi önemli adımları hatırlatan bir kontrol listesi (checklist) sunar.

## 2\. Nasıl Çalışırlar? `.github` Klasörünün Rolü

GitHub, bir projenin kök dizininde `.github` adında özel bir klasör arar. Bu klasörün içine belirli isimlerde dosyalar veya alt klasörler koyduğunuzda, GitHub bunları otomatik olarak algılar ve ilgili özellikleri etkinleştirir. Issue ve PR şablonları da bu klasörün içinde yaşar.

## 3\. Issue Şablonları Oluşturma

Kullanıcıların farklı amaçlar için (hata bildirme, özellik önerme) farklı şablonlar seçebilmesini sağlamak en iyi pratiktir.

### Klasör Yapısı

Projenizin kök dizininde şu yapıyı oluşturun:

```
.github/
└── ISSUE_TEMPLATE/
    ├── bug_report.md
    ├── feature_request.md
    └── config.yml
```

### a. Hata Raporu Şablonu (`bug_report.md`)

Bu şablon, bir hatayı yeniden oluşturmak için gereken tüm bilgileri ister.

```markdown
---
name: 🐞 Hata Raporu (Bug Report)
about: Projede bir hata bulduysanız bunu bildirmek için kullanın.
title: "[HATA] Kısa ve açıklayıcı bir başlık yazın"
labels: 'bug'
assignees: ''

---

**Hatanın Açıklaması**
Hatanın ne olduğu hakkında açık ve net bir açıklama yapın.

**Tekrarlama Adımları**
Hatanın nasıl tekrarlanabileceğini adım adım açıklayın:
1. '...' sayfasına gidin.
2. '...' butonuna tıklayın.
3. Aşağı kaydırın ve '...' görün.
4. Hata burada beliriyor.

**Beklenen Davranış**
Normalde ne olmasını beklediğinizi açıkça belirtin.

**Ekran Görüntüleri**
Mümkünse, hatayı anlamamıza yardımcı olacak ekran görüntüleri ekleyin.

**Teknik Ortam (Lütfen bu bilgileri doldurun):**
 - İşletim Sistemi: [örn. Windows 10, macOS Sonoma]
 - Tarayıcı (eğer uygulanabilirse): [örn. Chrome, Firefox]
 - Proje Versiyonu: [örn. v1.2.3]

**Ek Bilgiler**
Sorunla ilgili eklemek istediğiniz başka bir bağlam var mı?
```

### b. Özellik Önerisi Şablonu (`feature_request.md`)

Bu şablon, yeni bir fikir veya geliştirme önerisi için kullanılır.

```markdown
---
name: ✨ Özellik Önerisi (Feature Request)
about: Proje için yeni bir fikir veya geliştirme önerin.
title: "[ÖNERİ] Kısa ve açıklayıcı bir başlık yazın"
labels: 'enhancement'
assignees: ''

---

**Öneriniz bir problemle mi ilgili? Lütfen açıklayın.**
Örneğin: "Sürekli X işlemini yapmak zorunda kalıyorum ve bu çok zaman alıyor, keşke Y özelliği olsa..." gibi bir açıklama yapın.

**Çözüm Öneriniz**
Bu sorunu çözeceğini düşündüğünüz özelliği veya geliştirmeyi net bir şekilde açıklayın.

**Düşündüğünüz Alternatifler**
Bu sorunu çözebilecek başka çözümler veya özellikler düşündünüz mü?

**Ek Bilgiler**
Önerinizle ilgili eklemek istediğiniz başka bir bağlam, ekran görüntüsü veya örnek var mı?
```

### c. Yapılandırma Dosyası (`config.yml`)

Bu dosya, kullanıcı "New issue" butonuna tıkladığında hangi seçenekleri göreceğini belirler.

```yaml
blank_issues_enabled: false
contact_links:
  - name: 💬 Topluluk Tartışmaları
    url: https://github.com/kullanici/proje/discussions
    about: Lütfen özellik önermek veya hata bildirmek dışındaki genel sorular için Tartışmalar bölümünü kullanın.
```

## 4\. Pull Request Şablonu Oluşturma

PR şablonu, katkıda bulunanların gerekli kontrolleri yaptığından emin olmanıza yardımcı olur.

### Dosya Yeri ve Adı

Projenizin kök dizininde şu dosyayı oluşturun: `.github/PULL_REQUEST_TEMPLATE.md`

### Örnek `PULL_REQUEST_TEMPLATE.md`

```markdown
## 🎯 Bu PR Ne Hakkında?
- 
- 
- 

## 🔗 İlgili Issue
Closes #

## 📸 Ekran Görüntüleri (Eğer Varsa)
##  checklist:
- [ ] Kodum, projenin kodlama standartlarına uyuyor.
- [ ] Değişikliklerim için gerekli testleri yazdım ve çalıştırdım.
- [ ] İlgili dokümantasyonu güncelledim.
- [ ] Değişikliklerim yeni bir uyarı (warning) oluşturmuyor.
```

## 5\. En İyi Kullanım Pratikleri

  - **Açık ve Basit Olun:** Şablonlarınızdaki dilin anlaşılır ve takip etmesi kolay olduğundan emin olun.
  - **Zorunlu ve Opsiyonel Alanları Belirtin:** Kullanıcıların hangi bilgileri mutlaka vermesi gerektiğini netleştirin.
  - **Yönlendirme Yapın:** `config.yml` kullanarak, genel sorular için kullanıcıları "Discussions" veya diğer iletişim kanallarına yönlendirin.
  - **Güncel Tutun:** Projenizin süreci değiştikçe şablonlarınızı güncellemeyi unutmayın.