# Hablemos - Spanish speaking tutor (iPhone PWA)

Roleplay conversations in Mexican / Colombian / Central American Spanish with
pronunciation scoring (Azure), sentence corrections + natural rephrasing (Claude),
and native-voice replies.

## One-time setup (~10 min)
1. **Azure Speech (free F0 tier)**: portal.azure.com -> Create resource -> "Speech service"
   -> Pricing tier **Free F0**, region **East US**. Open it -> Keys and Endpoint -> copy KEY 1 and the region.
   Free tier: 5 audio hrs/month recognition + 0.5M chars/month voice. Plenty for daily practice.
2. **Claude API key**: console.anthropic.com -> API Keys -> create. Add ~$5 credit; a 15-min session is a few cents.
3. Host these files over HTTPS (needed for the mic on iPhone). Easiest: a GitHub Pages repo.
4. On iPhone, open the URL in Safari -> Share -> **Add to Home Screen**.
5. First launch opens Settings: paste both keys + region -> **Test keys**.

Keys live only in the phone's browser storage, never in the code/repo.

## Using it
- Pick a scenario (or Custom), level, tutor accent/voice/speed -> Start.
- Tap mic, speak, tap again. Words are underlined green / yellow / red; tap one to hear it.
- Feedback card: scores, corrected sentence, "more natural" version, pronunciation tips (each with play).
- 💡 = suggested next line. ⌨︎ = type instead. **Review** = end-of-session summary + phrases to keep.

## Note on accents
Azure's pronunciation grader supports es-MX (and es-ES) only, so your speech is always graded
against Mexican Spanish. The tutor's voice, vocabulary and slang follow whichever country you pick.
