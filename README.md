# Gölge Diyarı — yasal sayfalar

Uygulama mağazalarının istediği sayfalar. GitHub Pages ile yayınlanır.

| Sayfa | Ne için |
|---|---|
| `index.html` | Marketing URL (App Store) / Website (Play Console) |
| `privacy.html` | **Privacy Policy URL** — iki mağazada da zorunlu |
| `terms.html` | Kullanım koşulları |
| `support.html` | **Support URL** — App Store'da zorunlu |

## Yayınlamak

GitHub'da: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)`**

Bir iki dakika sonra adresler:

```
https://KULLANICI.github.io/golgeDiyariSozlesme/
https://KULLANICI.github.io/golgeDiyariSozlesme/privacy.html
https://KULLANICI.github.io/golgeDiyariSozlesme/terms.html
https://KULLANICI.github.io/golgeDiyariSozlesme/support.html
```

## Önce yapılacak tek şey

Üç sayfada `BURAYA_EPOSTA` yer tutucusu var. Mağazalar bir destek adresi şart
koşuyor; kendi adresini koymadan yayınlama:

```sh
cd golgeDiyariSozlesme
sed -i '' 's/BURAYA_EPOSTA/senin@adresin.com/g' *.html
```

## Gizlilik metni neden bu kadar kısa

Çünkü uygulama gerçekten hiçbir şey toplamıyor. Kodda ağ çağrısı yok, analitik
yok, reklam yok; tek saklama cihazın kendi deposunda tutulan oyun kaydı.
Mağaza formlarında da "Data Not Collected" / "No data collected" seçilecek.

**Online Pazar geldiğinde bu değişecek.** Oyuncular arası alışveriş sunucu ve
hesap demek; o özellik yazılmadan önce bu politikanın yeniden yazılması gerekir.
