# Sado — Privacy Policy

Last updated: October 7, 2026. Other languages: [O'zbekcha](PRIVACY.uz.md), [Русский](PRIVACY.ru.md).

Sado is a browser extension that translates the English subtitles of course videos into Uzbek and shows them as
Uzbek subtitles over the video or reads them aloud in Uzbek in sync with the video.

## Summary

- Sado contains no analytics, telemetry, advertising or tracking code. The author runs no server: Sado sends
  nothing to us.
- Data goes only to the services listed below that you choose — and only after you agree when setting up the
  translation service.
- Your API keys, settings and translation cache are stored only in this browser profile.

## Who receives what

| Recipient | When | What is sent |
|---|---|---|
| The **one** translation service you select in the settings: Google (Gemini API), Anthropic, OpenAI, OpenRouter or Groq | When a lesson is translated | The English subtitle text of the current lesson (sentences and their neighbouring sentences), the terms from your glossary that must stay unchanged, a list of technical terms whose pronunciation is learned, and the model name. The request goes directly to the service's API with your API key |
| Microsoft — the Edge browser's online voices ("Online (Natural)": Sardor, Madina) | When an online Uzbek voice in Edge reads the dub | The Uzbek translated sentences. Edge sends them to Microsoft's cloud service to be spoken |
| Google — Gemini voice (model `gemini-3.8-flash-lite-tts`) | Only if the browser has no Uzbek voice (for example Google Chrome) and the selected translation service is Google (Gemini) | The Uzbek translated sentences (several per request), with the same Gemini API key, to `generativelanguage.googleapis.com`. Not used in Edge, where the browser has an Uzbek voice, and not used with other translation services |
| Microsoft — Azure Speech | Only if "Azure" is selected as the voice engine | The Uzbek translated sentences, with your Azure key, to `<region>.tts.speech.microsoft.com` |
| The lesson site (Udemy, master.dev or a site you enabled) | When subtitles are loaded | On Udemy, first a request to Udemy's own API on the same site, with your Udemy session as the lesson page itself does, for the current lesson's title and list of subtitle files. Then the extension downloads from that site, without cookies, a subtitle file Udemy listed for the lesson or the lesson page itself requested |

The tests on the settings page ("Ulanishni tekshirish" — test connection, "Ovozni eshitish" — play voice sample, and
listening to a pronunciation) send only the test text or the word you typed to that service — never lesson text.
The model list is requested from the selected translation service with your saved key; that request contains no
text.

Each service processes the data it receives under its own terms and privacy policy.

**Gemini free tier.** On the free tier Google may use the text you send (both for translation and for the Gemini voice) to improve its products. The Gemini API
may be used only by people aged 18 or over. Details: [Gemini API Additional Terms of Service](https://ai.google.dev/gemini-api/terms).
If you do not want this, choose a paid tier that does not use your data for training, or another service.

## Consent

Consent is given when you set up the translation service: directly above the "Roziman — saqlash va tekshirish"
(I agree — save and test) button, the welcome page and the settings page say that the lesson subtitles go to the
selected service and the Uzbek text goes to Microsoft for the voice or, if the browser has no Uzbek voice and the service is Gemini, to Google. The consent covers only the selected service:
if you switch to another one, it is asked again. If consent is missing (for example after switching the service
or when the list of recipients changes), the panel shows a short prompt with a "Roziman" (I agree) button; until
you press it, nothing is sent. The full list (recipients, what stays on the device, the Gemini notice) is in the
"Maxfiylik" (Privacy) section of the settings page. The consent (version, service and date) is stored on this
device. You can withdraw it at any time: Settings → "Maxfiylik" → "Rozilikni qaytarib olish" (Withdraw consent).
After that no lesson text is sent anywhere, and translation and voice stop at once in open lessons.

## What is stored on your device

In the browser's extension storage (`chrome.storage.local`), in this browser profile only. Nothing is synced to
other devices.

- **API keys** (translation service, Azure) — in the extension's background part. Neither the web page nor the
  extension's script on the page can read them.
- **Settings** — selected service and model, voice engine and selected voice, Azure region, the panel mode
  (Off / Subtitles / Voice) and subtitle display options, the consent record.
- **Dictionaries** — the terms and pronunciations you wrote, and term pronunciations learned from the translation
  service.
- **Translation cache** — per lesson: the lesson identifier (on sites you enabled, the page address) and title, the
  English subtitle text, the Uzbek translation, timings and which model translated it. The cache means you do not
  pay the service again when you reopen that lesson.
- **Voice audio cache** — in the extension's IndexedDB: the audio synthesised by Azure or the Gemini voice, so a
  replay does not send the sentences again.
- **Diagnostics log** — the code of the last 50 errors (for example `auth`, `timeout`), the kind of work
  (translation, subtitles, voice, model list), time, duration and count. Subtitle text, translations and keys are
  never written to it. The log is never sent anywhere by itself: Settings → "Diagnostikani nusxalash" (Copy
  diagnostics) copies it together with the extension version, browser name, service and model name and voice
  status, and you decide whom to send it to.
- **Model speed** — for each of the last 20 service and model pairs: the average number of output tokens per second,
  the number of measurements and the time of the last one. No text is stored. It is included in "Copy diagnostics"
  (without the time) and is never sent anywhere by itself.

Temporarily (`chrome.storage.session`, cleared when the browser closes): the address, type and requesting page of
subtitle files requested by the lesson page and of requests that help locate the subtitle address (for example
master.dev lesson data) — at most 50 per tab. A tab's entries are deleted when the tab closes. The extension stores
no other requests and never blocks or modifies any request.

## How to delete it

- **Translation cache:** Settings → "Kutubxona" (Library) → a lesson's delete button (one lesson) or
  "Hammasini o'chirish" (Delete all).
- **Translation service key:** Settings → "Tarjima" (Translation) → "API key" → "O'chirish" (Delete).
- **Everything** (including the Azure key, dictionaries, learned pronunciations and consent): remove the extension
  from the browser — the browser deletes all of its local data as well.
- Data held by the services is deleted according to that service's policy.

## No selling, no transfer

Sado does not sell data, does not use it for advertising and does not give it to anyone other than the services
named above that you chose. Data is used only for the extension's single purpose — translating and voicing
subtitles. Sado complies with the Chrome Web Store User Data Policy, including the Limited Use requirements.

## Children

Sado is not directed at children under 13. Using the Gemini API requires being 18 or older.

## Changes

If this policy changes, this document is updated. If the list of recipients changes, the extension asks for
consent again before the first request to a new recipient.

## Contact

[namazbaevshakhzod@gmail.com](mailto:namazbaevshakhzod@gmail.com)
