# Voice calls

Press the call button in any chat to talk to a bot. You speak, the bot answers by voice, and you can interrupt it at any time. Both sides are written on screen as you talk. Say "bye" or "hang up" to end the call.

## Gemini Live (recommended)

1. Get a free API key from [Google AI Studio](https://aistudio.google.com/apikey).
2. In Seva Bots open **Settings → API keys** and paste it into the Gemini field.
3. Start a call. The call screen shows **Live**.

The bot hears you through Gemini Live and usually starts answering in about a second. Punjabi (Gurmukhi) and English are both understood. When a question needs real work (files, Gurbani search, your memory, the web), the bot does that work with its normal tools and then tells you the result.

Your key stays on your computer. The app's own server talks to Google; the window never sees the key.

## Local voice (advanced, no key)

If the internet drops during a call, the call keeps going on the local voice server when it is running on `127.0.0.1:8833`, and returns to Gemini between turns when the connection is back. Without a Gemini key, calls use the local voice server directly. Answers are slower: about 3 to 4 seconds in English and around 10 seconds in Punjabi on an M1 Mac.

The local voice server is not included in the download yet. It uses Whisper for English, wav2vec2 for Punjabi, Kokoro for English speech and Meta MMS for Punjabi speech. MMS is licensed for non-commercial use only.

## OpenAI or Azure

If you already use an OpenAI key, calls keep using OpenAI GPT-Live. You can switch service in **Call settings**.
