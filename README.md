# Kerim's PDF Tools - QPDF ULTRA FAST V4

[![Version](https://img.shields.io/badge/version-4.0-blue.svg)](https://github.com/yourusername/kerim-pdf-tools)
[![PowerShell](https://img.shields.io/badge/PowerShell-5.1%2B-blueviolet.svg)](https://github.com/PowerShell/PowerShell)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)](https://www.microsoft.com/en-us/windows)

> **Free, efficient PDF merge and compress tool. Merges and compresses PDF files better than any online services.**

---

<img width="1063" height="752" alt="image" src="https://github.com/user-attachments/assets/3cc21681-bdd6-4fb9-a06c-c89e9d9f4052" />


<img width="1224" height="653" alt="image" src="https://github.com/user-attachments/assets/031e792c-fa1b-46f9-977b-caffd5e8becb" />

<img width="1063" height="752" alt="image" src="https://github.com/user-attachments/assets/966a5cdc-dfbd-49ed-b997-def997ec294b" />

<img width="1086" height="768" alt="image" src="https://github.com/user-attachments/assets/bc058f81-238a-466b-bf74-2e8613a8b133" />


## 📋 Table of Contents

- [Quick Start](#-quick-start)
- [Overview](#-overview)
- [Core Features](#-core-features)
- [UI/UX Features](#-uiux-features)
- [Technical Advantages](#-technical-advantages)
- [User Experience Advantages](#-user-experience-advantages)
- [Innovative Features](#-innovative-features)
- [Use Cases](#-use-cases)
- [Performance Metrics](#-performance-metrics)
- [Competitive Advantages](#-competitive-advantages)
- [Future Potential](#-future-potential)
- [Summary](#-summary)
- [Key Selling Points](#-key-selling-points)

---

## 🚀 Quick Start

### Download & Run

1. **Download** the latest release from the [Releases](https://github.com/yourusername/kerim-pdf-tools/releases) section
2. **Unpack** the archive to your Desktop (or any folder)
3. **Run** `Start.bat` file
4. **GUI** will appear - Enjoy! 🎉

### System Requirements

- **OS**: Windows 10, Windows 11 (fully tested)
- **No installation required** - Portable application
- **No admin rights needed** - Run as regular user

---

## 📋 Overview

**Kerim's PDF Tools** is a comprehensive, GUI-based PDF manipulation suite built with PowerShell and Windows Forms. It leverages **QPDF**, **Ghostscript**, and **PDFtk** for ultra-fast PDF processing with enterprise-grade features.

### Built With

| Tool | Purpose | Location |
|------|---------|----------|
| **QPDF** | Ultra-fast PDF operations | `LIBS\qpdf\` |
| **PDFtk** | Fallback PDF operations | `LIBS\PDFtk Server\` |
| **Ghostscript** | Compression & preview | `LIBS\gs\` |
| **PowerShell** | GUI & logic | `LIBS\guipdf.ps1` |

---

## 🔧 Core Features

### 1. **PDF Merge (Ultra-Fast)**
- ⚡ **QPDF Engine**: Merges hundreds of pages in milliseconds
- 📂 **Multiple Input Methods**: Browse, drag & drop, clipboard paste
- 🎨 **Preview System**: First-page thumbnail generation
- 📊 **Statistics**: Real-time file count and total size tracking
- 📝 **Import/Export**: TXT file list support for batch operations
- 🔄 **Order Control**: Move Up/Down with visual feedback
- 📁 **Smart Compression**: Optional post-merge compression

### 2. **PDF Split**
- 🎯 **Two Splitting Modes**:
  - **Manual Range**: Custom page ranges (e.g., `1-3, 4-6, 7-10`)
  - **Auto Split**: Automatically split every N pages
- 📊 **Intelligent Detection**: Auto-detects page count
- 📂 **Batch Processing**: Split entire PDFs in one operation
- 🔄 **Progress Tracking**: Real-time status updates
- 📁 **Auto-Open**: Automatically opens output folder

### 3. **PDF Encryption (AES-256)**
- 🛡️ **Military-Grade Security**: 256-bit AES encryption
- 🔑 **Two-Tier Password System**:
  - **User Password**: Required to open the file
  - **Owner Password**: Required to change permissions
- 📋 **Granular Permissions Control**:
  - Printing (Full/Low/None)
  - Document modification
  - Content extraction
  - Accessibility features
  - Annotation/commenting
  - Form filling
  - Document assembly
- 🔍 **Debug Console**: Detailed logging for troubleshooting

### 4. **Smart PDF Compression**
- 🤖 **AI-Like Content Analysis**:
  - Text extraction analysis
  - Image detection
  - Mixed content identification
  - Page count detection
  - File size analysis
- 🎯 **6 Compression Methods**:

| Method | Best For | Compression Rate |
|--------|----------|------------------|
| **Smart Auto** | All documents | 50-90% |
| **Image Optimized** | Image-heavy PDFs | 60-80% |
| **Font Subset** | Text documents | 90%+ |
| **Balanced** | Mixed content | 40-70% |
| **Rebuild from Text** | Corrupted PDFs | Varies |
| **Maximal + PDFtk Strip** | Maximum compression | 95%+ |

---

## 🎨 UI/UX Features

### **Modern Interface**
- Clean, professional design with color-coded sections
- Tabbed interface for easy navigation
- Real-time status updates
- Animated "Working..." dialog with marquee progress bar
- Professional color scheme (Blues, Greens, Purples, Oranges)

### **File Management**
- **Multiple input methods**:
  - Browse files
  - Browse folders (recursive PDF scanning)
  - Drag & drop
  - Clipboard paste (Ctrl+V)
  - **Import/Export TXT file lists**
  - Copy selected paths (Ctrl+C)
  - Delete keys

### **Context Menu**
- Open files
- Paste files/paths
- Copy selected paths
- **Import list from TXT file**
- **Export list to TXT file**
- Remove selected
- Clear all

### **Preview System**
- First page thumbnail preview
- Ghostscript-powered rendering
- Zoom to fit display
- Status indicators

---

## 🛠️ Technical Advantages

### **Performance**
- **Ultra-fast**: QPDF engine handles large PDFs in milliseconds
- **Multi-threaded**: Responsive UI during processing
- **Memory efficient**: Processes files without loading entire PDFs into memory
- **Batch processing**: Handle hundreds of files simultaneously

### **Reliability**
- **Fallback mechanisms**: QPDF → PDFtk fallback for merging
- **Error handling**: Comprehensive try-catch blocks
- **Debug console**: Detailed logging for troubleshooting
- **Validation**: File existence checks, valid PDF verification

### **Compatibility**
- **Cross-version support**: PDF versions 1.4 - 1.7
- **Input formats**: Standard PDF, encrypted PDFs
- **Output formats**: PDF, TXT (for file lists)
- **Unicode support**: Full international character support

### **Tool Detection**
- **Recursive scanning**: Automatically finds tools in LIBS folder
- **Multiple tool paths**: Supports various installation structures
- **Fallback detection**: PATH environment variable search

### **Security**
- **AES-256 encryption**: Government-grade security
- **Permission management**: Fine-grained access control
- **Password protection**: Dual password system
- **Secure processing**: Temporary file cleanup

---

## 📊 User Experience Advantages

### **Ease of Use**
- **One-click operations**: Merge, split, encrypt, compress
- **Intuitive interface**: Clear labeling and organization
- **Visual feedback**: Status updates and progress indicators
- **Keyboard shortcuts**: Ctrl+V, Ctrl+C, Delete

### **Productivity Boost**
- **Batch operations**: Process multiple files at once
- **Folder scanning**: Auto-add all PDFs from a folder
- **TXT import/export**: Share file lists across sessions
- **Auto-split**: Split all pages with one click

### **Accessibility**
- **Multi-language support**: Language file support (.lang)
- **Keyboard navigation**: Full keyboard support
- **Clear messaging**: Informative error and success messages
- **Tool tips**: Contextual help

---

## 💡 Innovative Features

### **Smart Auto-Compression**
The tool analyzes PDF content to determine the optimal compression method:
- **Text-only PDFs**: Uses aggressive font subsetting
- **Image-heavy PDFs**: Applies quality-adjusted image compression
- **Mixed content**: Balances text and image optimization
- **Scanned documents**: Applies specialized image compression

### **Two-Mode Splitting**
- **Custom ranges**: Exact control over page extraction
- **Auto-chunking**: Split large PDFs into manageable chunks

### **Dual-Password Encryption**
- **User password**: Controls document access
- **Owner password**: Controls document permissions
- **Flexible security**: Use one or both passwords

---

## 🚀 Use Cases

### **For Professionals**
- **Legal**: Merge exhibits, split large documents, encrypt sensitive files
- **Publishing**: Compress high-res PDFs, extract pages
- **Education**: Split lecture materials, merge assignments
- **Government**: Secure document encryption, PDF processing

### **For Personal Use**
- **Photo albums**: Compress large image PDFs
- **E-books**: Split books into chapters
- **Scanned documents**: Optimize and organize
- **Secure sharing**: Password-protect personal documents

---

## 📈 Performance Metrics

| Operation | Typical Speed | Technology |
|-----------|---------------|------------|
| Merge 100 PDFs | < 1 second | QPDF |
| Split 500-page PDF | 2-3 seconds | QPDF |
| AES-256 Encryption | 5-10 seconds | QPDF |
| Compression (Image) | 15-30 seconds | Ghostscript |
| Compression (Text) | 5-10 seconds | Ghostscript |
| Preview Generation | < 1 second | Ghostscript |

---

## 🎯 Competitive Advantages

### **Versus Online Tools**
- ✅ No file size limits
- ✅ No internet required
- ✅ Unlimited processing
- ✅ No privacy concerns
- ✅ Batch processing
- ✅ Multiple output formats
- ✅ **Better compression quality**

### **Versus Desktop Alternatives**
- ✅ Free and open-source
- ✅ Lightweight (no heavy dependencies)
- ✅ No installation required
- ✅ Ultra-fast processing
- ✅ Enterprise-grade encryption
- ✅ **More efficient than paid tools**

---

## 🔮 Future Potential

### **Potential Enhancements**
- **Batch processing**: Process multiple operations in sequence
- **OCR integration**: Add optical character recognition
- **Cloud integration**: Direct cloud storage support
- **Watermarking**: Add text/image watermarks
- **Digital signatures**: Sign PDF documents
- **Metadata editing**: Modify PDF properties
- **Form extraction**: Extract form field data
- **Page rotation**: Batch page rotation

---

## 📋 Summary

**Kerim's PDF Tools - QPDF ULTRA FAST V4** is a **professional-grade PDF manipulation suite** that combines:

- **Enterprise performance** with QPDF's ultra-fast engine
- **Military-grade security** with AES-256 encryption
- **Professional features** including smart compression and two-mode splitting
- **User-friendly interface** with modern UI and intuitive controls
- **Zero cost** - completely free and open-source
- **Privacy-focused** - processes entirely offline
- **Better results** than any online service

**Perfect for**: Legal professionals, publishers, educators, government agencies, and anyone needing fast, secure PDF processing without the cloud privacy concerns.

---

## ⭐ Key Selling Points

1. **ULTRA FAST**: Merges in milliseconds, not minutes
2. **100% FREE**: No hidden costs, no subscriptions
3. **OFFLINE**: Process sensitive documents securely
4. **AES-256**: Military-grade encryption
5. **SMART COMPRESSION**: AI-like content analysis
6. **NO INSTALLATION**: Portable executable
7. **BATCH PROCESSING**: Handle hundreds of files
8. **PROFESSIONAL UI**: Clean, modern interface
9. **BETTER THAN ONLINE**: Superior compression quality
10. **WINDOWS 10/11**: Fully tested and optimized

---

## 📦 Download

### Latest Release
[![Download](https://img.shields.io/badge/Download-Latest_Release-blue.svg)](https://github.com/yourusername/kerim-pdf-tools/releases/latest)

### Installation Steps
1. Download the archive from the [Releases](https://github.com/yourusername/kerim-pdf-tools/releases) section
2. Unpack to any folder (recommended: Desktop)
3. Run `Start.bat`
4. The GUI will appear - ready to use!

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

### Official Binaries Used
- **QPDF** - The core PDF processing engine (`LIBS\qpdf\`)
- **Ghostscript** - PDF compression and preview generation (`LIBS\gs\`)
- **PDFtk** - Fallback tool for PDF operations (`LIBS\PDFtk Server\`)

### GUI Technology
- **PowerShell** - The GUI and logic (`LIBS\guipdf.ps1`)

### Credits
- **Tural** - Creator and main developer
- **Kerim** - Inspiration and dedication

---

**Made with ❤️ for the PDF community**

*"Processing PDFs at the speed of thought"* ⚡

---





# Kerim's PDF Tools - QPDF ULTRA FAST V4

[![Version](https://img.shields.io/badge/version-4.0-blue.svg)](https://github.com/yourusername/kerim-pdf-tools)
[![PowerShell](https://img.shields.io/badge/PowerShell-5.1%2B-blueviolet.svg)](https://github.com/PowerShell/PowerShell)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)](https://www.microsoft.com/en-us/windows)

> **Pulsuz, sürətli PDF birləşdirmə və sıxışdırma aləti. PDF fayllarını istənilən onlayn xidmətlərdən daha yaxşı birləşdirir və sıxışdırır.**

---

<img width="1063" height="752" alt="image" src="https://github.com/user-attachments/assets/3cc21681-bdd6-4fb9-a06c-c89e9d9f4052" />

<img width="1224" height="653" alt="image" src="https://github.com/user-attachments/assets/031e792c-fa1b-46f9-977b-caffd5e8becb" />

<img width="1063" height="752" alt="image" src="https://github.com/user-attachments/assets/966a5cdc-dfbd-49ed-b997-def997ec294b" />

<img width="1086" height="768" alt="image" src="https://github.com/user-attachments/assets/bc058f81-238a-466b-bf74-2e8613a8b133" />


## 📋 Mündəricat

- [Sürətli Başlanğıc](#-sürətli-başlanğıc)
- [Ümumi Baxış](#-ümumi-baxış)
- [Əsas Xüsusiyyətlər](#-əsas-xüsusiyyətlər)
- [UI/UX Xüsusiyyətləri](#-uiux-xüsusiyyətləri)
- [Texniki Üstünlüklər](#-texniki-üstünlüklər)
- [İstifadəçi Təcrübəsi Üstünlükləri](#-istifadəçi-təcrübəsi-üstünlükləri)
- [İnnovativ Xüsusiyyətlər](#-innovativ-xüsusiyyətlər)
- [İstifadə Halları](#-istifadə-halları)
- [Performans Göstəriciləri](#-performans-göstəriciləri)
- [Rəqabət Üstünlükləri](#-rəqabət-üstünlükləri)
- [Gələcək Potensial](#-gələcək-potensial)
- [Xülasə](#-xülasə)
- [Əsas Satış Nöqtələri](#-əsas-satış-nöqtələri)

---

## 🚀 Sürətli Başlanğıc

### Yüklə və İşə Sal

1. **Son buraxılışı** [Releases](https://github.com/yourusername/kerim-pdf-tools/releases) bölməsindən yükləyin
2. **Arxivi** İş masasına (və ya istənilən qovluğa) açın
3. `Start.bat` faylını işə salın
4. **GUI** açılacaq - Zövq alın! 🎉

### Sistem Tələbləri

- **ƏS**: Windows 10, Windows 11 (tam test edilib)
- **Quraşdırma tələb olunmur** - Portativ proqram
- **Admin hüquqları tələb olunmur** - Adi istifadəçi kimi işlədin

---

## 📋 Ümumi Baxış

**Kerim's PDF Tools** PowerShell və Windows Forms ilə qurulmuş hərtərəfli, GUI əsaslı PDF manipulyasiya dəstidir. Ultra-sürətli PDF emalı üçün **QPDF**, **Ghostscript** və **PDFtk** istifadə edir.

### Hansı Alətlərlə Qurulub

| Alət | Məqsəd | Yerləşdiyi Yer |
|------|--------|----------------|
| **QPDF** | Ultra-sürətli PDF əməliyyatları | `LIBS\qpdf\` |
| **PDFtk** | Ehtiyat PDF əməliyyatları | `LIBS\PDFtk Server\` |
| **Ghostscript** | Sıxışdırma və önbaxış | `LIBS\gs\` |
| **PowerShell** | GUI və məntiq | `LIBS\guipdf.ps1` |

---

## 🔧 Əsas Xüsusiyyətlər

### 1. **PDF Birləşdirmə (Ultra-Sürətli)**
- ⚡ **QPDF Mühərriki**: Yüzlərlə səhifəni millisaniyələr ərzində birləşdirir
- 📂 **Çoxlu Daxiletmə Metodları**: Baxış, sürüşdür & burax, clipboard yapışdır
- 🎨 **Önbaxış Sistemi**: İlk səhifənin kiçik şəkli
- 📊 **Statistika**: Fayl sayı və ümumi ölçü izləmə
- 📝 **İdxal/İxrac**: Toplu əməliyyatlar üçün TXT fayl siyahısı
- 🔄 **Sıra Nəzarəti**: Yuxarı/Aşağı hərəkət et
- 📁 **Ağıllı Sıxışdırma**: Birləşdirmədən sonra sıxışdırma (isteğe bağlı)

### 2. **PDF Bölmə**
- 🎯 **İki Bölmə Rejimi**:
  - **Əl ilə Aralıq**: İstifadəçi səhifə aralıqları (məsələn, `1-3, 4-6, 7-10`)
  - **Avtomatik Bölmə**: Hər N səhifədən bir avtomatik böl
- 📊 **Ağıllı Deteksiya**: Səhifə sayını avtomatik müəyyən edir
- 📂 **Toplu Emal**: Bütün PDF-i bir əməliyyatda böl
- 🔄 **Proqres İzləmə**: Real vaxt status yeniləmələri
- 📁 **Avtomatik Açma**: Çıxış qovluğunu avtomatik açır

### 3. **PDF Şifrələmə (AES-256)**
- 🛡️ **Hərbi Səviyyəli Təhlükəsizlik**: 256-bit AES şifrələmə
- 🔑 **İki Səviyyəli Parol Sistemi**:
  - **İstifadəçi Parolu**: Faylı açmaq üçün tələb olunur
  - **Sahib Parolu**: İcazələri dəyişmək üçün tələb olunur
- 📋 **İncə İcazə Nəzarəti**:
  - Çap (Tam/Aşağı/Heç)
  - Sənəd dəyişiklikləri
  - Məzmun çıxarılması
  - Əlçatanlıq xüsusiyyətləri
  - Qeyd/şərh əlavə etmək
  - Forma doldurma
  - Sənəd montajı
- 🔍 **Debug Konsolu**: Problemlərin aradan qaldırılması üçün ətraflı qeyd

### 4. **Ağıllı PDF Sıxışdırma**
- 🤖 **Süni İntellektə Bənzər Məzmun Analizi**:
  - Mətn çıxarılması analizi
  - Şəkil deteksiyası
  - Qarışıq məzmun identifikasiyası
  - Səhifə sayı deteksiyası
  - Fayl ölçüsü analizi
- 🎯 **6 Sıxışdırma Metodu**:

| Metod | Ən Yaxşı Olduğu Sahə | Sıxışdırma Dərəcəsi |
|-------|---------------------|-------------------|
| **Ağıllı Avtomatik** | Bütün sənədlər | 50-90% |
| **Şəkil Optimallaşdırılmış** | Şəkil ağırlıqlı PDF-lər | 60-80% |
| **Şrift Alt Dəsti** | Mətn sənədləri | 90%+ |
| **Balanslaşdırılmış** | Qarışıq məzmun | 40-70% |
| **Mətndən Yenidən Qurma** | Zədələnmiş PDF-lər | Dəyişir |
| **Maksimal + PDFtk Strip** | Maksimum sıxışdırma | 95%+ |

---

## 🎨 UI/UX Xüsusiyyətləri

### **Müasir İnterfeys**
- Rəng kodlu bölmələrlə təmiz, peşəkar dizayn
- Asan naviqasiya üçün tablı interfeys
- Real vaxt status yeniləmələri
- Marquee proqres çubuğu ilə animasiyalı "İşləyir..." dialoqu
- Peşəkar rəng sxemi (Mavilər, Yaşıllar, Bənövşəyilər, Narıncalar)

### **Fayl İdarəetmə**
- **Çoxlu daxiletmə metodları**:
  - Fayl baxışı
  - Qovluq baxışı (rekursiv PDF skan etmə)
  - Sürüşdür & burax
  - Clipboard yapışdır (Ctrl+V)
  - **TXT fayl siyahılarının idxal/ixracı**
  - Seçilmiş yolları kopyala (Ctrl+C)
  - Sil düymələri

### **Kontekst Menyu**
- Faylları aç
- Faylları/yolları yapışdır
- Seçilmiş yolları kopyala
- **TXT faylından siyahı idxal et**
- **TXT faylına siyahı ixrac et**
- Seçilmişləri sil
- Hamısını təmizlə

### **Önbaxış Sistemi**
- İlk səhifənin kiçik şəkli
- Ghostscript ilə render
- Ekrana uyğunlaşdır
- Status göstəriciləri

---

## 🛠️ Texniki Üstünlüklər

### **Performans**
- **Ultra-sürətli**: QPDF mühərriki böyük PDF-ləri millisaniyələr ərzində emal edir
- **Çoxşaxəli**: Emal zamanı reaktiv UI
- **Yaddaş səmərəli**: Faylları tamamilə yaddaşa yükləmədən emal edir
- **Toplu emal**: Yüzlərlə faylı eyni anda emal et

### **Etibarlılıq**
- **Ehtiyat mexanizmləri**: QPDF → PDFtk ehtiyat birləşdirmə
- **Xəta idarəetməsi**: Hərtərəfli try-catch blokları
- **Debug konsolu**: Problemlərin aradan qaldırılması üçün ətraflı qeyd
- **Validasiya**: Fayl mövcudluğu yoxlamaları, etibarlı PDF təsdiqi

### **Uyğunluq**
- **Çarpaz versiya dəstəyi**: PDF versiyaları 1.4 - 1.7
- **Daxiletmə formatları**: Standart PDF, şifrələnmiş PDF-lər
- **Çıxış formatları**: PDF, TXT (fayl siyahıları üçün)
- **Unicode dəstəyi**: Tam beynəlxalq simvol dəstəyi

### **Alət Deteksiyası**
- **Rekursiv skan**: LIBS qovluğunda alətləri avtomatik tapır
- **Çoxlu alət yolları**: Müxtəlif quraşdırma strukturlarını dəstəkləyir
- **Ehtiyat deteksiya**: PATH mühit dəyişənində axtarış

### **Təhlükəsizlik**
- **AES-256 şifrələmə**: Dövlət səviyyəli təhlükəsizlik
- **İcazə idarəetməsi**: İncə səviyyəli giriş nəzarəti
- **Parol qorunması**: İkiqat parol sistemi
- **Təhlükəsiz emal**: Müvəqqəti faylların təmizlənməsi

---

## 📊 İstifadəçi Təcrübəsi Üstünlükləri

### **İstifadə Asanlığı**
- **Bir klik əməliyyatları**: Birləşdir, böl, şifrələ, sıxışdır
- **İntuitiv interfeys**: Aydın etiketləmə və təşkilatlanma
- **Vizual geribildirim**: Status yeniləmələri və proqres göstəriciləri
- **Klaviatura qısayolları**: Ctrl+V, Ctrl+C, Delete

### **Məhsuldarlıq Artımı**
- **Toplu əməliyyatlar**: Birdən çox faylı eyni anda emal et
- **Qovluq skan etmə**: Qovluqdan bütün PDF-ləri avtomatik əlavə et
- **TXT idxal/ixrac**: Sessiyalar arası fayl siyahılarını paylaş
- **Avtomatik bölmə**: Bütün səhifələri bir kliklə böl

### **Əlçatanlıq**
- **Çoxdilli dəstək**: Dil faylı dəstəyi (.lang)
- **Klaviatura naviqasiyası**: Tam klaviatura dəstəyi
- **Aydın mesajlaşma**: Məlumatlandırıcı xəta və uğur mesajları
- **Alət məsləhətləri**: Kontekstual yardım

---

## 💡 İnnovativ Xüsusiyyətlər

### **Ağıllı Avtomatik Sıxışdırma**
Alət optimal sıxışdırma metodunu müəyyən etmək üçün PDF məzmununu analiz edir:
- **Yalnız mətn PDF-ləri**: Aqressiv şrift alt dəsti tətbiq edir
- **Şəkil ağırlıqlı PDF-lər**: Keyfiyyətə uyğunlaşdırılmış şəkil sıxışdırması tətbiq edir
- **Qarışıq məzmun**: Mətn və şəkil optimallaşdırmasını balanslaşdırır
- **Skan edilmiş sənədlər**: Xüsusi şəkil sıxışdırması tətbiq edir

### **İki Rejimli Bölmə**
- **İstifadəçi aralıqları**: Səhifə çıxarılması üzərində tam nəzarət
- **Avtomatik hissələrə bölmə**: Böyük PDF-ləri idarə olunan hissələrə böl

### **İki Parollu Şifrələmə**
- **İstifadəçi parolu**: Sənədə girişi idarə edir
- **Sahib parolu**: Sənəd icazələrini idarə edir
- **Çevik təhlükəsizlik**: Bir və ya hər iki paroldan istifadə edin

---

## 🚀 İstifadə Halları

### **Peşəkarlar Üçün**
- **Hüquq**: Eksponatları birləşdir, böyük sənədləri böl, həssas faylları şifrələ
- **Nəşriyyat**: Yüksək keyfiyyətli PDF-ləri sıxışdır, səhifələri çıxar
- **Təhsil**: Mühazirə materiallarını böl, tapşırıqları birləşdir
- **Dövlət**: Sənədlərin təhlükəsiz şifrələnməsi, PDF emalı

### **Şəxsi İstifadə Üçün**
- **Foto albomlar**: Böyük şəkil PDF-lərini sıxışdır
- **Elektron kitablar**: Kitabları fəsillərə böl
- **Skan edilmiş sənədlər**: Optimallaşdır və təşkil et
- **Təhlükəsiz paylaşım**: Şəxsi sənədləri parol ilə qoru

---

## 📈 Performans Göstəriciləri

| Əməliyyat | Tipik Sürət | Texnologiya |
|-----------|-------------|-------------|
| 100 PDF-i birləşdir | < 1 saniyə | QPDF |
| 500 səhifəlik PDF-i böl | 2-3 saniyə | QPDF |
| AES-256 Şifrələmə | 5-10 saniyə | QPDF |
| Sıxışdırma (Şəkil) | 15-30 saniyə | Ghostscript |
| Sıxışdırma (Mətn) | 5-10 saniyə | Ghostscript |
| Önbaxış yaratma | < 1 saniyə | Ghostscript |

---

## 🎯 Rəqabət Üstünlükləri

### **Onlayn Xidmətlərə Qarşı**
- ✅ Fayl ölçüsü məhdudiyyəti yoxdur
- ✅ İnternet tələb olunmur
- ✅ Limitsiz emal
- ✅ Məxfilik narahatlığı yoxdur
- ✅ Toplu emal
- ✅ Çoxlu çıxış formatları
- ✅ **Daha yaxşı sıxışdırma keyfiyyəti**

### **Masaüstü Alternativlərə Qarşı**
- ✅ Pulsuz və açıq mənbəli
- ✅ Yüngül (ağır asılılıqlar yoxdur)
- ✅ Quraşdırma tələb olunmur
- ✅ Ultra-sürətli emal
- ✅ Müəssisə səviyyəli şifrələmə
- ✅ **Ödənişli alətlərdən daha səmərəli**

---

## 🔮 Gələcək Potensial

### **Potensial Təkmilləşdirmələr**
- **Toplu emal**: Ardıcıl olaraq çoxlu əməliyyatları emal et
- **OCR inteqrasiyası**: Optik simvol tanıma əlavə et
- **Bulud inteqrasiyası**: Birbaşa bulud yaddaş dəstəyi
- **Su nişanı**: Mətn/şəkil su nişanları əlavə et
- **Rəqəmsal imzalar**: PDF sənədlərini imzala
- **Metadata redaktəsi**: PDF xassələrini dəyiş
- **Forma çıxarılması**: Forma sahəsi məlumatlarını çıxar
- **Səhifə fırlanması**: Toplu səhifə fırlanması

---

## 📋 Xülasə

**Kerim's PDF Tools - QPDF ULTRA FAST V4** aşağıdakıları birləşdirən **peşəkar səviyyəli PDF manipulyasiya dəstidir**:

- **Müəssisə performansı** QPDF-in ultra-sürətli mühərriki ilə
- **Hərbi səviyyəli təhlükəsizlik** AES-256 şifrələmə ilə
- **Peşəkar xüsusiyyətlər** ağıllı sıxışdırma və iki rejimli bölmə daxil olmaqla
- **İstifadəçi dostu interfeys** müasir UI və intuitiv idarəetmə ilə
- **Sıfır xərc** - tamamilə pulsuz və açıq mənbəli
- **Məxfilik yönümlü** - tamamilə oflayn emal edir
- **İstənilən onlayn xidmətdən daha yaxşı nəticələr**

**Ən uyğundur**: Hüquq peşəkarları, nəşriyyatçılar, təhsil işçiləri, dövlət qurumları və bulud məxfilik narahatlığı olmadan sürətli, təhlükəsiz PDF emalına ehtiyacı olan hər kəs üçün.

---

## ⭐ Əsas Satış Nöqtələri

1. **ULTRA SÜRƏTLİ**: Dəqiqələr yox, millisaniyələr ərzində birləşdirir
2. **100% PULSUZ**: Gizli xərclər yoxdur, abunəlik yoxdur
3. **OFFLAYIN**: Həssas sənədləri təhlükəsiz emal et
4. **AES-256**: Hərbi səviyyəli şifrələmə
5. **AĞILLI SIXIŞDIRMA**: Süni intellektə bənzər məzmun analizi
6. **QURAŞDIRMA TƏLƏB OLUNMUR**: Portativ icra olunan fayl
7. **TOPLU EMAL**: Yüzlərlə faylı idarə et
8. **PEŞƏKAR UI**: Təmiz, müasir interfeys
9. **ONLAYN XİDMƏTLƏRDƏN DAHA YAXŞI**: Üstün sıxışdırma keyfiyyəti
10. **WINDOWS 10/11**: Tam test edilib və optimallaşdırılıb

---

## 📦 Yükləmə

### Son Buraxılış
[![Download](https://img.shields.io/badge/Yüklə-Son_Buraxılış-blue.svg)](https://github.com/yourusername/kerim-pdf-tools/releases/latest)

### Quraşdırma Addımları
1. Arxivi [Releases](https://github.com/yourusername/kerim-pdf-tools/releases) bölməsindən yükləyin
2. İstənilən qovluğa açın (tövsiyə: İş masası)
3. `Start.bat` faylını işə salın
4. GUI açılacaq - istifadəyə hazırdır!

---

## 📄 Lisenziya

Bu layihə MIT Lisenziyası altında lisenziyalaşdırılıb - ətraflı məlumat üçün [LICENSE](LICENSE) faylına baxın.

---

## 🙏 Təşəkkürlər

### İstifadə Olunan Rəsmi İkili Fayllar
- **QPDF** - Əsas PDF emal mühərriki (`LIBS\qpdf\`)
- **Ghostscript** - PDF sıxışdırma və önbaxış yaratma (`LIBS\gs\`)
- **PDFtk** - Ehtiyat PDF əməliyyatları (`LIBS\PDFtk Server\`)

### GUI Texnologiyası
- **PowerShell** - GUI və məntiq (`LIBS\guipdf.ps1`)

### Təşəkkürlər
- **Tural** - Yaradıcı və baş inkişaf etdirici
- **Kerim** - İlham və həsr

---

**❤️ ilə PDF cəmiyyəti üçün hazırlanıb**

*"PDF-ləri düşüncə sürətində emal edir"* ⚡

---

*Windows 10, Windows 11-də test edilib*

**Tam Dəyişikliklər Siyahısı**: https://github.com/Kerim4ik4/PDF-Compress-and-Merge/compare/v3...v4

*Tested on Windows 10, Windows 11*

**Full Changelog**: https://github.com/Kerim4ik4/PDF-Compress-and-Merge/compare/v3...v4

**Full Changelog**: https://github.com/Kerim4ik4/PDF-Compress-and-Merge/compare/v3...v4
