---
layout: default
title: Privacy Policy
---

# Privacy Policy — QuestHold AI

**Last updated:** October 4, 2026

**Provider:** Goodhope Technologies LLC ("we", "us"), United States. Email: **support@goodhopetech.com**. Our business address and phone number are shown on QuestHold's Google Play listing.

---

## In short

- QuestHold has no accounts and no servers of its own. We do not collect your personal information, and nothing you type or say is sent to us.
- The AI Game Master runs on your phone. Your campaigns are stored only on your phone, encrypted.
- QuestHold uses the internet to download its AI models, and to open a link or an email when you choose to. Google Play also checks your purchase and, where the law requires it, your age group.
- If you play co-op with friends, the phones at the table talk to each other over your Wi-Fi or hotspot. That goes from phone to phone, never to us.
- No ads, no analytics, no tracking, no crash reports.

## 1. What stays on your phone

All of this is kept on your phone and is never sent to us:

- **Your campaigns:** worlds, heroes, characters, the story so far, every dice roll and the chronicle. They are kept in an encrypted database (SQLCipher, AES-256) whose key is held in Android's secure key store on this phone.
- **What you type and say:** your moves and anything else you write. In single-player, it never leaves the phone.
- **Your voice:** if you play by voice, your speech is turned into text on the phone. See section 3.
- **Pictures:** the pictures QuestHold paints are made on the phone, and a safety filter on the phone checks each one before it is shown.
- **Settings:** for example whether you roll your own dice, whether downloads wait for Wi-Fi, which version of the Terms you agreed to, which passages and pictures you reported, and your free-turn count.
- **Your age group from Google Play,** if Google Play gives one (section 6).
- **The AI model files** the app downloaded.
- **A short error log** kept by Android on the phone, with personal details removed. It is never sent anywhere.

## 2. When QuestHold uses the internet

### The model download

Nothing downloads until you agree. Then QuestHold fetches only the models your phone can run, from these places:

- **Story model** (Gemma 4 E2B by Google): from Hugging Face, huggingface.co/unsloth/gemma-4-E2B-it-GGUF.
- **Memory model** (EmbeddingGemma by Google): from Hugging Face, huggingface.co/yyiimmiiyy/embeddinggemma-300m-mirror (our copy of the files Google publishes as litert-community/embeddinggemma-300m).
- **Voices and speech recognition** (Kokoro by hexgrad, its pronunciation lists, Moonshine by Useful Sensors and Silero VAD): from Hugging Face (huggingface.co/onnx-community/Kokoro-82M-v1.0-ONNX, huggingface.co/PeterReid/graphemes_to_phonemes_en_us, huggingface.co/moonshine-ai/moonshine) and GitHub (github.com/hexgrad/misaki, github.com/k2-fsa/sherpa-onnx for the Silero VAD file).
- **Picture safety filter:** from Hugging Face, huggingface.co/onnx-community/nsfw_image_detection-ONNX.
- **Art models, on phones that paint pictures on the processor** (Stable Diffusion 1.5, LCM-LoRA and TAESD): from Hugging Face (huggingface.co/second-state/stable-diffusion-v1-5-GGUF, huggingface.co/latent-consistency/lcm-lora-sdv1-5, huggingface.co/madebyollin/taesd).
- **Art models for phones with an AI chip:** delivered by Google Play.

