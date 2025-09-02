# 📖 Word-by-Word Quran Translation API (Free, Open & Unlimited)

A **free, open, static API** for accessing the Quran word-by-word in **18 languages**.  
- ✅ No authentication required  
- ✅ No rate limiting  
- ✅ No CORS issues  
- ✅ Delivered via jsDelivr CDN (fast & reliable)  
- ✅ Beginner-friendly JSON format  

---

## 📂 API Endpoints

### 1. Surah in a Specific Language
https://cdn.jsdelivr.net/gh/Tawhid-200/word-by-word-quran-translation/api/surah/{surah_number}/language/{lang}.json


- `{surah_number}` → `1` to `114`  
- `{lang}` → one of the 18 language codes above  

✅ Example: Surah 1 (Al-Fatiha) in **Bengali**  
👉 [Click here](https://cdn.jsdelivr.net/gh/Tawhid-200/word-by-word-quran-translation/api/surah/1/language/bn.json)

✅ Example: Surah 1 (Al-Fatiha) in **English**  
👉 [Click here](https://cdn.jsdelivr.net/gh/Tawhid-200/word-by-word-quran-translation/api/surah/1/language/en.json)

---

### 2. List of Languages (Static Reference)

Check the full list of available languages here:

👉 [languages.json](https://cdn.jsdelivr.net/gh/Tawhid-200/word-by-word-quran-translation/api/surah/languages.json)

Example (`languages.json`):

{
  "bn": { "language": "Bengali", "original": "বাংলা", "code": "bn" },
  "de": { "language": "German", "original": "Deutsch", "code": "de" },
  "en": { "language": "English", "original": "English", "code": "en" },
}

## Currently supported:
bn, de, dv, en, en_trans, fa, fr, hi, in, inh, ml, ru, sd, sq, ta, tr, ur, zh

---
## 📦 Example JSON Response

Example: Surah 1 (Al-Fatiha) in **English (`en`)**

```json
[
  "In the name of Allah,",
  "the Entirely Merciful,",
  "the Especially Merciful.",
  "All praise is [due] to Allah,",
  "Lord of the worlds –",
  "The Entirely Merciful,",
  "the Especially Merciful,",
  "Sovereign of the Day of Recompense.",
  "It is You we worship and You we ask for help.",
  "Guide us to the straight path –",
  "The path of those upon whom You have bestowed favor,",
  "not of those who have evoked [Your] anger or of those who are astray."
] 
```
## ⚡ Usage Examples
### JavaScript (Browser / Node.js)

// Fetch Surah 1 (Al-Fatiha) in Bengali
async function getSurah(surah, lang) {
  const url = `https://cdn.jsdelivr.net/gh/Tawhid-200/word-by-word-quran-translation/api/surah/${surah}/language/${lang}.json`;
  const res = await fetch(url);
  const data = await res.json();
  console.log(data);
}

getSurah(1, "bn");

## 🚀 Features

Extremely fast (served from global CDN)

Free forever, no signup needed

Perfect for Islamic apps, Quran learning tools, and research projects

## 🤝 Contributing

Fork this repo

Add improvements (translations, corrections, etc.)

Submit a Pull Request

## 📜 License

This dataset is provided freely for everyone.
Use it in your apps, projects, or research without restrictions.

