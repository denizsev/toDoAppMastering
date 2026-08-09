# Görevler

Sözdizimsiz, tamamen dokunmatik, tek dosyalık bir günlük yapılacaklar (to-do) uygulaması.
Kurulum yok, derleme adımı yok, sunucu yok, hesap yok. Verin sadece kendi tarayıcında kalır.

**[Canlı demo →](#)** *(GitHub Pages linkini yayınladıktan sonra buraya ekle)*

---

## Neden

Çoğu to-do uygulaması ya "yarın 15:00 #okul p1" gibi bir sözdizimi öğrenmeni ister, ya da
masaüstü alışkanlıklarını (klavye kısayolu, sidebar, hover menü) telefona olduğu gibi taşır.
Bu uygulama tam tersini yapıyor: her şey dokunma. Yazman gereken tek şey görevin başlığı —
tarih, saat, liste ve öncelik hepsi çip'lere dokunarak seçiliyor.

## Özellikler

- **Sıfır sözdizimi** — FAB'a dokun, başlığı yaz, çip'lerle tarih/saat/liste/öncelik seç
- **Kaydırma jestleri** — sağa kaydır tamamla, sola kaydır ertele/sil (uzun-bas ile de erişilebilir)
- **Günü Planla** — gecikmiş görevleri tek tek, büyük dokunma butonlarıyla triyaj et
- **Listeler** — Gelen Kutusu + kendi oluşturduğun listeler
- **Tekrarlayan görevler** — her gün / hafta içi / her hafta / her ay
- **Koyu mod**, ilerleme halkası, geri alınabilir silme (5 saniyelik "Geri al")
- **Çevrimdışı çalışır** — veri tarayıcının `localStorage`'ında tutulur, hiçbir yere gönderilmez
- **Ana ekrana eklenebilir** — telefonda "Ana Ekrana Ekle" ile gerçek bir uygulama gibi açılır

## Kullanmaya başla

1. [Canlı demo linkini](#) telefonunda aç
2. Paylaş menüsünden **"Ana Ekrana Ekle"**'ye dokun
3. Artık ana ekranında bir ikon — dokun, kullan

Kendi cihazına indirip de kullanabilirsin: `index.html` dosyasını indir, çift tıkla, açılsın.

## Teknik

Vanilla JavaScript, HTML, CSS — hiçbir framework veya bağımlılık yok. Tek dosya, ~50KB.
Veri kalıcılığı `localStorage` ile sağlanıyor; tarih hesaplamaları saat dilimi/DST hatalarından
kaçınmak için takvim günü (`YYYY-MM-DD`) bazlı yapılıyor. Sürükleme/sıralama için
[fractional indexing](https://www.figma.com/blog/realtime-editing-of-ordered-sequences/) kullanılıyor.

## Bu projeyi kendi GitHub Pages'inde yayınlama

Bu klasördeki dosyaları yeni bir GitHub deposuna yükleyip **Settings → Pages** üzerinden
yayınlayabilirsin — kod yazmana ya da bir şey kurmana gerek yok. Adımlar için depo
açıklamasına veya paylaşılan sohbete bak.

## Lisans

MIT — [LICENSE](LICENSE) dosyasına bak. Kopyala, değiştir, kendi ihtiyacına uyarla.
