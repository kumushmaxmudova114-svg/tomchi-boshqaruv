# Tomchi Somsa — Boshqaruv (GitHub Pages + Firebase)

Bu papkada dadangizning boshqaruv paneli GitHub orqali haqiqiy sayt sifatida joylashtirish uchun tayyor.
Belgi (icon) sifatida sizning "Tomchi Somsa" logotipingiz ishlatilgan.

## 1-qadam: Firebase loyihasi ochish (bepul)

1. https://console.firebase.google.com ga kiring, Google hisobingiz bilan.
2. "Add project" (Loyiha qo'shish) tugmasini bosing, nom bering (masalan "tomchi-somsa"), davom eting.
3. Chap menyudan **Build → Firestore Database** ni oching, "Create database" bosing, **test mode** ni tanlang (keyinroq xavfsizlik qoidalarini kuchaytirish mumkin), yaqin regionni tanlang.
4. Chap menyuda **Project settings** (dvigatel belgisi) → pastga tushib "Your apps" bo'limida **Web (</>) belgisi**ni bosib yangi web-ilova qo'shing (nom istalgan). Sizga `firebaseConfig` degan JavaScript obyekt ko'rsatiladi — shuni nusxalab oling.

## 2-qadam: Config'ni qo'yish

`index.html` faylini oching, ichidan `const firebaseConfig = {...}` qismini toping va Firebase'dan olgan qiymatlaringiz bilan almashtiring.

## 3-qadam: GitHub'ga yuklash

1. https://github.com da yangi repository oching (masalan `tomchi-somsa`), Public qilib qo'ying.
2. Shu papkadagi barcha fayllarni (index.html, manifest.json, service-worker.js, icons/) repositoryga yuklang (GitHub saytida "Add file → Upload files" orqali eng oson).
3. Repository ichida **Settings → Pages** bo'limiga o'ting. "Branch" qismida `main` ni tanlang, saqlang.
4. Bir necha daqiqadan so'ng sizga havola beriladi: `https://SIZNING-USERNAME.github.io/tomchi-somsa/`

## 4-qadam: Telefonga ilova qilib o'rnatish

1. Yuqoridagi havolani telefon brauzerida oching.
2. **Android (Chrome):** o'ng tepadagi ⋮ menyu → "Ilovani o'rnatish" / "Bosh ekranga qo'shish".
3. **iPhone (Safari):** pastdagi ulashish belgisi → "Bosh ekranga qo'shish".
4. Endi telefon ekranida "Tomchi Somsa" nomi va logotipi bilan **alohida ilova** paydo bo'ladi — brauzer manzil satrisiz ochiladi.

## Eslatma

- Bu bosh sahifa hozircha faqat **dadam uchun boshqaruv panelini** o'z ichiga oladi.
- Filiallar (xodimlar) uchun buyurtma kiritish ilovalarini ham xuddi shu tarzda, bir xil Firebase bazasiga ulab, alohida-alohida (masalan `filial1/index.html`, `filial2/index.html`, `filial3/index.html`) qilib beraman — shuni ham xohlasangiz ayting.
- Firestore bepul reja (Spark) kichik oilaviy biznes uchun to'liq yetarli.
