# Portfolio Sayti — Muhammadsino Muhammatoirov

Backend muhandis uchun mo'ljallangan, qorong'i va hashamatli uslubdagi bir sahifali (single-page) portfolio sayti. Dizayn "mukofot plitasi" (plaque) motividan ilhomlangan — oltin ranglar, nafis serif shrift va aniq strukturaga ega.

## Fayl tuzilishi

```
portfolio.html   → to'liq sayt (HTML + CSS + JS bitta faylda)
README.md        → ushbu qo'llanma
```

Saytni ochish uchun shunchaki `portfolio.html` faylini istalgan brauzerda oching — hech qanday o'rnatish yoki server talab qilinmaydi.

## Bo'limlar

| Bo'lim | Tavsif |
|---|---|
| Hero | Ism, lavozim va qisqa statistik ma'lumotlar |
| Men haqimda | Ish uslubi va asosiy tamoyillar |
| Ko'nikmalar | Texnologiyalar (Backend, DevOps, Arxitektura) |
| Loyihalar | Tanlangan 4 ta ish namunasi |
| Tajriba | Karyera yo'nalishi va mukofotlar |
| Aloqa | Email va ijtimoiy tarmoq havolalari |

## Matnni o'zgartirish

Barcha matnlar `portfolio.html` faylining ichida oddiy o'zbek tilida yozilgan — dasturlash bilimisiz ham `<h1>`, `<p>`, `<h3>` teglari ichidagi matnni topib, o'zingizning ma'lumotlaringizga almashtirsangiz bo'ldi. Masalan:

- **Ism/lavozim** — `.plaque-name` va `.plaque-role` klasslari yaqinida
- **Loyihalar** — `id="work"` bo'limi ichidagi `.project` bloklari
- **Tajriba** — `id="experience"` bo'limidagi `.tl-item` bloklari
- **Aloqa havolalari** — `id="contact"` bo'limidagi `<a href="...">` manzillari (email, LinkedIn, GitHub, Telegram)

## Rasmni almashtirish

Hozirgi profil rasmi fayl ichiga base64 formatda joylashtirilgan (`data:image/png;base64,...`). O'z rasmingizni qo'yish uchun:
1. Yangi rasmni [base64.guru](https://base64.guru/converter/encode/image) kabi saytda base64 formatga o'giring
2. `src="data:image/png;base64,..."` qismini yangi kod bilan almashtiring

## Onlayn joylashtirish (deploy)

Sayt bitta statik HTML fayl bo'lgani uchun quyidagi bepul xizmatlarning istalganiga yuklab qo'yishingiz mumkin:

- **GitHub Pages** — repozitoriyga yuklab, Settings → Pages orqali yoqing
- **Netlify** — `portfolio.html` faylini `index.html` deb nomlab, saytga sudrab tashlash (drag & drop) yetarli
- **Vercel** — GitHub repozitoriyni ulash orqali avtomatik deploy

## Texnik tafsilotlar

- Shriftlar: Google Fonts orqali `Fraunces` (sarlavhalar), `Inter` (matn), `JetBrains Mono` (texnik yorliqlar)
- Alohida kutubxona yoki freymvork talab qilinmaydi
- To'liq responsiv — mobil qurilmalarda ham to'g'ri ko'rinadi
- Scroll paytida animatsiyalar `IntersectionObserver` orqali ishlaydi

## Keyingi qadam

Menga quyidagi ma'lumotlarni yuborsangiz, barcha namunaviy matnlarni haqiqiysiga almashtirib beraman:
- Ism, lavozim, qisqa bio
- Haqiqiy loyihalar va ishlatilgan texnologiyalar
- Ish tajribasi va kompaniyalar
- Email, LinkedIn, GitHub, Telegram havolalari
