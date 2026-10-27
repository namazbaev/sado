# Privacy policy

Effective date: October 28, 2026 · Version 1.2

Sado is an extension for Chrome and Microsoft Edge. It adds Uzbek subtitles and voice-over to online course videos.
This page explains what data Sado works with, where it is stored and who it is sent to.

## In short

- **Sado has no server.** Your data never reaches us: we don't collect or store it. You don't need to sign up
  either.
- **Everything stays in your browser.** Your API key, settings, glossary and saved lessons stay in this browser
  only. You can delete them at any time.
- **Text is sent only with your consent.** For translation, the lesson subtitles go to the service you choose
  (usually Google Gemini); for voice-over, the translated text goes to a speech service. This starts only after
  you click «Roziman» ("I agree").
- **No ads, no tracking.** Sado uses no analytics, cookies or ads. Your data is never sold and is used only for
  translation and voice-over.

## 1. Who we are

Sado is developed and maintained by Shakhzod Namazbaev ("we"). This policy applies to the Sado extension in the
Chrome Web Store and Microsoft Edge Add-ons.

If you have questions, write to [namazbaevshakhzod@gmail.com](mailto:namazbaevshakhzod@gmail.com).

## 2. How Sado works

When you open a lesson on a course site, Sado takes the lesson's original subtitles (usually English) from that
site itself — from the subtitle file the page loads or, on Udemy, from the site's own API, just as the page does.
It then sends the subtitles to the translation service. The translation appears over the video as Uzbek subtitles.
In voice mode, a speech service reads the translation aloud.

Requests go straight from your browser to the service, with the API key you entered. There is no Sado server in
between, so this data never reaches us.

If a lesson was translated before, Sado takes the translation from the Library and sends nothing to the service.
The tests in Settings ("Ulanishni tekshirish" — check connection, "Ovozni eshitish" — hear the voice, the pronunciation
preview) send only a sample sentence or a word you typed, not lesson text; the model list request contains no text at
all.

## 3. What data Sado handles

The table lists every type of data Sado uses.

| Data | Where it's stored | Who it's sent to | How long it's kept |
|---|---|---|---|
| **API key** — for the translation service (for example, Gemini) | In your browser, in extension storage | Only to the service that issued the key — with each request | Until you delete it |
| **Lesson subtitles** — original text and translation | In your browser, in Kutubxona (the Library) | Original — to the translation service. Translation — to the speech service if voice is on | Until you delete the lesson from the Library |
| **Lesson title and identifier** (on sites you turn on — the page address) | In the Library — to link a translation to the right lesson | No one | Until you delete the lesson from the Library |
| **Glossary and pronunciation list** | In your browser | Included in translation requests, so terms are translated and read the way you set them | Until you delete it |
| **Voice** — audio read by Gemini TTS | In your browser | No one: replaying a line doesn't send it to the service again | The oldest is removed when the size limit is reached |
| **Settings** — mode, voice, subtitle style, daily limit, consent | In your browser | No one | Until the extension is removed |
| **Usage measurements** — today's usage, Gemini TTS count, translation and voice speed, counts for recent lessons (with the lesson identifier, no text) | In your browser | No one. Included in "Diagnostikani nusxalash" (copy diagnostics) without the lesson identifier | Reset daily or kept for the last 10 lessons; not removed when you delete a lesson from the Library |
| **Diagnostics log** — error code, task type, time and site name (for example, udemy) | In your browser, last 50 entries | No one — unless you copy and send it yourself | Old entries are removed automatically |
| **Subtitle file address** — the subtitle file a page requested and that page's address | In your browser, temporarily | No one | Until the tab or browser is closed |

The diagnostics log and usage measurements never contain your API key or lesson text. The Gemini TTS count stores
a short one-way fingerprint of the key, not the key itself.

## 4. What we don't collect

- **Personal details** — your name, email and the like. Sado has no accounts.
- **Browsing history.** Sado doesn't keep your browsing history. It reads page content only on course sites and
  sites you turn on.
- **Video or audio.** Sado doesn't record the video or send it anywhere.
- **Payment details or location.**
- **Usage statistics.** Sado uses no analytics, cookies, ads or tracking tools.

## 5. Third-party services

For translation and voice-over, Sado works with the services below. They process the text you send under their own
terms and privacy policies, which we don't control.

