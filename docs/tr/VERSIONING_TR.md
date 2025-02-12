# Sürümleme Rehberi
Bu belge, projelerde sürüm yönetimini standartlaştırmak ve anlaşılır hale
getirmek için oluşturulmuştur. Semantik (SemVer) sistemini temel alan bu 
yapı, geliştirme sürecinde yapılan değişiklikleri açık ve tutarlı bir 
şekilde takip etmeyi amaçlar.

Belgede aşağıdaki konular ele alınmaktadır:

- [Semantik Sürümleme Kuralları:](#semantik-mantıksal-sürümleme---semver)
Major, Minor ve Patch sürümleri arasındaki farklar ve kullanım kriterleri.

- [Evrensel Sürüm Açıklama Sembolleri:](#evrensel-sürüm-açıklama-sembolleri)
Sürüm notlarını hızlı ve anlaşılır hale getirmek için kullanılan standart
semboller.

- [Sürüm Geçmiş Tablosu:](#sürüm-geçmiş-tablosu)
Bu belgenin gelişimini adım adım takip etmeyi sağlayan kayıt sistemi.

## Semantik (Mantıksal) Sürümleme - SemVer

Sürüm numaraları `Ana.Alt.Yama` (`Major.Minor.Patch`) formatında takip 
edilir.

### Sürüm Numaralandırma Yapısı

| **Sürüm Tipi**         | **Açıklama**                                              | **Örnek**      |
|------------------------|-----------------------------------------------------------|----------------|
| **Ana Sürüm (Major)**  | Büyük değişiklikler ve geriye dönük uyumsuzluklar içerir. | `0.1.1 → 1.0.0` |
| **Alt Sürüm (Minor)**  | Yeni özellikler eklenir, ancak geriye dönük uyumluluk korunur.| `0.0.1 → 0.1.0` |
| **Yama Sürüm (Patch)** | Küçük hata düzeltmeleri ve iyileştirmeler içerir.         | `0.0.0 → 0.0.1` |

### Sürümleme Kuralları

1. **Ana sürüm (Major) arttırıldığında**, önceki sürümlerle uyumsuz büyük
değişiklikler yapılmış demektir.
2. **Alt sürüm (Minor) arttırıldığında**, yeni özellikler eklenmiş ancak 
eski sürümlerle uyum korunmuştur.
3. **Yama sürüm (Patch) arttırıldığında**, hata düzeltmeleri veya küçük 
performans iyileştirmeleri yapılmıştır.

---

📌 **Not:** Bu sistem, yaygın olarak kullanılan
[Semantik Sürümleme (SemVer)](https://semver.org/lang/tr)
standardına dayanmaktadır.

[Başa Dön](#sürümleme-rehberi)

---

## Evrensel Sürüm Açıklama Sembolleri

Sürüm değişikliklerini hızlı ve net bir şekilde ifade etmek için aşağıdaki
semboller kullanılır:

| **Sembol** | **Açıklama** |
|------------|--------------|
| **(+)**    | Yeni özellik ve içerik eklendi. |
| **(~)**    | Mevcut özellik veya içerikte düzeltmeler ve iyileştrilmeler yapıldı.|
| **(-)**    | Mevcut özellik veya içerik kaldırıldı. |
| **(!)**    | Bu sürümde uyumsuzluklar mevcut.
| **(?)**    | Deneysel özellik veya içerik eklendi.
| **(#)**    | Birden fazla değişiklik kategorisini (ekleme, kaldırma, deneysel vb.) içeren karma sürüm. |

## Örnek Kullanım 

**Version History Table**

| **Version** | **Date**      | **Contributor**     | **Description** |
|-------------|---------------|---------------------|-----------------|
| 1.0.0       | 02.04.2025    | Uruz                | **(#)** Various major changes and new features added. |
| 0.3.0       | 16.03.2025    | Utku                | **(?)** Experimental feature added. |
| 0.2.0       | 01.03.2025    | Uruz                | **(+)** A new feature added. |
| 0.1.1       | 19.02.2025    | Utku                | **(~)** Improvements made to existing features. |
| 0.1.0       | 13.02.2025    | Uruz                | **(+)** First official release published. |
| 0.0.1       | 12.02.2025    | Uruz                | Initial draft created. |

### Evrensel Sembollerin Amaçları

- **Anlaşılabilirlik:** Sürüm değişikliklerini hızlıca kavramayı sağlar.

- **Evrensel Kullanım:** Evrensel semboller sayesinde her dilde aynı anlamı
taşır.

- **Tutarlılık Sağlamak**: Tüm projelerde standart bir sürüm takip yöntemi
oluşturur.

📌 **Not:** Daha ayrıntılı bir belge oluşturmak için her değişiklik türü ayrı
ayrı belirtilmelidir. `(#)` sembolü, yanlızca birden fazla değişiklik türü
içeren karma sürümler için kullanılmalıdır.

[Başa Dön](#sürümleme-rehberi)

---

## Sürüm Geçmiş Tablosu

| **Sürüm** | **Tarih**  | **Katkıda Bulunan** | **Açıklama** |
|-----------|------------|---------------------|--------------|
| 0.1.0     | 12.02.2025 | Uruz                | **(+)** İlk resmi sürüm yayımlandı. |
| 0.0.1     | 12.02.2025 | Uruz                | İlk ham taslak oluşturuldu. |

[Başa Dön](#sürümleme-rehberi)