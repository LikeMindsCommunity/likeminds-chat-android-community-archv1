# LikeMinds Chat SDK for Android

Drop-in chat for Android apps, in Kotlin. Group chatrooms, 1:1 DMs, polls, voice notes and
reactions, with offline sync.

[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)

**Docs:** https://docs.likeminds.io/

> **This is the shipping Android Chat SDK**, despite the `archv1` in the repo name. The SDK lives in
> the `chatmm` module. [likeminds-chat-android](https://github.com/LikeMindsCommunity/likeminds-chat-android)
> is an unused scaffold and is not what you want.

## What you get

Group chatrooms and 1:1 DMs with request, approve, reject, block and rate limits · emoji reactions ·
reply, edit, delete, multi-select · @-mentions · polls · voice notes · images, video, GIFs via Giphy,
PDFs and documents · link previews via Chrome Custom Tabs · chatroom topics · search across
chatrooms, conversations and members · explore chatrooms · secret chatrooms and invites · report and
moderation · push notifications · offline sync with a local database.

Beyond that: an in-app **image editor** with crop, freehand draw and text overlay, **video trimming**,
and **audio waveform** playback.

## Install

The UI SDK is consumed as a git submodule rather than a Maven artifact:

```groovy
// settings.gradle
include ':chatmm'
```

It depends on the data layer, which **is** published:

```groovy
implementation 'community.likeminds:likemindschat:2.13.0'
```

Source for the data layer is at
[likeminds-chat-android-data](https://github.com/LikeMindsCommunity/likeminds-chat-android-data).

## What is in this repo

| Directory | What it is |
|---|---|
| `chatmm/` | The SDK itself, roughly 510 Kotlin files |
| `community-chat/` | Group chatrooms only |
| `networking-chat/` | 1:1 DMs only |
| `community-hybrid-chat/` | Both in one app |
| `ai-chatbot/` | Chat against an AI bot participant |

## Three product shapes

Selected by theme: community for group chatrooms, networking for DMs, hybrid for both.

## Built on

ExoPlayer · Glide · Dagger · Firebase

## Contributing

See the org-wide [contributing guide](https://github.com/LikeMindsCommunity/.github/blob/main/.github/CONTRIBUTING.md).
Security issues go to **natesh@likeminds.community**, not the issue tracker.

## License

Apache 2.0. See [LICENSE](LICENSE).
