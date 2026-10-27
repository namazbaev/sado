# Maxfiylik siyosati

Kuchga kirgan sana: 2026-yil 28-oktabr · Versiya 1.2

Sado — Chrome va Microsoft Edge uchun kengaytma. U onlayn kurs videolariga o'zbekcha subtitr va ovoz qo'shadi. Bu
sahifada Sado qanday ma'lumot bilan ishlashi, uni qayerda saqlashi va kimga yuborishi yozilgan.

## Qisqacha

- **Sadoning serveri yo'q.** Ma'lumotlaringiz bizga kelmaydi: biz ularni yig'maymiz va saqlamaymiz. Ro'yxatdan
  o'tish ham shart emas.
- **Hammasi brauzeringizda saqlanadi.** API key, sozlamalar, atamalar va saqlangan darslar faqat shu brauzerda
  turadi. Ularni istalgan vaqtda o'chirishingiz mumkin.
- **Matn faqat roziligingiz bilan yuboriladi.** Tarjima uchun dars subtitri siz tanlagan servisga (odatda Google
  Gemini), ovoz uchun esa tarjima matni ovoz servisiga yuboriladi. Bu siz «Roziman» tugmasini bosganingizdan
  keyingina boshlanadi.
- **Reklama va kuzatuv yo'q.** Sado analitika, cookie va reklama ishlatmaydi. Ma'lumotlaringiz sotilmaydi va faqat
  tarjima hamda ovoz uchun ishlatiladi.

## 1. Biz kimmiz

Sadoni Shakhzod Namazbaev ishlab chiqadi va qo'llab-quvvatlaydi (quyida — «biz»). Bu siyosat Chrome Web Store va
Microsoft Edge Add-ons do'konlaridagi Sado kengaytmasiga tegishli.

Savollaringiz bo'lsa, [namazbaevshakhzod@gmail.com](mailto:namazbaevshakhzod@gmail.com) manziliga yozing.

## 2. Sado qanday ishlaydi

Kurs saytida dars ochilganda Sado darsning asl subtitrini (odatda inglizcha) o'sha saytning o'zidan oladi —
sahifa yuklagan subtitr faylidan yoki, Udemy'da, saytning o'z API'sidan, sahifaning o'zi kabi. Keyin subtitrni
tarjima servisiga yuboradi. Tarjima video ustida o'zbekcha subtitr bo'lib chiqadi. Ovoz rejimida tarjimani ovoz
servisi o'qib beradi.

So'rovlar brauzeringizdan to'g'ridan-to'g'ri servisga boradi va siz kiritgan API key bilan yuboriladi. Oraliqda
Sado serveri yo'q, shuning uchun bu ma'lumotlar bizga kelmaydi.

Dars avval tarjima qilingan bo'lsa, Sado tarjimani kutubxonadan oladi va servisga hech narsa yubormaydi.
Sozlamalardagi sinovlar («Ulanishni tekshirish», «Ovozni eshitish», talaffuzni tinglash) dars matnini emas, faqat
namuna jumlani yoki siz yozgan so'zni yuboradi; modellar ro'yxati so'rovida esa matn umuman yo'q.

## 3. Sado qanday ma'lumot bilan ishlaydi

Sado ishlatadigan barcha ma'lumotlar quyidagi jadvalda keltirilgan.

