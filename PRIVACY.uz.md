# Sado — maxfiylik siyosati

Oxirgi yangilanish: 2026-yil 24-oktabr. Boshqa tillarda: [English](PRIVACY.en.md), [Русский](PRIVACY.ru.md).

Sado — kurs videolarining inglizcha subtitrini o'zbekchaga tarjima qilib, video ustida o'zbekcha subtitr sifatida
ko'rsatadigan yoki video bilan sinxron o'zbekcha ovozda o'qib beradigan brauzer kengaytmasi.

## Qisqacha

- Sado'da analitika, telemetriya, reklama yoki kuzatuv kodi yo'q. Kengaytma muallifining serveri yo'q: Sado
  bizga hech qanday ma'lumot yubormaydi.
- Ma'lumot faqat quyidagi jadvaldagi, siz o'zingiz tanlagan servislarga ketadi — va faqat tarjima servisini
  sozlashda rozilik berganingizdan keyin.
- API keylaringiz, sozlamalar va tarjima keshi faqat shu brauzer profilida saqlanadi.

## Kimga nima yuboriladi

| Oluvchi | Qachon | Nima yuboriladi |
|---|---|---|
| Siz sozlamada tanlagan **bitta** tarjima servisi: Google (Gemini API), Anthropic, OpenAI, OpenRouter yoki Groq | Dars tarjima qilinganda | Joriy darsning inglizcha subtitr matni (jumlalar va ularning qo'shni jumlalari), lug'atingizdagi o'zgarmas qoladigan atamalar, talaffuzi o'rganiladigan texnik atamalar ro'yxati va model nomi. So'rov servis API'siga to'g'ridan-to'g'ri, sizning API keyingiz bilan ketadi |
| Microsoft — Edge brauzerining onlayn ovozlari ("Online (Natural)": Sardor, Madina) | Edge'da onlayn o'zbek ovozi dublyaj qilganda | O'zbekcha tarjima jumlalari. Edge ularni o'qish uchun Microsoft'ning bulut servisiga yuboradi |
| Google — Gemini TTS (model `gemini-3.8-flash-lite-tts`) | Brauzerda o'zbek ovozi bo'lmasa (masalan Google Chrome) va tanlangan tarjima servisi Google (Gemini) bo'lsa | O'zbekcha tarjima jumlalari (bir so'rovda bir nechta), o'sha Gemini API keyingiz bilan `generativelanguage.googleapis.com` manziliga. Brauzerda o'zbek ovozi bor Edge'da va boshqa tarjima servislari bilan ishlatilmaydi |
| Microsoft — Azure Speech | Sozlamada ovoz dvigateli "Azure" tanlangan bo'lsa | O'zbekcha tarjima jumlalari, sizning Azure API keyingiz bilan `<hudud>.tts.speech.microsoft.com` manziliga |
| Dars sayti (Udemy, master.dev yoki siz yoqqan sayt) | Subtitr yuklanganda | Udemy'da avval Udemy'ning o'z API'siga shu saytda, dars sahifasining o'zi kabi Udemy sessiyangiz bilan so'rov ketadi: joriy darsning nomi va subtitr fayllari ro'yxati so'raladi. Keyin Udemy dars uchun ko'rsatgan yoki dars sahifasining o'zi so'ragan subtitr faylini kengaytma shu saytdan yuklab oladi (cookie'siz). YouTube'da (siz yoqqan sayt) YouTube player'ining o'zi so'ragan subtitrning inglizcha treki cookie'siz yuklanadi; CC o'chiq bo'lsa, kengaytma shu so'rov uchun CC'ni yoqadi va keyin yana o'chiradi |

Sozlamalar sahifasidagi sinovlar ("Ulanishni tekshirish", "Ovozni eshitish", talaffuzni tinglash) faqat sinov
matnini yoki siz yozgan so'zni o'sha servisga yuboradi — dars matnini emas. Model ro'yxati tanlangan tarjima
servisidan saqlangan API keyingiz bilan so'raladi; bu so'rovda hech qanday matn yo'q.

Har bir servis olgan ma'lumotni o'z shartlari va maxfiylik siyosati bo'yicha qayta ishlaydi.

**Gemini bepul tarifi.** Bepul tarifda Google yuborilgan matndan (tarjima ham, Gemini TTS ham) o'z mahsulotlarini yaxshilash uchun
foydalanishi mumkin. Gemini API'dan faqat 18 yoshdan oshganlar foydalana oladi. Batafsil:
[Gemini API qo'shimcha shartlari](https://ai.google.dev/gemini-api/terms). Buni istamasangiz, ma'lumotdan
o'qitish uchun foydalanmaydigan pullik tarifni yoki boshqa servisni tanlang.

## Rozilik

Rozilik tarjima servisini sozlashda beriladi: tanishuv va sozlamalar sahifasida **Roziman — saqlash va tekshirish**
tugmasining ustida dars subtitri tanlangan servisga, ovoz uchun o'zbekcha matn Microsoft'ga yoki (brauzerda o'zbek ovozi bo'lmasa va servis Gemini bo'lsa) Google'ga yuborilishi aytiladi.
Rozilik faqat tanlangan servisga tegishli: boshqasiga o'tsangiz, qayta so'raladi. Rozilik yo'q bo'lsa (masalan
servis almashgan yoki oluvchilar ro'yxati o'zgargan), panelda **Roziman** tugmali qisqa so'rov chiqadi; uni
bosmaguningizcha hech narsa yuborilmaydi. To'liq ro'yxat (oluvchilar, qurilmada nima qoladi, Gemini sharti)
sozlamalar sahifasining "Maxfiylik" bo'limida. Rozilik (versiya, servis va sana) shu qurilmada saqlanadi.
Rozilikni istalgan vaqtda qaytarib olishingiz mumkin: Sozlamalar → "Maxfiylik" → **Rozilikni qaytarib olish**.
Shundan keyin dars matni hech qayerga yuborilmaydi, ochiq darslarda tarjima va ovoz darhol to'xtaydi.

## Qurilmada nima saqlanadi

Brauzerning kengaytma xotirasida (`chrome.storage.local`), faqat shu brauzer profilida. Boshqa qurilmaga
sinxronlanmaydi.

- **API keylari** (tarjima servisi, Azure) — kengaytmaning fon qismida. Veb-sahifa ham, sahifadagi
  kengaytma skripti ham ularni o'qiy olmaydi.
- **Sozlamalar** — tanlangan servis va model, ovoz dvigateli va tanlangan ovoz, Azure hududi, panel rejimi
  (O'chiq / Subtitr / Ovoz) va subtitr ko'rinishi, rozilik yozuvi, siz qo'ygan kunlik token chegarasi.
- **Lug'atlar** — siz yozgan atamalar va talaffuzlar, tarjima servisidan o'rganilgan atamalar talaffuzi.
- **Tarjima keshi** — har dars uchun: dars identifikatori (siz yoqqan saytlarda — sahifa manzili) va sarlavhasi,
  inglizcha subtitr matni, o'zbekcha tarjima, vaqtlar va qaysi model tarjima qilgani. Kesh o'sha darsni qayta
  ochganingizda servisga qayta pul to'lamaslik uchun kerak.
- **Ovoz keshi** — kengaytmaning IndexedDB'ida: Azure yoki Gemini TTS sintez qilgan audio, shunda qayta eshitganda
  jumlalar qayta yuborilmaydi.
- **Gemini TTS kunlik hisobi** — bugungi sana, shu kunda yuborilgan ovoz so'rovlari soni va limit tugaganmi, hamda
  API keyning qaytarib bo'lmaydigan barmoq izi (SHA-256 boshi, key'ning o'zi emas). Panel qancha ovoz qolganini
  shundan ko'rsatadi; yozuv har kuni yangilanadi va hech qayerga yuborilmaydi.
- **Diagnostika jurnali** — oxirgi 50 ta xatoning kodi (masalan `auth`, `timeout`), ish turi (tarjima, subtitr,
  ovoz, model ro'yxati), vaqti, davomiyligi va soni, subtitr xatosida esa qaysi saytda (masalan `udemy`; sahifa
  manzili emas). Subtitr matni, tarjima va API keylar unga yozilmaydi. Jurnal
  o'zi hech qayerga yuborilmaydi: Sozlamalar → "Yordam" → "Diagnostikani nusxalash" uni kengaytma versiyasi,
  brauzer nomi, servis va model nomi hamda ovoz holati bilan birga nusxalaydi, kimga yuborishni esa o'zingiz hal
  qilasiz. "Telegram'da xabar berish" ham faqat nusxalaydi va dasturchining Telegram sahifasini ochadi: xabarni
  o'zingiz yozasiz va yuborasiz.
- **Model tezligi** — oxirgi 20 ta servis va model juftligi uchun: soniyasiga o'rtacha chiqish tokeni, o'lchovlar
  soni va oxirgisining vaqti. Matn saqlanmaydi. "Diagnostikani nusxalash" ga (vaqtsiz) kiradi, o'zi hech qayerga
  yuborilmaydi.
- **Kunlik sarf** — bugungi sana, shu kunda servis javob bergan so'rovlar (tarjima va Gemini TTS) soni va ular
  sarflagan tokenlar. Sado siz qo'ygan kunlik chegarada shundan to'xtaydi va chegara maydoni ostida bugungi sarfni
  ko'rsatadi; yozuv har kuni yangilanadi va hech qayerga yuborilmaydi.
- **Ovoz sinxronligi** — oxirgi 10 ta dars uchun: sayt, dars identifikatori, ovoz dvigateli va ovoz videoga
  qanchalik ulgurgani (eng katta kechikish, sekinlashtirilgan soniyalar, to'xtashlar, o'qilgan va tashlab ketilgan
  jumlalar soni). Matn saqlanmaydi. "Diagnostikani nusxalash" ga dars identifikatorisiz kiradi, o'zi hech qayerga
  yuborilmaydi.
- **Tarjima o'lchovi** — oxirgi 10 ta dars uchun (boshqa model bilan qayta tarjima qilingan dars alohida yozuv
  oladi): sayt, dars identifikatori, servis va model, nechta jumla tarjima qilingani, servis nechta so'rovga javob
  bergani va ular sarflagan tokenlar (o'ylash va keshdan o'qilgan tokenlar bilan), nechta so'rov qayta yuborilgani,
  bo'lingani, rad etilgani yoki javob chegarasida kesilgani, nechta tarjima jumla vaqtiga sig'magani, inglizcha
  qolgani yoki lotin bo'lmagan harf bilan chiqqani. Matn saqlanmaydi. "Diagnostikani nusxalash" ga dars
  identifikatorisiz kiradi, o'zi hech qayerga yuborilmaydi.
- **Ovoz vaqti** — oxirgi 10 ta ishlatilgan ovoz uchun o'lchangan nutq tezligi va boshlanish kechikishi: ovoz har
  jumlaning vaqtiga sig'ishi uchun. Matn saqlanmaydi.
- **Yangilanish belgisi** — Sado qaysi versiyaga yangilangani (faqat versiya raqami): popup "Sado yangilandi"
  ro'yxatini ko'rsatadi, "Tushunarli" bosilganda yozuv o'chiriladi.

Vaqtinchalik (`chrome.storage.session`, brauzer yopilganda o'chadi): dars sahifasi so'ragan subtitr fayllari va
subtitr manzilini topishga yordam beradigan so'rovlar (masalan master.dev dars ma'lumoti) manzili, turi va qaysi
sahifadan so'ralgani — har varaq uchun ko'pi bilan 50 ta. Varaq yopilganda uning yozuvlari o'chiriladi.
Kengaytma boshqa so'rovlarni saqlamaydi, hech qaysi so'rovni to'smaydi yoki o'zgartirmaydi.

## Qanday o'chirish mumkin

- **Tarjima keshi:** Sozlamalar → "Kutubxona" → darsning o'chirish tugmasi (bitta dars) yoki "Hammasini o'chirish".
- **Tarjima servisi API keyi:** Sozlamalar → "Tarjima" → "API key" → "O'chirish".
- **Hammasi** (Azure API keyi, lug'atlar, o'rganilgan talaffuzlar, rozilik ham): kengaytmani brauzerdan o'chiring —
  brauzer uning barcha mahalliy ma'lumotini ham o'chiradi. Shundan keyin brauzer ochiq repodagi qisqa
  [fikr sahifasini](https://github.com/namazbaev/sado/blob/main/FEEDBACK.md) ochadi (nima yoqmaganini Telegram'da so'raydi). Manziliga hech qanday ma'lumot
  qo'shilmaydi; sahifani GitHub odatdagi sahifa kabi ko'rsatadi.
- Servislar tomonidagi ma'lumot o'sha servisning siyosati bo'yicha o'chiriladi.

## Sotilmaydi va uzatilmaydi

Sado ma'lumotni sotmaydi, reklama uchun ishlatmaydi va yuqorida nomlangan, siz tanlagan servislardan boshqa
hech kimga bermaydi. Ma'lumot faqat kengaytmaning yagona vazifasi — subtitrni tarjima qilish va ovozlash — uchun
ishlatiladi. Chrome Web Store'ning foydalanuvchi ma'lumotlari siyosatiga, jumladan Limited Use talablariga amal
qilinadi.

## Bolalar

Sado 13 yoshgacha bolalarga mo'ljallanmagan. Gemini API'dan foydalanish uchun 18 yosh talab qilinadi.

## O'zgarishlar

Siyosat o'zgarsa, shu hujjat yangilanadi. Ma'lumot oluvchilar ro'yxati o'zgarsa, kengaytma yangi servisga
birinchi so'rovdan oldin rozilikni qayta so'raydi.

## Aloqa

Telegram: [t.me/shakhzod_namazbaev](https://t.me/shakhzod_namazbaev) · E-pochta:
[namazbaevshakhzod@gmail.com](mailto:namazbaevshakhzod@gmail.com)