Like any download, these requests show Hugging Face, GitHub, Google Play and the content-delivery networks they use your IP address, the file being fetched and basic details of the app making the request. QuestHold sends no name, account, identifier or game data with them. Their own privacy policies apply: [Hugging Face](https://huggingface.co/privacy), [GitHub](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement), [Google](https://policies.google.com/privacy).

While the download runs, Android shows a notification so it can carry on when you leave the app. If Android stops a long download, QuestHold carries on with it the next time you open the app.

### Models shared with our other apps

If another Goodhope Technologies app on your phone already holds the same model file, QuestHold can use that copy instead of downloading it again. The file is checked by size and fingerprint first. QuestHold offers its own checked model files to those apps in the same way. Only model files are ever shared between the apps, never your campaigns or anything you typed.

### Links you open

Opening the Terms or this Privacy Policy on the web opens your browser at yyiimmiiyy.github.io (GitHub Pages). Both are also readable inside the app with no connection.

### Reports you choose to email

You can report a passage the Game Master wrote (press and hold it) or a picture QuestHold painted (press and hold it). The report is made on your phone and the passage or picture is hidden at once. QuestHold then offers to open your email app with a report already written. It contains:

- the reason you picked and any details you typed;
- for a passage, the passage itself; for a picture, a short description of what it was meant to show and its file name (the picture itself is not attached);
- the app version and the time of the report.

Nothing is sent unless you press send in your email app. Section 7 explains what happens to a report you send.

### Google Play and Pro

Installing, updating and buying Pro all happen through Google Play, under Google's privacy policy. We never see your card details; we only receive what Google Play gives every developer about an order. Your free-turn count and trial are counted on your phone and are not sent to us. If Google Play needs a parent to approve a purchase, Google Play asks them; QuestHold only learns that the purchase is waiting or approved.

## 3. Your voice and the AI voices

- **Speaking your moves:** if you choose to play by voice, Android asks you for the microphone first. QuestHold's own speech model (Moonshine) turns your speech into text on the phone, and the audio is not sent anywhere or kept. Until that model has downloaded, QuestHold uses your phone's built-in speech recognition and asks Android to keep it on the phone; that recognition is part of Android (usually provided by Google) and works under its own privacy terms. We never receive your audio.
- **The voices you hear** are made by AI on your phone (Kokoro), or by your phone's own text-to-speech before the voices have downloaded. They are not recordings of real people.

## 4. Smart dice (Bluetooth)

If you choose to connect a smart die (such as Pixels dice), QuestHold uses Bluetooth to find the die and read the number it rolls. Android asks you for the "Nearby devices" permission first. QuestHold does not use Bluetooth to find your location. The connection is between your phone and your die only; nothing about it is sent to us.

## 5. Co-op on the same Wi-Fi or hotspot

Co-op works without the internet and without our servers. The phone that hosts the game runs the story; friends' phones join it over the same Wi-Fi network or the host's phone hotspot.

- **While a table has a free seat,** the host's phone announces it on the local network every two seconds (UDP port 42021), so friends' phones can find it: a short table label the host chose (the host's hero's name unless they change it), how many seats are free, the port to connect to, and a random number for that table. Any device on the same network can see that announcement. It never carries the campaign's title, the story or anyone's moves.
- **To sit down,** a friend's phone connects to the host's phone (TCP port 42020) and sends the four-digit table code shown on the host, and a random secret key that QuestHold made on the friend's phone, so a returning friend gets their own hero back. Nothing else is accepted before the code is right, and wrong guesses are limited.
- **Once seated,** the friend's phone sends their hero (name, abilities and training), their moves (typed, or spoken and turned into text on their phone), the dice they roll, and their level-up choices. The host's phone sends each friend the story the Game Master tells, the heroes at the table and the scene, and asks them to roll when the game needs it.
- **Who receives it:** only the phones at that table, directly over your local network. None of it goes to us or over the internet.
- **How it travels:** as plain messages on your local network, not encrypted. Anyone else on the same network could see them if they tried, so play co-op on a network you trust, such as your home Wi-Fi or your own phone's hotspot, not public Wi-Fi.
- **What is kept:** the campaign, including each friend's hero and their secret key, is saved only on the host's phone, in its encrypted campaign database. A friend's phone keeps its own secret key and table settings.
- On newer Android versions, Android asks you before QuestHold may use the local network.

## 6. Age checks (Google Play Age Signals)

Some places, such as Texas, require app stores and apps to know whether a player is a minor and to get a parent's approval for some things. When you open QuestHold, and when you open the Pro screen, QuestHold asks Google Play's Age Signals service on the phone what it knows about the account: whether its age is shared, its age range (for example 13 to 15), and whether a parent manages it. Google Play may ask you first whether to share it. QuestHold keeps only that answer, on your phone, and uses it only to follow these laws:

- If a parent manages the account, buying Pro goes through Google Play's parental approval, and Pro opens when the parent approves.
- If Google Play says the account belongs to someone under 18 whom no parent manages in Google Play, Pro waits for a parent: they can buy it on their own account, or supervise yours and approve it.
- If the law where you live requires a verified age and Google Play does not have one yet, Pro waits until you confirm your age in Google Play.
- If Google Play says the account belongs to someone under 13, QuestHold cannot be played on it.

Free play is never held back by these checks, and if Google Play gives no answer, QuestHold works as normal. We never receive the answer and never use it for anything else.

## 7. Reports you email us: how we handle them

This section applies only if you send us an email (a report or a question). It is the only personal information we ever receive.

- **Who is responsible:** Goodhope Technologies LLC, at the address and email at the top of this policy.
- **What we receive:** your email address, your name if your email app includes it, and what the email says.
- **Why, and on what basis:** to read your report or question, fix what went wrong in QuestHold, and answer you. Under the EU and UK GDPR our legal basis is our legitimate interest in keeping QuestHold safe and working and in answering you (Article 6(1)(f)).
- **Who else sees it:** only the email service that delivers and stores our mail. We do not sell or share it with anyone else.
- **Where:** we are in the United States, so your email is received and stored there.
- **How long:** we delete a report email, and your address with it, within 12 months of the last message about it, or sooner if you ask.
- **Your rights:** you can ask us for a copy of what we hold about you, and ask us to correct it, delete it, limit how we use it or stop using it (object), and to give it to you in a portable form. Write to support@goodhopetech.com. If you are in the EU or UK and think we have not handled your data properly, you have the right to complain to your data protection authority (in the UK, the Information Commissioner's Office).
- You do not have to send a report. Reporting inside the app works without email.

## 8. Permissions

- **Internet and the local network:** the model download, links you open, and co-op on your Wi-Fi or hotspot.
- **Notifications, a foreground service and keeping the phone awake:** so the download shows its progress and keeps going when you leave the app.
- **Microphone:** only if you play by voice (section 3). Android asks first.
- **Nearby devices (Bluetooth):** only if you connect a smart die (section 4). Android asks first.

QuestHold does not ask for your location, contacts, camera or photos.

## 9. Children

QuestHold is for players aged 13 and over. It collects no personal information from anyone, of any age. If a child under 13 has emailed us, contact us and we will delete the email.

## 10. Keeping and deleting your data

- Your campaigns stay on your phone until you delete them. Uninstalling QuestHold, or clearing its storage in Android's settings, deletes them and everything else QuestHold stored. We cannot recover them.
- QuestHold does not let Android back up its files to your Google account. To keep a copy of a campaign, use "Back up and restore" in QuestHold's settings: the backup file is encrypted with a password you choose, and you decide where it goes.
- Report emails are kept as section 7 says.

## 11. Your rights

We do not sell or share personal information, and we hold none about you unless you emailed us. You can ask us what we hold, and ask us to correct or delete it, at the email address above.

## 12. Changes to this policy

If we change this policy, we update the date above. When a change matters, QuestHold asks you to agree again before you next play.

## 13. Contact

Questions about privacy: **support@goodhopetech.com**, or write to Goodhope Technologies LLC at the address at the top of this policy.
