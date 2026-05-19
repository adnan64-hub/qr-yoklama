# QR Yoklama Sistemi

Öğretmen QR kodu oluşturur, öğrenciler telefonuyla okutup numaralarını girerek yoklamaya katılır.

---

## 🚀 Deploy (Yayınlama)

### Vercel ile (önerilen — ücretsiz)

1. [vercel.com](https://vercel.com) adresine gidin, GitHub hesabıyla kayıt olun.
2. Bu klasörü GitHub'a yükleyin **veya** Vercel CLI kullanın:

```bash
npm install -g vercel
cd qr-yoklama
vercel
```

3. Sorulara Enter ile devam edin. Birkaç dakikada link hazır:
   `https://qr-yoklama-xxx.vercel.app`

---

### Netlify ile (alternatif — ücretsiz)

1. [netlify.com](https://netlify.com) → "Add new site" → "Deploy manually"
2. Önce projeyi build edin:

```bash
npm install
npm run build
```

3. Oluşan `dist/` klasörünü Netlify'a sürükle-bırak yapın.

---

### GitHub Pages ile

```bash
npm install
npm run build
# dist klasörünü gh-pages branch'ine push edin
```

---

## 💻 Lokal Çalıştırma

```bash
npm install
npm run dev
```

Tarayıcıda `http://localhost:5173` açın.

---

## 📋 Kullanım

1. **Öğretmen paneli** açılır (varsayılan sayfa)
2. Ders adı, tarih, süre ve öğrenci listesini girin
   - Format: `101 Ahmet Yılmaz` (numara boşluk ad soyad)
3. **"QR OLUŞTUR VE BAŞLAT"** butonuna tıklayın
4. Ekrandaki QR kodu projektöre yansıtın
5. Öğrenciler telefonlarıyla okutup numaralarını girer
6. Katılımlar canlı olarak panelde görünür
7. Süre dolunca veya "Oturumu Kapat" ile sonuçlar gösterilir

---

## ⚙️ Notlar

- Veriler tarayıcı localStorage'ında tutulur (aynı cihaz/ağ)
- QR link süresi dolduğunda otomatik geçersiz olur
- Aynı numara iki kez kayıt olamaz
