# Ulutürk Avukatlık Ortaklığı — örnek çalışma

Bu depo, bir avukatlık ortaklığı için hazırlanmış **örnek site çalışmasıdır**.
Yayındaki kuruma ait resmî bir site değildir ve içindeki metinler temsilîdir.

## İçerik

| Dosya | Açıklama |
|---|---|
| `index.html` | Sitenin tamamı — tek dosya, harici bağımlılık yok |
| `404.html` | Hatalı adreslerde gösterilen sayfa |
| `robots.txt` | Tarayıcı erişim kuralları |

## Teknik notlar

- Tek HTML dosyası. Çerçeve, derleme adımı ve paket bağımlılığı yok.
- Dışarıdan yüklenen tek kaynak Google Fonts. Görsel dosyası kullanılmıyor;
  arka plandaki grafik SVG olarak kodun içinde çiziliyor.
- Türkçe / İngilizce içerik geçişi sayfa içinde çalışır.
- `prefers-reduced-motion` desteklenir, klavye ile tam gezinilebilir.

## Arama motoru davranışı

Bu sürüm **bilerek dizine kapatılmıştır**: `noindex, nofollow, noarchive`.
Canonical ve hreflang etiketleri ile yapısal veri (JSON-LD) devre dışı bırakılmıştır,
çünkü bu bir örnek çalışmadır ve gerçek alan adına sinyal göndermemesi gerekir.
Ayrıntılar `index.html` dosyasının en üstündeki yorum bloğunda.

> `robots.txt` yalnızca alan adının kökünde geçerlidir. GitHub Pages'te site bir alt
> klasörde yayınlandığı için bu dosya etkisizdir; koruma `<head>` içindeki `noindex`
> etiketiyle sağlanır. Dosya, ileride kök dizine veya kendi alan adına taşınma
> ihtimaline karşı depoda tutulmaktadır.

## Yerelde açmak

Dosyayı çift tıklayıp tarayıcıda açmak yeterlidir. Sunucu gerekmez.
