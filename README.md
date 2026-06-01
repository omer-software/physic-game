# ⚗️ Usta Karim'in Sırrı — Kaldırma Kuvveti Etkileşimli Oyunu

**Fizik 9. Sınıf · Kaldırma Kuvveti · Tarayıcı Tabanlı Pixel Art Oyunu**

---

## Proje Hakkında

Bu proje, 9. sınıf fizik dersi için tasarlanmış etkileşimli bir tarayıcı oyunudur. Öğrenciler, Antik İskenderiye'de gemi yükü hesapları yapan **Usta Karim**'e yardım ederek kaldırma kuvvetinin hangi değişkenlere bağlı olduğunu deneyle keşfeder.

Oyun tamamen saf HTML + CSS + JavaScript ile yazılmıştır. Herhangi bir kurulum, sunucu veya internet bağlantısı gerektirmez. Dosyayı tarayıcıda açmak yeterlidir.

---

## Dosyalar

```
kaldirma.html   ← Oyunun tüm kodu (tek dosya, bağımsız çalışır)
README.md       ← Bu dosya
```

---

## Nasıl Açılır

`kaldirma.html` dosyasını herhangi bir modern tarayıcıda açın (Chrome, Firefox, Edge, Safari).

Kurulum gerekmez. İnternet bağlantısı sadece Google Fonts için kullanılır; fontlar yüklenmese de oyun çalışmaya devam eder.

---

## Oyun İçeriği

Oyun dört bölümden oluşur ve her bölüm bir fizik değişkenini ele alır.

### Bölüm 1 — Hacim Deneyi
Cismin hacmi kaydırıcıyla 1–12 dm³ arasında değiştirilerek kaldırma kuvvetinin (Fk) hacimle doğru orantılı arttığı gözlemlenir.

### Bölüm 2 — Yoğunluk Deneyi
Tahta, parafin, beton ve demir arasından cisim seçilir. Aynı hacimde tüm cisimlerin aynı kaldırma kuvveti aldığı, ancak cisim yoğunluğunun batıp batmamayı belirlediği keşfedilir.

### Bölüm 3 — Sıvı Deneyi
Tatlı su, deniz suyu, zeytinyağı ve cıva arasından sıvı seçilir. Sıvı yoğunluğu arttıkça kaldırma kuvvetinin nasıl değiştiği gözlemlenir.

### Bölüm 4 — Final Sınavı
Üç çoktan seçmeli soru ile öğrenilen kavramlar pekiştirilir ve Usta Karim'den diploma alınır.

---

## Öğrenme Kazanımları

Oyunun sonunda öğrenci şunları kavramış olur:

- Kaldırma kuvvetinin formülü: **Fk = ρ_sıvı · V · g**
- Kaldırma kuvveti sıvının yoğunluğuna ve cismin suya batan hacmine bağlıdır
- Cisim yoğunluğu kaldırma kuvvetini değil, batıp batmamayı belirler
- Yüzme koşulu: **Fk ≥ W**, yani **ρ_cisim ≤ ρ_sıvı**

---

## Teknik Detaylar

| Özellik | Değer |
|---|---|
| Platform | HTML5 (tek dosya) |
| Bağımlılık | Yok (sadece Google Fonts, opsiyonel) |
| Grafik | Canvas API — Pixel art tarzı |
| Tarayıcı desteği | Chrome 80+, Firefox 75+, Edge 80+, Safari 14+ |
| Mobil uyumlu | Evet (responsive layout) |

---

## Fizik Parametreleri

Oyun içinde kullanılan değerler:

| Parametre | Değer |
|---|---|
| Yerçekimi (g) | 9.8 m/s² |
| Tatlı su yoğunluğu | 1000 kg/m³ |
| Deniz suyu yoğunluğu | 1025 kg/m³ |
| Zeytinyağı yoğunluğu | 900 kg/m³ |
| Cıva yoğunluğu | 13600 kg/m³ |
| Tahta yoğunluğu | 600 kg/m³ |
| Parafin yoğunluğu | 870 kg/m³ |
| Beton yoğunluğu | 1800 kg/m³ |
| Demir yoğunluğu | 7800 kg/m³ |

---

## Geliştirici Notları

Oyunun kaynak kodu `kaldirma.html` içinde tek blok halindedir. Değiştirmek isteyenler için temel yapı:

- **Veri dizileri** (`OBJS`, `LIQS`, `STORIES`, `PHASE_Q`, `FINAL_Q`) — dosyanın üst kısmında, kolayca düzenlenebilir
- **Fizik hesapları** — `getFk()`, `getW()`, `floats()` fonksiyonları
- **Canvas çizimi** — `draw()` ve alt fonksiyonları
- **Kontrol paneli** — `buildCtrl()` fonksiyonu, DOM elemanlarını dinamik olarak oluşturur

---

## Hazırlayan

Bu oyun bir fizik ödevi kapsamında hazırlanmıştır.
