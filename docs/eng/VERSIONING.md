# Versioning Guide
This document has been created to standardize and clarify version management
in projects. Based on the Semantic Versioning (SemVer) system, this structure
aims to track changes made during development in a clear and consistent
manner.

The document covers the following topics:

- [Semantic Versioning Rules:](#semantic-versioning-semver)
Differences between Major, Minor, and Patch versions and their usage 
criteria.

- [Universal Version Description Symbols:](#universal-version-description-symbols)
Standard symbols used to make release notes quick and easy to understand.

- [Version History Table:](#version-history-table)
A log system that allows tracking the development of this document step
by step.

## Semantic Versioning - SemVer

Version numbers are tracked in the `Major.Minor.Patch` format.

### Version Numbering Structure

| **Version Type**        | **Description**                                            | **Example**     |
|-------------------------|------------------------------------------------------------|-----------------|
| **Major Release**       | Contains major changes and backward incompatible updates.  | `0.1.1 → 1.0.0` |
| **Minor Release**       | New features added while maintaining backward compatibility. | `0.0.1 → 0.1.0` |
| **Patch Release**       | Contains bug fixes and minor improvements.                 | `0.0.0 → 0.0.1` |

### Versioning Rules

1. When the **Major release** is increased, it indicates that major,
backward-incompatible changes have been made.
2. When the **Minor release** is increased, it means new features have
been added, but backward compatibility has been maintained.
3. When the **Patch release** is increased, bug fixes or small performance
 improvements have been made.

---

📌 **Note:** This system is based on the widely used
[Semantic Versioning (SemVer)](https://semver.org/lang/en) standard.

[Back to Top](#versioning-guide)

---

## Universal Version Description Symbols

The following symbols are used to express version changes in a quick and clear way:

| **Symbol** | **Description** |
|------------|-----------------|
| **(+)**    | New features and content added. |
| **(~)**    | Fixes and improvements made to existing features or content. |
| **(-)**    | Existing features or content removed. |
| **(!)**    | This version contains incompatibilities. |
| **(?)**    | Experimental feature or content added. |
| **(#)**    | A mixed version containing multiple types of changes (e.g., additions, removals, experimental). |

## Example Usage 

**Versiyon Geçmiş Tablosu**

| **Versiyon** | **Tarih**  | **Katkıda Bulunan** | **Açıklama** |
|--------------|------------|---------------------|-----------------|
| 1.0.0        | 02.04.2025 | Uruz                | **(#)** Çeşitli büyük değişiklikler ve yeni özellikler eklendi. |
| 0.3.0        | 16.03.2025 | Utku                | **(?)** Deneysel özellik eklendi. |
| 0.2.0        | 01.03.2025 | Uruz                | **(+)** Yeni bir özellik eklendi. |
| 0.1.1        | 19.02.2025 | Utku                | **(~)** Mevcut özelliklerde iyileştirmeler yapıldı. |
| 0.1.0        | 13.02.2025 | Uruz                | **(+)** İlk resmi sürüm yayımlandı. |
| 0.0.1        | 12.02.2025 | Uruz                | İlk ham taslak oluşturuldu. |

### Purposes of Universal Symbols

- **Clarity:** Allows quickly understanding version changes.

- **Universal Usage:** The symbols carry the same meaning in every language.

- **Consistency:** Establishes a standardized version tracking method for all projects.

📌 **Note:** To create a more detailed document, each change type should be
specified separately. The `(#)` symbol should only be used for mixed versions
containing multiple change types.

[Back to Top](#versioning-guide)

---

***Translation***
\
*You can find the sources used for the translation below.*
* [Google Translate](https://translate.google.com/?hl=tr&sl=tr&tl=la&op=translate)
* [ChatGPT](https://chatgpt.com/)

---

## Version History Table

| **Version** | **Date**   | **Contributor** | **Description** |
|-------------|------------|-----------------|-----------------|
| 0.1.0       | 12.02.2025 | Uruz            | **(+)** First official release published. |
| 0.0.1       | 12.02.2025 | Uruz            | Initial draft created. |

[Back to Top](#versioning-guide)
