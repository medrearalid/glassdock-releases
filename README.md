<div align="center">

<img src="docs/glassdock-icon.png" width="88" alt="glassdock simgesi">

# glassdock

Windows 11 için cam bir dock. Görev çubuğunun yerine geçer, Başlat menüsünü yeniler, masaüstüne hareket katar.

Kendi duvar kâğıdı motoruyla gelir. Videoyu ekranına göre bir kez hazırlar, ekran kartında oynatır ve dock'tan ayrı çalıştırır. Bir pencere üstünü kapatınca durur, oyun açılınca belleği bırakır.

<a href="https://github.com/medrearalid/glassdock-releases/releases/latest"><img src="https://img.shields.io/github/v/release/medrearalid/glassdock-releases?style=for-the-badge&label=GLASSDOCK%27U%20%C4%B0ND%C4%B0R&color=0A84FF&logo=windows11&logoColor=white" alt="glassdock'u indir" height="36"></a>

<sub>[Neler yeni](https://github.com/medrearalid/glassdock-releases/releases/latest) · [Kurulum](#kurulum) · [Gizlilik](#gizlilik) · [SSS](#sss)</sub>

<br>

<img src="docs/hero-black.webp" alt="glassdock, masaüstünün altında" width="100%">

</div>

<br>

## Başlat ve arama

Win tuşuna bas ve yazmaya başla. Uygulamalar, Windows'un bütün ayarları ve dosyaların tek listede gelir, en iyi eşleşme en üstte durur. Arama internete çıkmaz, reklam ya da web sonucu göstermez.

Yazım hatalarını ve baş harfleri anlar. "vsc" yazınca Visual Studio Code bulunur. Ayarlar ana sayfaya değil doğrudan aradığın ayara açılır. Bu Bilgisayar ve Geri Dönüşüm Kutusu da burada, masaüstün boş kalabilir.

<p align="center">
  <img src="docs/start.webp" width="49%" alt="Başlat paneli ve arama">
  <img src="docs/search-results.webp" width="49%" alt="Kategorilere ayrılmış arama sonuçları">
</p>

Windows'un kendi Başlat menüsünü özlersen Ayarlar › Başlat'tan tek dokunuşla geri getirebilirsin.

## Canlı duvar kâğıdı

Bir videoyu ya da hareketli sahneyi duvar kâğıdı yap. Eklediğin video ekranına göre küçültülür, böylece hem az yer kaplar hem de ekran kartını yormaz. Pencereler üstünü kapatınca, oyunda ve pilde kendini uyutur. Dock'un camı bu hareketi arkasından yansıtır.

<p align="center"><img src="docs/live-wallpaper-red.webp" width="100%" alt="Hareketli duvar kâğıdı ve önünde dock"></p>

Henüz beta. Ayarlar › Duvar kağıdı sekmesinden açılıyor.

## Her duvar kâğıdında yerinde

Cam, arkasındaki renkleri alır. Kenarlarında ışık mercek gibi kırılır.

<p align="center">
  <img src="docs/dock-on-purple.png" alt="Mor duvar kâğıdı üstünde dock" width="90%"><br>
  <img src="docs/dock-on-obsidian.png" alt="Koyu duvar kâğıdı üstünde dock" width="90%"><br>
  <img src="docs/dock-on-opal.png" alt="Renkli duvar kâğıdı üstünde dock" width="90%"><br>
  <img src="docs/dock-on-pearl.png" alt="Açık duvar kâğıdı üstünde dock" width="90%"><br>
  <img src="docs/dock-on-red.png" alt="Kırmızı duvar kâğıdı üstünde dock" width="90%">
</p>

## Müzik

Çalan şarkı dock'ta görünür. Üstüne tıklayınca açılan panelde sıradakiler, çalma listeleri ve şarkıyla birlikte akan sözler var. Spotify, YouTube Music ve tarayıcıda çalanlarla çalışır.

<p align="center"><img src="docs/music-panel.webp" width="34%" alt="Müzik paneli"></p>

## Gerisi

- **Uygulamalar ve klasörler.** Görev çubuğu sabitlerin kendiliğinden gelir. Açık pencerelerin canlı önizlemesi, sürükle bırak klasörler ve okunmamış mesaj rozetleri var.
- **Widget'lar.** Saat ve hava durumu, takvim, sistem kartı, yapay zekâ kullanım limitleri ve tepsi simgeleri. Her birinin üç boyutu var, üst üste de yığılabilir.
- **Bildirimler.** Windows bildirimleri dock'un kendi kartlarıyla gelir ve tepsideki zilde toplanır. Türkçe yazılan hatırlatıcılar da burada.
- **Akıllı gizlenme.** Bir pencere altına gelince kenara çekilir, imleç kenara gelince döner. Oyunda tamamen kaybolur.
- **Güncellemeler.** Günde bir kez bakar, yeni sürümü doğrulayıp sessizce kurar.

## Kurulum

1. [Son sürümün sayfasından](https://github.com/medrearalid/glassdock-releases/releases/latest) `glassdock-x.y.z-setup.exe` dosyasını indir.
2. Çalıştır. Yönetici izni istemez.
3. Dock ekranın altında açılır. Ayarlar için dock'a sağ tıkla.

Sonrasında glassdock kendini güncel tutar.

<details>
<summary><b>"Windows bilgisayarınızı korudu" uyarısı çıkarsa</b></summary>

<br>

Kurulum dosyası henüz imzalı olmadığı için SmartScreen uyarabilir. Ek bilgi › Yine de çalıştır ile devam edebilirsin. İstersen dosyayı sürümün yanındaki `.sha256` ile karşılaştır.

```powershell
Get-FileHash .\glassdock-x.y.z-setup.exe -Algorithm SHA256
```

</details>

Windows 11, 64 bit gerekir. Kurulum dosyası yaklaşık 5 MB.

## Gizlilik

glassdock hesap istemez, telemetri göndermez. Arama ve Başlat paneli tamamen bilgisayarında çalışır. İnternete yalnızca açtığın özellikler için çıkar.

| Özellik | Bağlandığı yer |
|:--|:--|
| Hava durumu | Open-Meteo |
| Takvim | Eklediğin iCal adresleri |
| Şarkı sözleri | LRCLIB, lyrics.ovh, NetEase |
| Spotify | Bağlarsan yalnızca Spotify |
| Yapay zekâ kullanımı | Bilgisayarındaki Claude, ChatGPT ya da Gemini girişinle ilgili sağlayıcı |
| Güncelleme | GitHub |

Ayarların `%APPDATA%\glassdock` klasöründe durur.

## Duvar kâğıtları

glassdock için hazırladığımız üç duvar kâğıdı, hepsi 1672×941. Görsele tıkla ve açılan sayfadan indir. Hepsini birden almak için Code › Download ZIP.

| | | |
|:-:|:-:|:-:|
| [<img src="wallpapers/previews/obsidian-void-grain.jpg" alt="Obsidian Void Grain">](wallpapers/obsidian-void-grain.png)<br><sub><b>Obsidian Void</b></sub> | [<img src="wallpapers/previews/pearl-void-grain.jpg" alt="Pearl Void Grain">](wallpapers/pearl-void-grain.png)<br><sub><b>Pearl Void</b></sub> | [<img src="wallpapers/previews/cosmic-opal.jpg" alt="Cosmic Opal">](wallpapers/cosmic-opal.png)<br><sub><b>Cosmic Opal</b></sub> |

## SSS

<details>
<summary><b>Windows görev çubuğuna ne oluyor?</b></summary>
<br>
glassdock açıkken görev çubuğu gizlenir. Dock kapanınca ya da kaldırılınca olduğu gibi geri gelir.
</details>

<details>
<summary><b>Oyunlarda performansı etkiler mi?</b></summary>
<br>
Tam ekran oyunda dock ve duvar kâğıdı durur, güncellemeler oyun bitene kadar bekler. Eski bilgisayarlarda performans modu animasyonları kapatır.
</details>

<details>
<summary><b>Win tuşu bazen Windows Başlat'ı açıyor</b></summary>
<br>
Oyun sırasında ve yönetici olarak çalışan bir pencere öndeyken Windows kendi menüsünü açar. Bu Windows'un bir sınırı.
</details>

<details>
<summary><b>Nasıl kaldırırım?</b></summary>
<br>
Ayarlar › Uygulamalar › Yüklü uygulamalar › glassdock › Kaldır. Ayarları da silmek istersen <code>%APPDATA%\glassdock</code> klasörünü sil.
</details>

## Geri bildirim

Hata ya da öneri için bir [issue aç](https://github.com/medrearalid/glassdock-releases/issues). Ekran görüntüsü eklersen daha çabuk çözeriz.

## Lisans

© 2026 Guney. Tüm hakları saklıdır. glassdock ücretsizdir ama açık kaynak değildir. Kendi bilgisayarında kullanabilir, duvar kâğıtlarını arka plan yapabilirsin. Yeniden dağıtmak, değiştirmek ya da satmak yazılı izne bağlı. Ayrıntılar [LICENSE](LICENSE) dosyasında.
