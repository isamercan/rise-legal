---
permalink: /privacy/
title: Rise — Privacy Policy
---

# Privacy Policy — Rise

**Effective date:** April 28, 2026
**Owner:** İsa Mercan ("we", "us", "Rise")

---

## 1. What we collect and why

Rise is an alarm app that wakes you up via short voice conversations with an AI coach. We collect the minimum data required to deliver that experience.

| Data | Why we need it | Where it's stored | Retention |
|---|---|---|---|
| Alarm settings (time, repeat days, persona, label) | To ring your alarm at the right time | On your device only (SwiftData) | Until you delete the alarm or the app |
| Onboarding answers (name, goal, morning style) | To personalize the AI greeting and persona suggestion | On your device only | Until you delete the app |
| Voice recordings (during the wake-up conversation) | To transcribe what you said and route it to the AI | Sent to **Apple Speech** (on-device or Apple-hosted) and **ElevenLabs** (via Fal.ai) for TTS playback. Audio is **not stored** by us | In-flight only — discarded as soon as the conversation ends |
| Conversation transcripts | To generate AI responses | Sent to **Anthropic** (Claude API) for response generation; stored on your device for the streak/insights views | On your device until you delete the wake-up session |
| Subscription state (entitlement, expiration) | To unlock premium features and gate paywall | **RevenueCat** anonymized device ID | While your subscription is active + 12 months |
| Crash logs and basic analytics | To find bugs and measure paywall conversion | **Firebase Analytics**, **Apple App Store Connect** (anonymized) | 14 months |

We do **not** collect: precise location, contacts, photos, browsing history, or biometrics.

## 2. Third-party processors (sub-processors)

The app sends data to the following services to function:

- **Anthropic, PBC** (Claude API) — receives your conversation transcript to generate AI responses. Anthropic's privacy policy: [https://www.anthropic.com/privacy](https://www.anthropic.com/privacy)
- **Fal.ai** — proxy for ElevenLabs TTS synthesis. Privacy policy: [https://fal.ai/legal/privacy-policy](https://fal.ai/legal/privacy-policy)
- **ElevenLabs Inc.** — receives the AI text response (downstream of Fal.ai) to synthesize voice playback. ElevenLabs' privacy policy: [https://elevenlabs.io/privacy](https://elevenlabs.io/privacy)
- **Apple Inc.** — Speech recognition framework, push notifications, App Store Connect analytics
- **RevenueCat, Inc.** — subscription state management. [https://www.revenuecat.com/privacy](https://www.revenuecat.com/privacy)
- **Google LLC (Firebase Analytics, Firebase Auth, Firebase App Check)** — anonymized usage analytics, anonymous session authentication for the AI proxy, and abuse protection. [https://firebase.google.com/support/privacy](https://firebase.google.com/support/privacy)

We do not sell your data. We do not share data with advertisers.

## 3. What we do NOT store

- Voice audio files — they are processed in-flight and discarded
- Authentication credentials — Rise has no login. Anonymous Firebase Auth issues a per-install identifier used only to authenticate proxy calls; no email or personal account is created
- Anything that identifies you across devices — RevenueCat uses an anonymized device ID

## 4. Your rights

- **Delete everything**: uninstall the app. All on-device data is removed.
- **Export your data**: not currently supported in v1.0 — email support@rise-app.com to request.
- **GDPR, CCPA, PIPEDA, LGPD, KVKK**: residents of those jurisdictions can request access, correction, or erasure by emailing support@rise-app.com. We respond within 30 days.

## 5. Children

Rise is rated 4+ but is not directed at children under 13. We do not knowingly collect data from children. If you believe a child has provided data, email support@rise-app.com and we will delete it.

## 6. Security

- Data in transit uses TLS 1.2+
- API keys for Anthropic and ElevenLabs are stored server-side in Firebase Cloud Functions Secret Manager and are not present in the iOS app binary
- Each proxy call is authenticated with a per-install Firebase Auth ID token; abuse is mitigated by Firebase App Check (App Attest) attestation

## 7. Changes

We may update this policy. The "effective date" above will reflect the latest revision. Material changes will be flagged in a what's new modal in-app.

## 8. Contact

support@rise-app.com

İsa Mercan
İstanbul, Türkiye