- **Google Gemini API** — translation (default) and the Gemini TTS voice.
  [Gemini API Terms](https://ai.google.dev/gemini-api/terms) ·
  [Google Privacy Policy](https://policies.google.com/privacy)
- **Microsoft** — Edge's online Uzbek voices.
  [Microsoft Privacy Statement](https://privacy.microsoft.com/privacystatement)
- **Another translation service you choose** — Anthropic, OpenAI, OpenRouter or Groq. That service's terms apply.

> **About the Gemini API free tier.** On the free tier, Google uses the text you send to improve its products, and
> people may review it. Don't use the free tier for lessons that contain confidential or personal information. Paid
> tiers have different terms — see Google's terms for details.

## 6. Consent

Before sending any text to a service for the first time, Sado shows what will be sent and where, and asks for your
consent. Nothing is sent until you click «Roziman» ("I agree"). Consent covers the selected service: if you switch to
another one, Sado asks again.

If the list of services or this policy changes significantly, Sado asks for consent again.

You can stop sending at any time: turn off subtitles and voice, or click «Rozilikni qaytarib olish» (withdraw
consent) in Settings → Maxfiylik (Privacy). After that nothing is sent, and translation and voice stop at once in open
lessons.

## 7. Browser permissions

Sado asks the browser for the permissions below and uses each one only for the stated purpose.

| Permission | When it's requested | Why it's needed |
|---|---|---|
| **Read and change data on course sites** — the sites where Sado always works (Udemy, Frontend Masters) | At install | To read lesson subtitles and show Uzbek subtitles over the video |
| **Translation and speech service addresses** — Gemini, Anthropic, OpenAI, OpenRouter, Groq | At install | To send requests straight to the service you chose. Nothing goes to the other services |
| **Access to this site only** — for YouTube and Coursera | When you turn the site on | Same as above, but only on the site you turned on |
| **Access to all sites** — for other course sites | When you turn on a site that isn't listed | On such sites the subtitle file is often loaded from another address. The Sado panel runs only on sites you turned on; if another tab requests something that looks like a subtitle file, its address stays only temporarily in your browser |
| **Storage** (`storage`, `unlimitedStorage`) | At install | To keep your API key, settings, glossary and Library in your browser; the Library can grow past the usual 10 MB limit |
| **Observe network requests** (`webRequest`) | At install | To find the subtitle file the lesson page loads. Requests are never blocked or changed |
| **Run scripts** (`scripting`) | At install | To start Sado on sites you turned on and in open tabs without reloading the page |
| **Current tab** (`activeTab`) | At install | To know the current site's address when you open the Sado window, so it can offer to turn Sado on there |
| **Side panel** (`sidePanel`) | At install | To show the lesson transcript in the browser's side panel |
| **Offscreen document** (`offscreen`) | At install | To play the Gemini TTS voice inside the extension when the page doesn't allow audio playback, and to compress audio for the voice cache |

To turn Sado off on a site you turned on, click «Bu saytda o'chirish» (turn off on this site) in the Sado window.
The permission for that site is removed as well; "access to all sites" is removed when the last site turned on with
it is turned off.

## 8. Viewing and deleting your data

You can view and delete the main data in Sado's settings:

- **API key** — Settings → Tarjima (Translation) → the «O'chirish» (Delete) button
  next to the API key.
- **Saved lessons** — Settings → Kutubxona (Library) → a single lesson or «Hammasini o'chirish» (Delete all).
- **Glossary** — Settings → Atamalar (Terms).
- **Consent** — Settings → Maxfiylik (Privacy) → «Rozilikni qaytarib olish» (withdraw consent).
- **Everything at once** — remove Sado from your browser. The browser deletes everything Sado stored. It then opens
  a short feedback page on GitHub; nothing is added to its address.

The voice cache, usage measurements and diagnostics log have no separate delete button: they expire on their own at
their size or count limits and are not removed when you delete a lesson from the Library. All of them are deleted when
you remove Sado from your browser.

Text sent to the services is kept under their own rules. To delete it, contact that service.

## 9. Security

- All requests are sent over an encrypted HTTPS connection.
- Your API key is kept in extension storage — websites can't read it. It isn't protected by a separate password,
  though: anyone with access to your browser profile on this computer could see it. If you used a shared computer,
  delete the API key when you're done.
- Never share your API key. If it leaks, delete it on that service's website (for Gemini — Google AI Studio) and
  create a new one.

## 10. Children

Sado is not intended for anyone under 18: under the Gemini API terms, only people aged 18 or older may use it. We
don't collect personal data from anyone, including children.

## 11. Chrome Web Store requirements

Sado's use of data complies with the Chrome Web Store User Data Policy, including the
[Limited Use](https://developer.chrome.com/docs/webstore/program-policies/limited-use/) requirements. This means
data is used only for Sado's single purpose — translating lessons and reading them aloud. It is never sold, never
used for advertising and never used to determine creditworthiness.

## 12. Changes to this policy

If this policy changes, the new text appears on this page with a new date and version number. If the change is
significant (for example, a new service is added), Sado tells you in the extension and asks for your consent again.
Previous versions are listed at the end of the page.

## 13. Contact

For privacy questions, suggestions or data deletion requests, write to
[namazbaevshakhzod@gmail.com](mailto:namazbaevshakhzod@gmail.com) or to the Sado support bot on Telegram,
[@sado_support_bot](https://t.me/sado_support_bot). Please include your Sado version: Settings → Yordam
(Help) → «Diagnostikani nusxalash» (copy diagnostics) adds it for you.

Messages you send to the bot, along with your name and Telegram username, are passed to the Sado author so they can
reply. A small program on Cloudflare relays them. It does not store message text: to avoid repeating the "delivered" reply,
it keeps only your Telegram ID and the time, and deletes them within 7 hours. The conversation stays in Telegram
chats.

---

This policy is published in Uzbek, English and Russian: [O'zbekcha](PRIVACY.uz.md) · [English](PRIVACY.en.md) ·
[Русский](PRIVACY.ru.md). If the versions differ, the Uzbek text prevails.

### Version history

- **1.2** — October 28, 2026. Contact: the Sado support bot on Telegram instead of a personal account; how messages
  to the bot are delivered.
- **1.1** — October 25, 2026. The Azure Speech voice was removed: Sado no longer sends anything to Azure, and a
  previously saved Azure API key and region are deleted from your browser after the update.
- **1.0** — October 25, 2026. Policy rewritten: summary, data and permissions tables, version number.
