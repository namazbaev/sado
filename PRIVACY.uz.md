# Sado — maxfiylik siyosati

Oxirgi yangilanish: 2026-yil 3-oktabr. Boshqa tillarda: [English](PRIVACY.en.md), [Русский](PRIVACY.ru.md).

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
| Microsoft — Azure Speech | Sozlamada ovoz dvigateli "Azure" tanlangan bo'lsa | O'zbekcha tarjima jumlalari, sizning Azure API keyingiz bilan `<hudud>.tts.speech.microsoft.com` manziliga |
| Dars sayti (Udemy, master.dev yoki siz yoqqan sayt) | Subtitr yuklanganda | Udemy'da avval Udemy'ning o'z API'siga shu saytda, dars sahifasining o'zi kabi Udemy sessiyangiz bilan so'rov ketadi: joriy darsning nomi va subtitr fayllari ro'yxati so'raladi. Keyin Udemy dars uchun ko'rsatgan yoki dars sahifasining o'zi so'ragan subtitr faylini kengaytma shu saytdan yuklab oladi (cookie'siz) |

Sozlamalar sahifasidagi sinovlar ("Ulanishni tekshirish", "Ovozni eshitish", talaffuzni tinglash) faqat sinov
matnini yoki siz yozgan so'zni o'sha servisga yuboradi — dars matnini emas. Model ro'yxati tanlangan tarjima
servisidan saqlangan API keyingiz bilan so'raladi; bu so'rovda hech qanday matn yo'q.

Har bir servis olgan ma'lumotni o'z shartlari va maxfiylik siyosati bo'yicha qayta ishlaydi.

**Gemini bepul tarifi.** Bepul tarifda Google yuborilgan matndan o'z mahsulotlarini yaxshilash uchun
foydalanishi mumkin. Gemini API'dan faqat 18 yoshdan oshganlar foydalana oladi. Batafsil:
[Gemini API qo'shimcha shartlari](https://ai.google.dev/gemini-api/terms). Buni istamasangiz, ma'lumotdan
o'qitish uchun foydalanmaydigan pullik tarifni yoki boshqa servisni tanlang.

## Rozilik

Rozilik tarjima servisini sozlashda beriladi: tanishuv va sozlamalar sahifasida **Roziman — saqlash va tekshirish**
tugmasining ustida dars subtitri tanlangan servisga, ovoz uchun o'zbekcha matn Microsoft'ga yuborilishi aytiladi.
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
  (O'chiq / Subtitr / Ovoz) va subtitr ko'rinishi, rozilik yozuvi.
- **Lug'atlar** — siz yozgan atamalar va talaffuzlar, tarjima servisidan o'rganilgan atamalar talaffuzi.
- **Tarjima keshi** — har dars uchun: dars identifikatori (siz yoqqan saytlarda — sahifa manzili) va sarlavhasi,
  inglizcha subtitr matni, o'zbekcha tarjima, vaqtlar va qaysi model tarjima qilgani. Kesh o'sha darsni qayta
  ochganingizda servisga qayta pul to'lamaslik uchun kerak.
- **Diagnostika jurnali** — oxirgi 50 ta xatoning kodi (masalan `auth`, `timeout`), ish turi (tarjima, subtitr,
  ovoz, model ro'yxati), vaqti, davomiyligi va soni. Subtitr matni, tarjima va API keylar unga yozilmaydi. Jurnal
  o'zi hech qayerga yuborilmaydi: Sozlamalar → "Diagnostikani nusxalash" uni kengaytma versiyasi, brauzer nomi,
  servis va model nomi hamda ovoz holati bilan birga nusxalaydi, kimga yuborishni esa o'zingiz hal qilasiz.
- **Model tezligi** — oxirgi 20 ta servis va model juftligi uchun: soniyasiga o'rtacha chiqish tokeni, o'lchovlar
  soni va oxirgisining vaqti. Matn saqlanmaydi. "Diagnostikani nusxalash" ga (vaqtsiz) kiradi, o'zi hech qayerga
  yuborilmaydi.

Vaqtinchalik (`chrome.storage.session`, brauzer yopilganda o'chadi): dars sahifasi so'ragan subtitr fayllari va
subtitr manzilini topishga yordam beradigan so'rovlar (masalan master.dev dars ma'lumoti) manzili, turi va qaysi
sahifadan so'ralgani — har varaq uchun ko'pi bilan 50 ta. Varaq yopilganda uning yozuvlari o'chiriladi.
Kengaytma boshqa so'rovlarni saqlamaydi, hech qaysi so'rovni to'smaydi yoki o'zgartirmaydi.

## Qanday o'chirish mumkin

- **Tarjima keshi:** Sozlamalar → "Kutubxona" → darsning o'chirish tugmasi (bitta dars) yoki "Hammasini o'chirish".
- **Tarjima servisi API keyi:** Sozlamalar → "Tarjima" → "API key" → "O'chirish".
- **Hammasi** (Azure API keyi, lug'atlar, o'rganilgan talaffuzlar, rozilik ham): kengaytmani brauzerdan o'chiring —
  brauzer uning barcha mahalliy ma'lumotini ham o'chiradi.
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

[namazbaevshakhzod@gmail.com](mailto:namazbaevshakhzod@gmail.com)