| Ma'lumot | Qayerda saqlanadi | Kimga yuboriladi | Qachongacha saqlanadi |
|---|---|---|---|
| **API key** — tarjima servisi (masalan, Gemini) uchun | Brauzeringizda, kengaytma xotirasida | Faqat shu keyni bergan servisga — har bir so'rov bilan birga | O'zingiz o'chirguningizcha |
| **Dars subtitri** — asl matn va uning tarjimasi | Brauzeringizda, «Kutubxona» bo'limida | Asl matn — tarjima servisiga. Tarjima — ovoz yoqilgan bo'lsa, ovoz servisiga | Kutubxonadan o'chirguningizcha |
| **Dars nomi va identifikatori** (siz yoqqan saytlarda — sahifa manzili) | Kutubxonada — tarjimani kerakli darsga bog'lash uchun | Hech kimga | Kutubxonadan o'chirguningizcha |
| **Atamalar va talaffuz lug'ati** | Brauzeringizda | Tarjima so'rovi bilan birga tarjima servisiga — atamalar siz xohlagandek tarjima qilinishi va o'qilishi uchun | O'zingiz o'chirguningizcha |
| **Ovoz** — Gemini TTS o'qigan audio | Brauzeringizda | Hech kimga: qayta eshitganda jumla servisga qayta yuborilmaydi | Hajm chegarasiga yetganda eng eskisi o'chadi |
| **Sozlamalar** — rejim, ovoz, subtitr ko'rinishi, kunlik limit, rozilik | Brauzeringizda | Hech kimga | Sadoni brauzerdan o'chirib tashlaguningizcha |
| **Ish o'lchovlari** — bugungi sarf, Gemini TTS hisobi, tarjima va ovoz tezligi, oxirgi darslar bo'yicha sanoqlar (dars identifikatori bilan, matnsiz) | Brauzeringizda | Hech kimga. «Diagnostikani nusxalash» ga dars identifikatorisiz kiradi | Har kuni yangilanadi yoki oxirgi 10 dars qoladi; kutubxonadan dars o'chirilganda o'chmaydi |
| **Diagnostika jurnali** — xato kodi, ish turi, vaqti va sayt nomi (masalan, udemy) | Brauzeringizda, oxirgi 50 ta yozuv | Hech kimga. Uni faqat o'zingiz nusxalab yuborishingiz mumkin | Eski yozuvlar o'z-o'zidan o'chadi |
| **Subtitr fayli manzili** — sahifa so'ragan subtitr fayli va o'sha sahifa manzili | Brauzeringizda, vaqtinchalik | Hech kimga | Varaq yoki brauzer yopilguncha |

Diagnostika jurnali va ish o'lchovlariga API key va dars matni yozilmaydi. Gemini TTS hisobi keyning o'zini emas,
undan olingan qaytarib bo'lmaydigan qisqa barmoq izini saqlaydi.

## 4. Biz nimani yig'maymiz

- **Shaxsiy ma'lumotlar** — ism, e-pochta va boshqalar. Sadoda akkaunt yo'q.
- **Brauzer tarixi.** Sado brauzer tarixini saqlamaydi. Sahifa mazmunini faqat kurs saytlarida va siz yoqqan
  saytlarda o'qiydi.
- **Video va audio.** Sado videoni yozib olmaydi va hech qayerga yubormaydi.
- **To'lov ma'lumotlari va joylashuv.**
- **Foydalanish statistikasi.** Sado analitika, cookie, reklama va kuzatuv vositalarini ishlatmaydi.

## 5. Uchinchi tomon servislari

Tarjima va ovoz uchun Sado quyidagi servislardan foydalanadi. Ular yuborilgan matnni o'z shartlari va maxfiylik
siyosatiga ko'ra qayta ishlaydi. Biz bu jarayonni nazorat qila olmaymiz.

