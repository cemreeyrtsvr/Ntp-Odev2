<!-- Başlık ve Badgeler -->
# 🔐 EduKey — Eğitim Amaçlı Tuş Kaydedici (Keylogger)  
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)  
[![Build](https://img.shields.io/badge/build-publish%20locally-green.svg)](#) 
[![Platform](https://img.shields.io/badge/platform-windows-orange.svg)](#)  
[![Consent Required](https://img.shields.io/badge/Consent-Required-yellow.svg)](#)  
[![Safe Use Recommended](https://img.shields.io/badge/Safe%20Use-VM%20only-red.svg)](#)

---

> **Kısa açıklama:**  
> `EduKey` eğitim amaçlı geliştirilmiş, yalnızca **açık ve yazılı rıza ile** kullanılması gereken bir tuş kaydedici deney/prototipidir. Bu proje **siber güvenlik eğitimi** için hazırlanmıştır ve kötüye kullanım amaçlı **hiçbir** davranışı desteklemez.

---

## 📌 Önemli Uyarı — Zorunlu Okuyun
- Bu yazılım **yalnızca** eğitim amaçlı kullanılmalıdır.  
- Uygulamayı çalıştırmadan **önce** tüm katılımcılardan **açık, yazılı rıza** almanız zorunludur.  
- Uygulamayı yalnızca **izole edilmiş VM’ler** veya öğretim görevlisinin belirlediği kontrollü ortamlarda çalıştırın.  
- Bu projeyi kötüye kullanan kişilerden doğacak etik veya yasal sorumluluk **kullanıcıya** aittir.

---

## 🧾 İçindekiler
1. [Proje Amacı](#proje-amacı)  
2. [Gereksinimler](#gereksinimler)  
3. [Derleme & Çalıştırma (Öğrenci / Ödev akışı)](#derleme--çalıştırma-öğrenci--ödev-akışı)  
4. [Güvenli Test Protokolü (Zorunlu)](#güvenli-test-protokolü-zorunlu)  
5. [Veri, Gizlilik ve Rıza](#veri-gizlilik-ve-rıza)  
6. [Sık Karşılaşılan Sorunlar ve Çözümleri](#sık-karşılaşılan-sorunlar-ve-çözümleri)  
7. [Lisans & İletişim](#lisans--iletişim)

---

## 🎯 Proje Amacı
Bu proje, öğrencilerin tuş yakalama yöntemlerini, log yönetimini ve güvenli test uygulamalarını öğrenmesi amacıyla hazırlanmıştır. Amaçlar:
- Klavye olaylarını yakalamak ve güvenli biçimde işlemeyi göstermek.  
- Log yönetimi, şifreleme ve gizli veri saklama risklerini değerlendirmek.  
- E-posta raporlama vs. gibi ağ tabanlı süreçleri izole bir ortamda test etmek.

---

## ⚙️ Gereksinimler
- Windows 10 / 11 (test için VM önerilir)  
- Visual Studio 2019/2022 veya .NET SDK (projeye göre)  
- .NET Framework veya .NET (projeye göre) — proje kökünde `TargetFramework`’e bakın  
- İnternet bağlantısı (sadece eğer e-posta raporlama testi yapılacaksa)  

> **Güvenlik:** Gerçek ağ üzerinde e-posta testleri yapmadan önce ortamı izole edin.

---

## 🛠️ Derleme & Çalıştırma (Öğrenci / Ödev akışı)
> Aşağıdaki akış, **kaynak kod paylaşımı** → **öğrenci kendi VM’inde derleme** mantığıyla hazırlanmıştır (önerilen ve güvenli yol).

### 1) Kaynak Kodunu Al
- Repo’yu klonlayın veya zip’i açın:
```bash
git clone https://github.com/ORNEK/KULLANICI/REPO.git
