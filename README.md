# Tente Dijital — site

Tente Dijital'in tek sayfalık tanıtım sitesi. Derleme adımı yok: düz HTML + CSS, GitHub Pages'ten yayınlanır.

- Yayın adresi: https://tentedijital.github.io/
- Depo: `tentedijital/tentedijital.github.io` (`main` dalı, kök klasör)

## Dosyalar

| Dosya | Ne işe yarar |
|---|---|
| `index.html` | Sayfanın tamamı |
| `assets/style.css` | Tasarım |
| `assets/logo.svg`, `logo.png` | Ana logo (açık zemin) |
| `assets/logo-beyaz.svg`, `logo-beyaz.png` | Koyu zemin için logo |
| `assets/ikon.svg`, `ikon-1024.png` | İkon: tenteli dükkân, lacivert zemin |
| `assets/ikon-acik.svg`, `ikon-acik-1024.png` | İkon: beyaz zemin |
| `assets/profil-1024.png` | WhatsApp / Instagram profil fotoğrafı (daire kesimine uygun) |
| `assets/favicon.svg`, `apple-touch-icon.png` | Tarayıcı ve telefon simgesi |
| `assets/og.png` | Link paylaşınca çıkan önizleme görseli (1200×630) |
| `assets/ornek-tuzla.jpg` | Örnek çalışma görseli |

Sayfadaki tüm bağlantılar göreli (`assets/...`, `./`), bu yüzden site hangi adreste yayınlanırsa yayınlansın çalışır.

## Alan adı alınınca (ör. tentedijital.com)

1. Depo köküne `CNAME` adlı bir dosya ekleyin, içine tek satır yazın: `tentedijital.com`
2. Şu üç dosyada `https://tentedijital.github.io` adresini `https://tentedijital.com` yapın:
   `index.html` (canonical, og:url, og:image, JSON-LD), `sitemap.xml`, `robots.txt`
3. Alan adı firmasının DNS panelinde:
   - `A` kayıtları (kök alan adı için): `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` kaydı: `www` → `tentedijital.github.io`
4. GitHub'da depo → Settings → Pages → Custom domain alanına `tentedijital.com` yazın, DNS yayılınca "Enforce HTTPS" kutusunu işaretleyin.

Eski `tentedijital.github.io` adresi yeni alan adına kendiliğinden yönlenir.

## İletişim bilgisi değişirse

WhatsApp numarası `index.html` içinde `wa.me/905356052888` olarak 5 yerde geçer; telefon `tel:+905356052888`, e-posta `mailto:` bağlantısındadır. Instagram hesabı açılınca iletişim bölümüne ve JSON-LD'ye (`sameAs`) eklenebilir.

## Yazı tipleri

Bricolage Grotesque (başlık) ve Manrope (metin), Google Fonts'tan yüklenir; ikisi de SIL Open Font License ile ücretsizdir. Logo dosyalarındaki harfler vektöre çevrilmiştir, yazı tipi gerektirmez.
