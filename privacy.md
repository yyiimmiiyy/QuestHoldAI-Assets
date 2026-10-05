---
layout: default
title: Privacy Policy
---

# Privacy Policy — QuestHold AI

**Last updated:** October 3, 2026

**Provider:** Goodhope Technologies LLC ("we", "us")

---

## In short

- QuestHold has no accounts and no servers of its own. We do not collect your personal information.
- The AI Game Master runs entirely on your phone. Nothing you type or say leaves the phone.
- Your campaigns are stored only on your phone, encrypted.
- QuestHold uses the internet only to download its AI models, and to open a link or an email when you choose to.
- No ads, no analytics, no tracking, no crash reports.

## 1. What stays on your phone

All of this is kept on your phone and is never sent to us or anyone else:

- **Your campaigns:** worlds, heroes, characters, the story so far, every dice roll and the chronicle. They are kept in an encrypted database (SQLCipher, AES-256) whose key is held in Android's secure key store on this phone.
- **What you type and say:** your moves and anything else you write. If you play by voice, your speech is turned into text on the phone by a speech model; the audio is not sent anywhere.
- **Pictures:** portraits and scenes are painted on the phone, and a safety filter on the phone checks each one before it is shown.
- **Settings:** for example whether you roll your own dice, whether downloads wait for Wi-Fi, which version of the Terms you agreed to, which passages you reported, and your free-turn count.
- **The AI model files** the app downloaded.
- **A short error log** kept by Android on the phone, with personal details removed. It is never sent anywhere.

## 2. When QuestHold uses the internet

### The model download

Nothing downloads until you agree. Then QuestHold fetches only the models your phone can run, from these places:

- **Story model** (Gemma 4 E2B by Google): from Hugging Face, huggingface.co/unsloth/gemma-4-E2B-it-GGUF.
- **Memory model** (EmbeddingGemma by Google): from Hugging Face, huggingface.co/yyiimmiiyy/embeddinggemma-300m-mirror (our copy of the files Google publishes as litert-community/embeddinggemma-300m).
- **Voices and speech recognition** (Kokoro by hexgrad, its pronunciation lists, Moonshine by Useful Sensors and Silero VAD): from Hugging Face (huggingface.co/onnx-community/Kokoro-82M-v1.0-ONNX, huggingface.co/PeterReid/graphemes_to_phonemes_en_us, huggingface.co/moonshine-ai/moonshine) and GitHub (github.com/hexgrad/misaki, github.com/k2-fsa/sherpa-onnx for the Silero VAD file).
- **Picture safety filter:** from Hugging Face, huggingface.co/onnx-community/nsfw_image_detection-ONNX.
- **Art models, on phones that paint pictures on the processor** (Stable Diffusion 1.5, LCM-LoRA and TAESD): from Hugging Face.
- **Art models for phones with an AI chip:** delivered by Google Play.

Like any download, these requests show Hugging Face, GitHub, Google Play and the content-delivery networks they use your IP address, the file being fetched and basic details of the app making the request. QuestHold sends no name, account, identifier or game data with them. Their own privacy policies apply: [Hugging Face](https://huggingface.co/privacy), [GitHub](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement), [Google](https://policies.google.com/privacy).

While the download runs, Android shows a notification so it can carry on when you leave the app.

### Models shared with our other apps

If another Goodhope Technologies app on your phone already holds the same model file, QuestHold can use that copy instead of downloading it again. The file is checked by size and fingerprint first. QuestHold offers its own checked model files to those apps in the same way. Only model files are ever shared between the apps, never your campaigns or anything you typed.

### Links you open

Opening the Terms or this Privacy Policy on the web opens your browser at yyiimmiiyy.github.io (GitHub Pages). Both are also readable inside the app with no connection.

### Reports you choose to email

When you press and hold a passage to report it, the report is made on your phone and the passage is hidden. QuestHold then offers to open your email app with a report already written. It contains:

- the reason you picked and any details you typed;
- the reported passage;
- the app version and the time of the report.

Nothing is sent unless you press send in your email app. If you send it, we receive the email and your email address. We use reports only to fix and improve QuestHold, and we delete a report and your address when you ask.

### Google Play and Pro

Installing, updating and buying Pro all happen through Google Play, under Google's privacy policy. We never see your card details; we only receive what Google Play gives every developer about an order. Your free-turn count and trial are counted on your phone and are not sent to us.

## 3. Permissions

QuestHold uses the internet (for the download), notifications and a foreground service (so the download shows its progress and keeps going), and can keep the screen on while you play. It does not ask for your location, contacts, camera or photos. If you choose to play by voice, Android asks you for the microphone first.

## 4. Children

QuestHold is for players aged 13 and over. It collects no personal information from anyone, of any age. If a child under 13 has emailed us, contact us and we will delete the email.

## 5. Keeping and deleting your data

- Your campaigns stay on your phone until you delete them. Uninstalling QuestHold, or clearing its storage in Android's settings, deletes them and everything else QuestHold stored. We cannot recover them.
- If your phone backs up apps to your Google account, Android may include QuestHold's files in that backup under Google's terms. Your campaign database is encrypted with a key that stays in this phone's secure key store, so a backup copy cannot be read.
- Report emails are kept only as long as we need them, and deleted when you ask.

## 6. Your rights

We do not sell or share personal information, and we hold none about you unless you emailed us. You can ask us what we hold, and ask us to correct or delete it, at the address below.

## 7. Changes to this policy

If we change this policy, we update the date above. When a change matters, QuestHold asks you to agree again before you next play.

## 8. Contact

Questions about privacy: **support@goodhopetech.com**
