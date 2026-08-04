# Yo'naltiruvchi — ko'zi ojizlar uchun ilova

## Nima qiladi
- Manzilni ovoz yoki matn bilan kiritasiz
- Kompas orqali qaysi tomonga yurish kerakligini ovozda aytadi
- Kamera orqali oldindagi to'siqlarni (odam, mashina, stul va h.k.) aniqlab, ovozda va tebranish orqali ogohlantiradi

## GitHub'da APK qurish (dasturlash bilmasangiz ham bo'ladi)

1. github.com'da yangi repository (repo) yarating — nomini masalan `blind-navigator` deb qo'ying, **Public** qiling.
2. Repo ichida "Add file" → "Upload files" tugmasini bosing.
3. Ushbu papkadagi barcha fayl va papkalarni (www, config.xml, package.json, .github papkasi ichidagi workflows bilan birga) shu joyga tashlang. Muhim: `.github/workflows/build-apk.yml` fayli papka tuzilishi bilan birga yuklanishi kerak.
4. "Commit changes" tugmasini bosing.
5. Repo ichida yuqoridagi **Actions** bo'limiga o'ting.
6. "APK qurish" ishi avtomatik boshlanadi (bir necha daqiqa davom etadi). Agar boshlanmasa, "Run workflow" tugmasini bosing.
7. Ish tugagach (yashil belgi ✅), o'sha ish sahifasiga kiring va pastda **Artifacts** qismidan `yonaltiruvchi-apk` faylini yuklab oling — bu ZIP ichida APK bo'ladi.
8. APK faylini telefoningizga o'tkazib, o'rnating (noma'lum manbadan o'rnatishga ruxsat berish kerak bo'lishi mumkin).

## Muhim eslatma
- Bu **debug APK** — sinov uchun ishlaydi, lekin Google Play'ga chiqarish uchun keyinroq imzolangan (signed) versiya kerak bo'ladi.
- Ilova internet talab qiladi (manzil qidirish va to'siq aniqlash tizimi uchun).
- Birinchi ochilishda kamera, joylashuv va mikrofonga ruxsat so'raladi — hammasiga "Ruxsat berish" deb bosing.
