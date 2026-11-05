<div align="center">

<img src="docs/icon.png" width="88" alt="glassdock simgesi">

# glassdock

**Windows 11 için cam bir dock.**<br>
Görev çubuğunun yerini alır: uygulamalar, klasörler, widget'lar, takvim ve bildirimler tek bir yerde.

[![Son sürüm](https://img.shields.io/github/v/release/medrearalid/glassdock-releases?style=flat-square&label=s%C3%BCr%C3%BCm&color=0A84FF)](https://github.com/medrearalid/glassdock-releases/releases/latest)
[![İndirme](https://img.shields.io/github/downloads/medrearalid/glassdock-releases/total?style=flat-square&label=indirme&color=30353d)](https://github.com/medrearalid/glassdock-releases/releases)
[![Platform](https://img.shields.io/badge/Windows%2011-x64-30353d?style=flat-square)](#gereksinimler)
[![Lisans](https://img.shields.io/badge/lisans-%C3%BCcretsiz-30353d?style=flat-square)](#lisans)

<a href="https://github.com/medrearalid/glassdock-releases/releases/latest"><img src="https://img.shields.io/github/v/release/medrearalid/glassdock-releases?style=for-the-badge&label=GLASSDOCK%27U%20%C4%B0ND%C4%B0R&color=0A84FF&logo=windows11&logoColor=white" alt="glassdock'u indir" height="36"></a>

<sub>[Neler yeni](https://github.com/medrearalid/glassdock-releases/releases/latest) · [Kurulum](#kurulum) · [Özellikler](#özellikler) · [Gizlilik](#gizlilik) · [SSS](#sss)</sub>

<br>

<img src="docs/hero.webp" alt="glassdock, masaüstünün altında" width="100%">

</div>

<br>

## Her duvar kâğıdında yerinde

Cam, arkasındaki duvar kâğıdından renk alır. Liquid modda kenarlarında mercek gibi kırılır; buzlu modda sistemin bulanık camını kullanır.

<p align="center">
  <img src="docs/dock-light.png" alt="Açık duvar kâğıdı üstünde dock" width="80%"><br>
  <img src="docs/dock-dark.png" alt="Koyu duvar kâğıdı üstünde dock" width="80%"><br>
  <img src="docs/dock-warm.png" alt="Sıcak tonlu duvar kâğıdı üstünde dock" width="80%">
</p>

<p align="center">
  <img src="docs/desktop-dark.webp" width="49%" alt="Koyu masaüstünde glassdock">
  <img src="docs/desktop-light.webp" width="49%" alt="Açık masaüstünde glassdock">
</p>

## Özellikler

<table>
<tr>
<td width="50%" valign="top">

### Dock
Liquid ya da buzlu cam; cam, gece ve açık stiller. Altta, üstte ya da yanlarda; ortada ya da kenardan kenara. Kenarından çekerek başka kenara taşınır, ekrana sığmayacak kadar büyümez.

</td>
<td width="50%" valign="top">

### Uygulamalar ve klasörler
Görev çubuğu sabitlemelerin kendiliğinden gelir. Açık pencereler gruplanır; üstüne gelince canlı önizleme ve pencere seçici açılır. Sürükle-bırak klasörler, çalışan uygulamalarda okunmamış mesaj rozetleri.

</td>
</tr>
<tr>
<td valign="top">

### Widget'lar
Saat ve canlı hava durumu, kapak resimli medya kontrolü, takvim, sistem kartı, tepsi simgeleri. Her widget'ın küçük, orta ve büyük boyutu var; widget'lar üst üste yığılabilir.

</td>
<td valign="top">

### Takvim ve bildirimler
Türkçe hızlı eklemeli planlayıcı ("yarın 14:30 diş hekimi 10dk önce"), sesli hatırlatıcılar ve "Sessiz" anahtarlı bildirim merkezi. Google, Outlook ya da iCloud takvimi iCal adresiyle bağlanır.

</td>
</tr>
<tr>
<td valign="top">

### Akıllı gizlenme
Altına etkileşimli bir şey gelince kenara çekilir, imleç kenara gelince açılır. Tam ekranda kompakt hâle geçer, oyunlarda tamamen gizlenir.

</td>
<td valign="top">

### Yapay zekâ kullanımı
Claude, ChatGPT ve Gemini limitleri tek kartta. Üstünde durunca tüm limitler ve yenilenme saatleri açılır; limit azalınca bildirim gelir.

</td>
</tr>
<tr>
<td valign="top">

### Hareket
GPU'da çizilen genie küçültme, uygulama açılış ve pencere geçiş animasyonları. Hepsi *performans modu* ile tek anahtardan kapanır.

</td>
<td valign="top">

### Güncellemeler
Günde bir kez denetlenir. Yeni sürüm SHA-256 ile doğrulanıp sessizce kurulur; dock'un kendi kartı yenilikleri özetler, notların tamamı ayarlarda.

</td>
</tr>
</table>

## Kurulum

1. [Son sürümün sayfasından](https://github.com/medrearalid/glassdock-releases/releases/latest) `glassdock-x.y.z-setup.exe` dosyasını indir.
2. Çalıştır. Yönetici izni gerekmez; kendi kullanıcı klasörüne kurulur.
3. Dock ekranın altında açılır. Ayarlar için dock'a sağ tıkla → **Ayarlar…**

Kurulduktan sonra glassdock kendini güncel tutar; bir daha indirmen gerekmez.

<details>
<summary><b>"Windows bilgisayarınızı korudu" uyarısı çıkarsa</b></summary>

<br>

Kurulum dosyası henüz kod imzalı değil, bu yüzden SmartScreen uyarı verebilir. **Ek bilgi → Yine de çalıştır** ile devam edebilirsin. İstersen indirdiğin dosyayı, sürümün yanındaki `.sha256` dosyasıyla karşılaştır:

```powershell
Get-FileHash .\glassdock-x.y.z-setup.exe -Algorithm SHA256
```

</details>

### Gereksinimler

| | |
|:--|:--|
| **Sistem** | Windows 11, 64 bit (Windows 10'da denenmedi) |
| **Yetki** | Yönetici izni gerekmez |
| **Bileşenler** | WebView2, yalnızca ayarlar penceresi için (Windows 11'de yüklü gelir) |
| **Boyut** | Kurulum dosyası yaklaşık 4 MB |

## Gizlilik

glassdock hesap istemez, kullanım verisi ya da telemetri göndermez. Yalnızca açtığın özellikler için şu adreslere bağlanır:

| Özellik | Bağlandığı yer |
|:--|:--|
| Hava durumu | Open-Meteo |
| Takvim | Yalnızca senin eklediğin iCal adresleri |
| Güncelleme | GitHub (bu depo) |
| Yapay zekâ kullanımı | Bilgisayarındaki Claude Code, Codex ya da Gemini CLI girişiyle, ilgili sağlayıcının kullanım adresi |

Ayarların ve hatırlatıcıların bilgisayarında, `%APPDATA%\glassdock` klasöründe durur.

## Duvar kâğıtları

Ekran görüntülerindeki duvar kâğıtları burada; hepsi 1672×941. Görsele tıkla, açılan sayfada **Download raw file** (⬇) ile indir. Hepsi için **Code → Download ZIP**. *Grain* sürümlerinde ince bir film greni var.

| | |
|:-:|:-:|
| [<img src="wallpapers/previews/cosmic-opal.jpg" alt="Cosmic Opal">](wallpapers/cosmic-opal.png)<br><sub><b>Cosmic Opal</b></sub> | [<img src="wallpapers/previews/chromatic-void.jpg" alt="Chromatic Void">](wallpapers/chromatic-void.png)<br><sub><b>Chromatic Void</b></sub> |
| [<img src="wallpapers/previews/obsidian-void.jpg" alt="Obsidian Void">](wallpapers/obsidian-void.png)<br><sub><b>Obsidian Void</b></sub> | [<img src="wallpapers/previews/obsidian-void-grain.jpg" alt="Obsidian Void Grain">](wallpapers/obsidian-void-grain.png)<br><sub><b>Obsidian Void · Grain</b></sub> |
| [<img src="wallpapers/previews/pearl-void.jpg" alt="Pearl Void">](wallpapers/pearl-void.png)<br><sub><b>Pearl Void</b></sub> | [<img src="wallpapers/previews/pearl-void-grain.jpg" alt="Pearl Void Grain">](wallpapers/pearl-void-grain.png)<br><sub><b>Pearl Void · Grain</b></sub> |
| [<img src="wallpapers/previews/chromatic-void-grain.jpg" alt="Chromatic Void Grain">](wallpapers/chromatic-void-grain.png)<br><sub><b>Chromatic Void · Grain</b></sub> | |

## SSS

<details>
<summary><b>Windows görev çubuğuna ne oluyor?</b></summary>
<br>
glassdock açıkken görev çubuğunu gizler ve tepsi simgelerini kendisi gösterir. Dock kapanınca ya da kaldırılınca görev çubuğu olduğu gibi geri gelir.
</details>

<details>
<summary><b>Oyunlarda performansı etkiler mi?</b></summary>
<br>
Tam ekran oyunlarda dock tamamen gizlenir ve güncellemeler oyun bitene kadar bekler. Eski bilgisayarlarda <i>performans modu</i> animasyonları kapatıp buzlu cama geçer.
</details>

<details>
<summary><b>Nasıl kaldırırım?</b></summary>
<br>
<b>Ayarlar → Uygulamalar → Yüklü uygulamalar → glassdock → Kaldır.</b> Ayarların <code>%APPDATA%\glassdock</code> klasöründe kalır; tamamen temizlemek için o klasörü de silebilirsin.
</details>

<details>
<summary><b>Otomatik güncellemeyi kapatabilir miyim?</b></summary>
<br>
Evet: <b>Ayarlar → Genel → Güncelleme</b>. Elle denetlemek için dock'a sağ tıkla → <b>Güncellemeleri denetle</b>.
</details>

## Geri bildirim

Hata ya da öneri için bir [issue aç](https://github.com/medrearalid/glassdock-releases/issues). Ekran görüntüsü ve Windows sürümünü eklersen hata daha çabuk çözülür.

## Lisans

glassdock ücretsiz kullanılabilir ama açık kaynak değil. Bu depoda yalnızca kurulum dosyaları ve duvar kâğıtları var. Kişisel kullanım için indirip kurabilirsin; kurulum dosyalarını başka yerlerde yeniden dağıtmak ya da değiştirerek yayınlamak serbest değil.

<br>

<p align="center"><sub>glassdock · Windows 11 için cam dock</sub></p>