- **Google Gemini API** — tarjima (odatiy servis) va Gemini TTS ovozi.
  [Gemini API shartlari](https://ai.google.dev/gemini-api/terms) ·
  [Google maxfiylik siyosati](https://policies.google.com/privacy)
- **Microsoft** — Edge'ning onlayn o'zbek ovozlari.
  [Microsoft maxfiylik bayonoti](https://privacy.microsoft.com/privacystatement)
- **Boshqa tarjima servislari** — Anthropic, OpenAI, OpenRouter yoki Groq. Ulardan birini tanlasangiz, o'sha
  servisning shartlari amal qiladi.

> **Gemini API bepul tarifi haqida.** Bepul tarifda Google yuborilgan matndan o'z mahsulotlarini yaxshilash uchun
> foydalanadi. Bu matnni tekshiruvchi odamlar ham o'qishi mumkin. Shuning uchun maxfiy yoki shaxsiy ma'lumot bor
> darslarda bepul tarifdan foydalanmang. Pullik tarifda shartlar boshqacha — batafsil Google shartlarida.

## 6. Rozilik

Sado biror matnni servisga birinchi marta yuborishdan oldin nima va qayerga yuborilishini ko'rsatadi va
roziligingizni so'raydi. Siz «Roziman» tugmasini bosmaguningizcha hech narsa yuborilmaydi. Rozilik tanlangan
servisga tegishli: boshqa servisga o'tsangiz, qayta so'raladi.

Servislar ro'yxati yoki bu siyosat muhim tarzda o'zgarsa, Sado roziligingizni qayta so'raydi.

Yuborishni istalgan vaqtda to'xtatishingiz mumkin: subtitr va ovozni o'chiring yoki Sozlamalar → Maxfiylik →
«Rozilikni qaytarib olish» tugmasini bosing. Shundan keyin hech narsa yuborilmaydi, ochiq darslarda tarjima va ovoz
darhol to'xtaydi.

## 7. Brauzer ruxsatlari

Sado brauzerdan quyidagi ruxsatlarni so'raydi va ularni faqat ko'rsatilgan maqsadda ishlatadi.

| Ruxsat | Qachon so'raladi | Nima uchun kerak |
|---|---|---|
| **Kurs saytlaridagi ma'lumotni o'qish va o'zgartirish** — Sado doim ishlaydigan saytlar (Udemy, Frontend Masters) uchun | O'rnatish paytida | Dars subtitrini o'qish va video ustida o'zbekcha subtitrni ko'rsatish |
| **Tarjima va ovoz servislari manzillari** — Gemini, Anthropic, OpenAI, OpenRouter, Groq | O'rnatish paytida | So'rovni siz tanlagan servisga to'g'ridan-to'g'ri yuborish. Boshqa servislarga hech narsa ketmaydi |
| **Faqat shu saytga ruxsat** — YouTube va Coursera uchun | Shu saytni yoqqaningizda | Yuqoridagi bilan bir xil, lekin faqat siz yoqqan saytda |
| **Barcha saytlarga ruxsat** — boshqa kurs saytlari uchun | Ro'yxatda yo'q saytni yoqqaningizda | Bunday saytlarda subtitr fayli ko'pincha boshqa manzildan yuklanadi. Sado paneli faqat siz yoqqan saytlarda ishlaydi; boshqa varaqda subtitrga o'xshash so'rov manzili ko'rilsa, u faqat vaqtincha brauzerda qoladi |
| **Xotira** (`storage`, `unlimitedStorage`) | O'rnatish paytida | API key, sozlamalar, atamalar va kutubxonani brauzeringizda saqlash; kutubxona odatiy 10 MB chegaradan katta bo'lishi mumkin |
| **Tarmoq so'rovlarini kuzatish** (`webRequest`) | O'rnatish paytida | Dars sahifasi yuklagan subtitr faylini topish. So'rovlar to'silmaydi va o'zgartirilmaydi |
| **Skript qo'shish** (`scripting`) | O'rnatish paytida | Siz yoqqan saytda va ochiq varaqlarda Sadoni sahifani yangilamasdan ishga tushirish |
| **Joriy varaq** (`activeTab`) | O'rnatish paytida | Sado oynasi ochilganda joriy sayt manzilini bilish — shu saytda yoqishni taklif qilish uchun |
| **Yon panel** (`sidePanel`) | O'rnatish paytida | Darsning matnini brauzer yon panelida ko'rsatish |
| **Fon hujjati** (`offscreen`) | O'rnatish paytida | Sahifa audio ijroga ruxsat bermaganda Gemini TTS ovozini kengaytmaning o'zida ijro etish va ovoz keshi uchun audioni siqish |

Siz yoqqan saytda Sadoni o'chirish uchun Sado oynasida «Bu saytda o'chirish» tugmasini bosing. Shu sayt uchun
berilgan ruxsat ham bekor qilinadi; «Barcha saytlarga ruxsat» esa u bilan yoqilgan oxirgi sayt o'chirilganda
qaytariladi.

## 8. Ma'lumotlarni ko'rish va o'chirish

Asosiy ma'lumotlarni Sado sozlamalarida ko'rishingiz va o'chirishingiz mumkin:

- **API key** — Sozlamalar → Tarjima → API key yonidagi «O'chirish» tugmasi.
- **Saqlangan darslar** — Sozlamalar → Kutubxona → bitta dars yoki «Hammasini o'chirish».
- **Atamalar** — Sozlamalar → Atamalar.
- **Rozilik** — Sozlamalar → Maxfiylik → «Rozilikni qaytarib olish».
- **Hammasini birdan** — Sadoni brauzerdan o'chirib tashlang. Brauzer Sado saqlagan barcha ma'lumotni o'zi
  o'chiradi. Shundan keyin brauzer GitHub'dagi qisqa fikr sahifasini ochadi; uning manziliga hech qanday ma'lumot
  qo'shilmaydi.

Ovoz keshi, ish o'lchovlari va diagnostika jurnalini alohida o'chiradigan tugma yo'q: ular hajm yoki son chegarasida
o'z-o'zidan eskiradi, kutubxonadan dars o'chirilganda esa o'chmaydi. Ularning hammasi Sadoni brauzerdan o'chirganda
o'chadi.

Servislarga yuborilgan matn ularning o'z qoidalari bo'yicha saqlanadi. Uni o'chirish uchun o'sha servisga murojaat
qiling.

## 9. Xavfsizlik

- Barcha so'rovlar shifrlangan HTTPS ulanish orqali yuboriladi.
- API key kengaytma xotirasida saqlanadi — saytlar uni o'qiy olmaydi. Ammo u alohida parol bilan himoyalanmagan:
  kompyuteringizdagi brauzer profilingizga kira oladigan odam uni ko'rishi mumkin. Umumiy kompyuterda ishlagan
  bo'lsangiz, ishdan keyin API keyni o'chiring.
- API keyingizni hech kimga bermang. Agar u begonalarga ma'lum bo'lib qolsa, uni o'sha servis sahifasida (Gemini
  uchun — Google AI Studio) o'chirib, yangisini yarating.

## 10. Bolalar

Sado 18 yoshga to'lmaganlar uchun mo'ljallanmagan: Gemini API shartlariga ko'ra undan faqat 18 yosh va undan katta
odamlar foydalanishi mumkin. Biz hech kimdan, jumladan bolalardan ham, shaxsiy ma'lumot yig'maymiz.

## 11. Chrome Web Store talablari

Sado ma'lumotlardan Chrome Web Store foydalanuvchi ma'lumotlari siyosatiga, jumladan
[«Cheklangan foydalanish» (Limited Use)](https://developer.chrome.com/docs/webstore/program-policies/limited-use/)
talablariga muvofiq foydalanadi. Bu degani: ma'lumotlar faqat Sadoning asosiy vazifasi — darslarni tarjima qilish va
o'qib berish uchun ishlatiladi. Ular sotilmaydi, reklama uchun ishlatilmaydi va kredit to'lash qobiliyatini baholash
uchun berilmaydi.

## 12. Siyosatdagi o'zgarishlar

Siyosat o'zgarsa, yangi matn shu sahifada yangi sana va versiya raqami bilan chiqadi. Muhim o'zgarish bo'lsa
(masalan, yangi servis qo'shilsa), Sado bu haqda kengaytmaning o'zida xabar beradi va roziligingizni qayta so'raydi.
Oldingi versiyalar ro'yxati sahifa oxirida.

## 13. Aloqa

Maxfiylik bo'yicha savol, taklif yoki ma'lumotni o'chirish haqida so'rovingiz bo'lsa,
[namazbaevshakhzod@gmail.com](mailto:namazbaevshakhzod@gmail.com) manziliga yoki Telegram'dagi Sado yordam botiga
[@sado_support_bot](https://t.me/sado_support_bot) yozing. Xatda Sado versiyasini ko'rsating:
Sozlamalar → Yordam → «Diagnostikani nusxalash» uni o'zi qo'shadi.

Botga yozgan xabaringiz, ismingiz va Telegram username'ingiz javob berish uchun Sado muallifiga yetkaziladi. Xabarni
Cloudflare'dagi kichik dastur uzatadi. U xabar matnini saqlamaydi: "yetkazildi" javobini qayta-qayta yubormaslik
uchun faqat Telegram ID'ingiz va vaqtni eslab qoladi va ularni 7 soat ichida o'chiradi. Yozishma Telegram chatlarida
qoladi.

---

Bu siyosat o'zbek, ingliz va rus tillarida e'lon qilingan: [O'zbekcha](PRIVACY.uz.md) · [English](PRIVACY.en.md) ·
[Русский](PRIVACY.ru.md). Tarjimalar orasida farq bo'lsa, o'zbekcha matn asos qilib olinadi.

### Versiyalar tarixi

- **1.2** — 2026-yil 28-oktabr. Aloqa: Telegram'da shaxsiy akkaunt o'rniga Sado yordam boti; botga yozilgan
  xabarlar qanday yetkazilishi.
- **1.1** — 2026-yil 25-oktabr. Azure Speech ovozi olib tashlandi: Sado endi Azure'ga hech narsa yubormaydi,
  avval saqlangan Azure API keyi va hududi yangilanishdan keyin brauzeringizdan o'chiriladi.
- **1.0** — 2026-yil 25-oktabr. Siyosat qayta yozildi: qisqacha, ma'lumotlar va ruxsatlar jadvali, versiya raqami.
