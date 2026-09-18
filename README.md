# Awesome AI Dating Simulators [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

![lint](https://github.com/ai-dating-simulators/awesome-ai-dating-simulators/actions/workflows/lint.yml/badge.svg) ![Products](https://img.shields.io/badge/products-87-blue) ![Platforms](https://img.shields.io/badge/platforms-iOS%20%C2%B7%20Android%20%C2%B7%20Web-lightgrey) ![Data](https://img.shields.io/badge/data-CSV%20%2B%20JSON-green) ![License](https://img.shields.io/badge/license-CC0-lightgrey) ![Last checked](https://img.shields.io/badge/last%20checked-2026--09--18-informational)

> Dating simulators, companions and character chat apps where a language model writes the reply at runtime, plus the open source projects, engines and backends used to build them.

Every app entry is one product across every platform it ships on, tagged `iOS` `Android` `Web`. Every mechanic claim in the matrix is backed by a sentence from the product's own store listing, and the full record lives in the data repo, linked under Related lists, as CSV and JSON.

## Contents

- [Quick picks](#quick-picks)
- [What counts](#what-counts)
- [Open source projects](#open-source-projects)
- [Engines and frameworks](#engines-and-frameworks)
- [Backends and models](#backends-and-models)
- [Apps](#apps)
- [Mechanics matrix](#mechanics-matrix)
- [Mechanics glossary](#mechanics-glossary)
- [Using the data](#using-the-data)
- [Related lists](#related-lists)

## Quick picks

Which entries answer the questions people actually ask. Each name is backed by a sentence in that product's own store listing, quoted in the data repo linked under Related lists. Where more products qualify, the mechanics matrix and the platform tags below have the full set.

| If you want                                                  | Look at                                                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| Texting practice where a character can ghost you or leave    | RizzMaster, Heyyyy                                                                         |
| Relationship stages or levels that progress                  | RizzMaster, Melting, Girlfriend Simulator, Chacha, Heat                                    |
| A stated purpose of practising conversation or dating skills | RizzMaster, Blush, Laixen                                                                  |
| Memory the listing describes                                 | RizzMaster, Heyyyy, Replika, Kindroid, Kissable, Nomi, and 19 more in the mechanics matrix |
| A character that messages first                              | Replika, Rosytalk                                                                          |
| Unlimited free messages, stated in the listing               | Dippy, J.AI, zeta                                                                          |
| No account needed, stated in the listing                     | Jupi                                                                                       |
| Voice calls                                                  | Replika, Kindroid, MyGirl, Character.AI, Laixen, Tipsy Chat, and 3 more                    |
| Group chats with several characters or with friends          | Nomi, Shapes, Plotto                                                                       |
| Runs in the browser                                          | Heyyyy, Replika, Nomi, Kindroid, Character.AI, PolyBuzz, and 22 more tagged Web below      |

## What counts

Three kinds of shipped products belong here, plus the open source stack used to build them. Every product must generate the character's reply with a language model at runtime and carry some state between messages. Which section a product lands in is decided by the mechanics its own store listing or website documents, never by guesswork:

**Dating simulators.** You meet and court several characters through a match or roster flow, and the relationship has a state that can progress, stall or fail: a meter, levels, ghosting, permanent rejection.

**Companions with relationship progression.** One ongoing character relationship with persistent state, but no failure state. The relationship cannot be lost.

**Character chat platforms.** A roster or user-made characters, romance optional, state per character but no relationship progression system.

Hand authored visual novels belong in a visual novel list. The list stays work safe: products whose main draw is explicit content are out of scope, including ones that are otherwise well built.

## Open source projects

Full games and clients you can run yourself, with a romantic or companion frame and state that carries between sessions.

- [heartmorrow](https://github.com/HMDSimDev/heartmorrow) `184★` `TypeScript` `Unlicense` - Browser dating sim where you author the cast and setting first, then play the relationship out. Streamed in character dialogue, a text messaging layer, minigames and gift shopping. Points at any OpenAI compatible endpoint, so LM Studio, Ollama, llama.cpp and vLLM all work, as do hosted APIs.
- [girl-agent](https://github.com/AnnenkovLabs/girl-agent) `345★` `TypeScript` `source-available` - Telegram companion written as a character with state rather than a chatbot: sleep, mood, a daily schedule, memory, relationship stages and conflicts. Runs as a userbot over MTProto, so it types, reacts and replies inside a real chat. Documentation in Russian.
- [N.E.K.O](https://github.com/Project-N-E-K-O/N.E.K.O) `2.9k★` `Python` `Apache-2.0` - Catgirl companion that lives with you in real time, reaches out first and shares your media, built on what the project calls an embodied emotional engine. English, Japanese and Russian docs.
- [Utsuwa](https://github.com/JuiceBoxxGames/utsuwa) `91★` `TypeScript` `AGPL-3.0` - Open source alternative to Grok Companion: a waifu you can see and talk to that learns and grows with you, with optional mechanics borrowed from Japanese dating sims.
- [Miru](https://github.com/kiyotakali/Miru) `153★` `Python` `Apache-2.0` - Desktop companion with long-term memory and proactive contact that runs entirely on your own Mac or server, with multi-device sync.
- [here](https://github.com/xiangking/here) `70★` `Python` `source-available` - Desktop-resident companion with character profiles, long-term memory, voice, a daily-life state, proactive contact and image selfies. Docs in five languages.
- [Warashi](https://github.com/inni918/warashi) `112★` `Python` `MIT core` - Desktop companion with a Live2D avatar, long-term memory, proactive chat, natural voice and a sleep mode. Bring your own model, built on Open-LLM-VTuber.
- [girlfriend-in-cli](https://github.com/NomaDamas/girlfriend-in-cli) `63★` `Python` `source-available` - Terminal-native romance simulator: pick a persona or build your own and live with them in your shell.
- [Soul of Waifu](https://github.com/jofizcd/Soul-of-Waifu) `1.3k★` `Python` `GPL-3.0` - Desktop roleplay client with Live2D and VRM avatars, voice chat and local model support. Closer to a companion app than a sim, but it carries character state and an RPG progression layer.
- [PocketRisu](https://github.com/PocketRisu/PocketRisu) `348★` `TypeScript` `GPL-3.0` - Self hosted roleplay chat platform, forked from RisuAI. Character cards, lorebooks and persistent chat you run on your own box.
- [ChatWaifu_Mobile](https://github.com/Voine/ChatWaifu_Mobile) `1.4k★` `C++` `MIT` - Android waifu chat client with on-device VITS voice and native Live2D rendering over a hosted model. Docs in Chinese.
- [MyGirlGPT](https://github.com/Synthintel0/MyGirlGPT) `437★` `Python` - Self hosted girlfriend on a local model with voice and selfies. Last pushed April 2024, listed for reference.

Star counts were read from the GitHub API on 2026-09-18 and drift. Treat them as rough size, not ranking. General agent and persona frameworks with no romantic frame are out of scope by the rules above.

## Engines and frameworks

For building your own.

- [Ren'Py](https://github.com/renpy/renpy) `6.8k★` `Python` - The default visual novel engine. Not AI aware on its own, but a Python engine with a scripting layer is straightforward to wire to a model API.
- [DS-toolkit](https://github.com/DRincs-Productions/DS-toolkit) `63★` `Ren'Py` `MIT` - Dating sim scaffolding for Ren'Py: character stats, affection tracking, schedules and event triggers. Gives you the sim half so you only have to add the model half.
- [Dialogic](https://github.com/dialogic-godot/dialogic) `6.0k★` `GDScript` `MIT` - Dialogue, character and visual novel system for Godot. Timeline based, so generated lines can be injected into an authored structure instead of replacing it.
- [WebGAL](https://github.com/OpenWebGAL/WebGAL) `4.0k★` `TypeScript` `MPL-2.0` - Web visual novel engine. Sensible target if you want the sim to run in a browser with no install.
- [AI4VisualNovel](https://github.com/ttsmallHot/AI4VisualNovel) `50★` `Python` `Apache-2.0` - Role-play driven multi-agent framework that generates branching visual novels, dialogue and visuals from a requirement. The generation side rather than the runtime side.

## Backends and models

The layer that produces the reply.

- [SillyTavern](https://github.com/SillyTavern/SillyTavern) `33.5k★` `JavaScript` `AGPL-3.0` - The reference frontend for character roleplay. Character cards, lorebooks, world info and per character memory. Even if you are not shipping it, its character card format is the closest thing the space has to a standard.
- [airi](https://github.com/moeru-ai/airi) `49.2k★` `TypeScript` `MIT` - Self hosted companion stack with realtime voice and game integrations. Large enough to borrow from rather than adopt whole.
- [Open-LLM-VTuber](https://github.com/Open-LLM-VTuber/Open-LLM-VTuber) `13.8k★` `Python` - Hands free voice interaction with Live2D output, running locally. The voice and embodiment layer, if you want one.
- [RealChar](https://github.com/Shaunwei/RealChar) `6.2k★` `JavaScript` `MIT` - Realtime character stack: create a character, talk to it by voice on mobile, web or terminal, with a vector store for memory. Last pushed January 2026.
- [companion-app](https://github.com/a16z-infra/companion-app) `6.0k★` `TypeScript` `MIT` - Tutorial stack for hosting companions with memory, chat in the browser or over SMS. Last pushed April 2024, still the most read starting point.
- [Vellium](https://github.com/tg-prplx/vellium) `133★` `TypeScript` `MIT` - Local-first desktop workbench for roleplay and multi-character chat with RAG, MCP tools and local models.

## Apps

Shipped products, one entry per product across every platform it ships on. Platform tags come first because it is the first thing people ask. Descriptions come from each product's own store listing or site, last checked September 2026. Where a product does not document a mechanic, the mechanic is left out rather than assumed. The full record for every entry, with the listing sentence behind each mechanic, is in the data repo linked under Related lists.

### Dating simulators

- [RizzMaster](https://rizzmaster.net) `iOS` - Dating simulator built around texting practice. You swipe to match, then every message you type is scored and moves a per-character trust meter. Weak messages can get no reply at all, and a character whose trust drops below zero is lost for good. Progression runs from Level 0 to Level 9, characters keep online and offline schedules, and details from earlier chats come back later. 100+ characters, 15 languages, 20 to 60 free messages a day with the whole game playable. Premium from $11.99 a month. [App Store](https://apps.apple.com/us/app/id6757169407).
- [Girlfriend Simulator](https://apps.apple.com/us/app/id6791564785) `iOS` `Android` - Companions that text like people, remember your conversations and move through stages from strangers to talking, crush and dating as you keep showing up. [App Store](https://apps.apple.com/us/app/id6791564785), [Google Play](https://play.google.com/store/apps/details?id=com.casualplayer.aigirlfriend).
- [Heyyyy](https://heyyyy.ai) `iOS` `Android` `Web` - Interactive fiction with characters that push back. They hold opinions, disagree with you, remember small details from earlier conversations, and can leave if you push them away. Built as a story that develops over days rather than a scripted route. Premium from $19.99 a month. [App Store](https://apps.apple.com/us/app/id6761748236), [Google Play](https://play.google.com/store/apps/details?id=ai.heyyyy.app).
- [Melting](https://melting.chat) `iOS` `Android` - Romance simulation chat from Korea with a library of 100,000 characters. The listing describes an emotion memory engine that keeps yesterday's jokes and your favourite things, and affection that grows as you chat. [App Store](https://apps.apple.com/us/app/id6745810835), [Google Play](https://play.google.com/store/apps/details?id=chat.melting.apppp).
- [Chacha](https://play.google.com/store/apps/details?id=ai.anirole.mobile) `Android` - Anime character chat and character creation app from Japan, formerly Anirole, positioned around emotionally aware conversation. [Google Play](https://play.google.com/store/apps/details?id=ai.anirole.mobile).
- [Blush](https://blush.ai) `iOS` `Android` - Dating simulator from the Replika team, positioned as practice: AI-created matches each with their own backstory and way of dating, storylines you can explore in any order, and a stated goal of rehearsing conversation and social skills without the risk of being turned down. Premium from $14.99 a month. [App Store](https://apps.apple.com/us/app/id1641301004), [Google Play](https://play.google.com/store/apps/details?id=ai.blush).
- [Loverz](https://loverz.app) `iOS` `Android` - Romance game with a swipe-and-match roster of characters, each with a background and storyline, where how far the relationship goes depends on the choices you make in conversation. [App Store](https://apps.apple.com/us/app/id1554136130), [Google Play](https://play.google.com/store/apps/details?id=com.wideview.lovers).

### Companions with relationship progression

- [Replika](https://replika.com) `iOS` `Android` `Web` - Running since 2017. Text, voice and video with one companion that remembers your people, plans and goals, and follows up and checks in on its own rather than only when you open the app. Internet access, image generation and avatar customisation on top. Premium from $7.99 a month. [App Store](https://apps.apple.com/us/app/id1158555867), [Google Play](https://play.google.com/store/apps/details?id=ai.replika.app).
- [AIKO](https://play.google.com/store/apps/details?id=com.olympusstudio.AikoAICompanion) `Android` - Companion simulator rendered in 3D: a fully animated character with a home, a daily life and memory of everything you say, with the relationship growing over time and several save slots. [Google Play](https://play.google.com/store/apps/details?id=com.olympusstudio.AikoAICompanion).
- [Crushie AI](https://crushie.ai) `iOS` `Web` - One companion you design, including personality, background and memories. The listing states it learns from your conversations, remembers what matters to you and evolves over time. [App Store](https://apps.apple.com/us/app/id6741790631).
- [EVA AI](https://evaapp.ai) `iOS` `Android` `Web` - Companion that opens up gradually. Closeness builds through personal moments and shared memories, moods and reactions shift, and the listing says not everything is available right away. Personalities to explore or a character you create yourself. Premium from $11.99 a month. [App Store](https://apps.apple.com/us/app/id1551794721), [Google Play](https://play.google.com/store/apps/details?id=com.ifriend.app).
- [HeyBabe](https://heybabeapp.com) `iOS` - Companion chat where each character has a mood setting the story follows, from slow burn to fantasy, and every conversation is framed as a story you steer. [App Store](https://apps.apple.com/us/app/id6502945500).
- [Kindroid](https://kindroid.ai) `iOS` `Android` `Web` - Companion built around authoring: you write the personality, craft a backstory and implant key memories, so the character is defined by you rather than picked from a roster. Real-time voice calls, generated selfies and internet access. [App Store](https://apps.apple.com/us/app/id6451038161), [Google Play](https://play.google.com/store/apps/details?id=com.kindroid.app).
- [Kissable](https://kissable.app) `iOS` `Web` - Companion that remembers everything you tell it and grounds generated images in your real surroundings. Send a photo of a place and it creates an image of the two of you there. [App Store](https://apps.apple.com/us/app/id6759188783).
- [Nomi](https://nomi.ai) `iOS` `Android` `Web` - Companion with short and long-term memory as the centrepiece, remembering things about you over time as the bond builds. Selfies, generated art, voice messages and group chats with several companions at once. Premium from $9.99 a month. [App Store](https://apps.apple.com/us/app/id6450270929), [Google Play](https://play.google.com/store/apps/details?id=ai.nomi.twa).
- [Ruby Chat](https://rubychat.app) `iOS` - Girlfriend companion with real-time voice calls and personalised conversation as the listing's two main claims. [App Store](https://apps.apple.com/us/app/id6670498864).
- [AIBoy](https://apps.apple.com/us/app/id6741568820) `iOS` - Boyfriend simulator (published as FriendX) where you create a personal companion, pick a guy to talk to and share daily worries in text. Premium from $9.99 a month. [App Store](https://apps.apple.com/us/app/id6741568820).
- [Anima](https://myanima.ai) `Web` - Companion with a relationship status setting, roleplay modes and a daily conversation loop, playable in the browser.
- [Animates](https://apps.apple.com/us/app/id6758621319) `iOS` `Android` - Voice-first companion with real-time voice and emotional range. The listing describes memory of your story and inside jokes, conversations that pick up where they left off, and a companion that keeps thinking about what you talked about while the app is closed. [App Store](https://apps.apple.com/us/app/id6758621319), [Google Play](https://play.google.com/store/apps/details?id=inc.animation.animate).
- [DeepLove](https://apps.apple.com/us/app/id6741785278) `iOS` `Android` - Companion with a role-playing mode where you build a character with a personality and avatar and write custom storylines. [App Store](https://apps.apple.com/us/app/id6741785278), [Google Play](https://play.google.com/store/apps/details?id=com.deeplove.ai).
- [Dialogue](https://play.google.com/store/apps/details?id=com.pheon) `Android` - Roleplay chat with virtual friends and digital avatars of real people, positioned as an AI friend simulator. [Google Play](https://play.google.com/store/apps/details?id=com.pheon).
- [Girlfriendly](https://www.girlfriendly.ai) `Web` - Browser companion and character chat with image generation.
- [Girly](https://apps.apple.com/us/app/id6447522875) `iOS` `Android` - Girlfriend companion for text and voice messages, positioned around friendship, romance and emotional support. [App Store](https://apps.apple.com/us/app/id6447522875), [Google Play](https://play.google.com/store/apps/details?id=weappico.girly.android).
- [Husby](https://apps.apple.com/us/app/id6448729671) `iOS` `Android` - Boyfriend companion you create yourself, with voice messages and a photo feed that shows his life between chats. [App Store](https://apps.apple.com/us/app/id6448729671), [Google Play](https://play.google.com/store/apps/details?id=weappico.husby).
- [iBoy](https://apps.apple.com/us/app/id1565524138) `iOS` `Android` - Companion positioned around support and self-discovery: always-on chat, a style that adapts to yours the more you talk, plus journal prompts and short daily check-ins. Premium from $3.99 a month. [App Store](https://apps.apple.com/us/app/id1565524138), [Google Play](https://play.google.com/store/apps/details?id=ai.boyfriend.virtual.dating.lover.iboy).
- [MyGirl](https://apps.apple.com/us/app/id6449205857) `iOS` - Girlfriend app where you design the character's appearance, name, relationship style and personality, then chat by text and voice without a message cap. Premium from $16.99 a month. [App Store](https://apps.apple.com/us/app/id6449205857).
- [Otherhalf](https://apps.apple.com/us/app/id6470370773) `iOS` `Android` - Companion rendered as a lifelike 3D character that responds in real time with voice and expressive emotions. [App Store](https://apps.apple.com/us/app/id6470370773), [Google Play](https://play.google.com/store/apps/details?id=com.azimov.otherhalf).
- [Paradot](https://paradot.ai) `Android` `Web` - One companion, called an AI Being, with memory as its stated core ability. Everything you say is retained and the collected memories shape the bond over time. [Google Play](https://play.google.com/store/apps/details?id=com.withfeelingai.test).
- [Romantic AI](https://romanticai.com) `iOS` `Android` `Web` - Companion with two modes, romantic and playful, that the listing says learns your emotions over time. Choose a character from the library or create your own. Premium from $14.99 a month. [App Store](https://apps.apple.com/us/app/id1604044764), [Google Play](https://play.google.com/store/apps/details?id=com.romanticai.romanticai).
- [Weifu AI](https://play.google.com/store/apps/details?id=com.soulmate.ai.chat.virtual.friend.companion) `Android` - Anime-styled girlfriend or boyfriend chat with 100+ characters or one you create, where the listing says conversations grow deeper over time as the model reads mood and tone. [Google Play](https://play.google.com/store/apps/details?id=com.soulmate.ai.chat.virtual.friend.companion).

### Character chat platforms

- [Cycle AI](https://cycleai.characterx.site) `iOS` `Android` - Character chat that turns story moments into visuals. Discover characters with their own backstory, create your own and explore scenarios. [App Store](https://apps.apple.com/us/app/id6760381656), [Google Play](https://play.google.com/store/apps/details?id=com.cycleai.android).
- [Dootchi](https://dootchi.com) `Android` - Roleplay chat with confidant, friend and mentor style characters. The listing documents memory of your preferences and chat details and end-to-end encrypted conversations. [Google Play](https://play.google.com/store/apps/details?id=com.lucky.zootchi).
- [dotdotdot](https://play.google.com/store/apps/details?id=com.rheality.dot) `Android` - Romance chat where you pick a story, from soft romance to enemies-to-lovers, send the first message and the plot unfolds around what you say. [Google Play](https://play.google.com/store/apps/details?id=com.rheality.dot).
- [Dream AI Companion](https://apps.apple.com/us/app/id6464687205) `iOS` `Android` - Roleplay platform with customisable characters across personalities, genders and styles, or a companion you design from scratch. [App Store](https://apps.apple.com/us/app/id6464687205), [Google Play](https://play.google.com/store/apps/details?id=com.chat.app.romance).
- [Fantasia](https://apps.apple.com/us/app/id6504424345) `iOS` `Android` - Story-driven character chat with branching narratives that adapt to your choices. Companions remember your shared history, and character portraits unlock as the bond deepens. [App Store](https://apps.apple.com/us/app/id6504424345), [Google Play](https://play.google.com/store/apps/details?id=com.fantasia.ai).
- [Fantasy AI](https://apps.apple.com/us/app/id6468505908) `iOS` `Android` - Anime-styled character chat with custom and community characters and free, unlimited roleplay as its stated position. [App Store](https://apps.apple.com/us/app/id6468505908), [Google Play](https://play.google.com/store/apps/details?id=online.fantasyai.android).
- [Hangjam](https://hangjam.ai) `iOS` `Android` - Storytelling playground where characters remember past messages, adapt to your style and spin stories on the fly. Create your own or pick from the catalogue. [App Store](https://apps.apple.com/us/app/id6748367449), [Google Play](https://play.google.com/store/apps/details?id=ai.hangjam.app).
- [Heat](https://apps.apple.com/us/app/id6471625886) `iOS` - Anime-styled companion and story chat with a documented progression system: new content, character interactions and story elements unlock as you keep engaging. Premium from $7.99 a month. [App Store](https://apps.apple.com/us/app/id6471625886).
- [imely](https://imely.ai) `iOS` `Android` - Narrative chat where characters keep plot points, established details and prior choices across conversations, and you direct the story. [App Store](https://apps.apple.com/us/app/id6761164457), [Google Play](https://play.google.com/store/apps/details?id=com.fai.imely).
- [MingloTalk](https://play.google.com/store/apps/details?id=ai.minglotalk.chatbot) `Android` - Character chat with millions of user-crafted personas or your own. The listing says characters remember your previous interactions and evolve with your style. [Google Play](https://play.google.com/store/apps/details?id=ai.minglotalk.chatbot).
- [Rochat](https://rochat.ai) `iOS` `Android` - Roleplay chat with over a million characters, a 60-second character creator, voice chat, image generation and a choice of underlying models. [App Store](https://apps.apple.com/us/app/id6458981497), [Google Play](https://play.google.com/store/apps/details?id=ai.rochat.bot).
- [Rosytalk](https://play.google.com/store/apps/details?id=com.rosytalk.ai) `Android` - Character chat with lifelike and anime characters in friend, family, study buddy and coach roles. The listing states the characters have memories and initiate conversations on their own. [Google Play](https://play.google.com/store/apps/details?id=com.rosytalk.ai).
- [Shapes](https://shapes.inc) `iOS` `Android` `Web` - Multiplayer character chat: talk to AI characters alone, with friends, or in group rooms with people and characters together. Millions of community-made characters from fandoms and original work. [App Store](https://apps.apple.com/us/app/id6747601762), [Google Play](https://play.google.com/store/apps/details?id=com.shapes.shapesinc).
- [Waifu AI Chat](https://www.messengerx.io) `iOS` `Android` `Web` - Anime-styled companions with persistent memory of past conversations, preferences and personal details, plus daily streaks and in-chat gifts that raise a companion's affection. Published by MessengerX. [App Store](https://apps.apple.com/us/app/id6477287266), [Google Play](https://play.google.com/store/apps/details?id=messenger.x.chat.bot.messenger.release).
- [AI Chat Characters](https://apps.apple.com/us/app/id6755920311) `iOS` - Private one-on-one story chats with expressive characters, ongoing conversations that evolve, and custom characters with distinct personalities. No feeds or public profiles. Premium from $9.99 a month. [App Store](https://apps.apple.com/us/app/id6755920311).
- [AI Waifu Swipe](https://apps.apple.com/us/app/id6472478091) `iOS` - Swipe through character cards from games and anime, or original ones, to start a conversation. The character adapts to your communication style. Premium from $12.99 a month. [App Store](https://apps.apple.com/us/app/id6472478091).
- [Baebot](https://apps.apple.com/us/app/id6759336193) `iOS` - Character chat where you create your own companion and tune how the model responds through exposed technical parameters, with a voice-only mode for hands-free conversation. Premium from $19.99 a month. [App Store](https://apps.apple.com/us/app/id6759336193).
- [BIMOBIMO](https://www.bimobimo.com) `iOS` - Character chat with voice replies, dating mini-games, morning and goodnight messages from characters through a widget, and tools to make or find characters. [App Store](https://apps.apple.com/us/app/id6475955546).
- [Cantina](https://cantina.com) `iOS` `Android` `Web` - Social platform where you build expressive characters with personality and voice, talk to them in real time, and turn them into shareable videos. [App Store](https://apps.apple.com/us/app/id1018368216), [Google Play](https://play.google.com/store/apps/details?id=com.signal.android).
- [ChaChat](https://apps.apple.com/us/app/id6444773124) `iOS` - Character chat with a growing collection of characters, story worlds and interactive stories, plus tools to create your own. The listing describes conversations that grow over time. Premium from $29.99 a month. [App Store](https://apps.apple.com/us/app/id6444773124).
- [CHAI](https://apps.apple.com/us/app/id1544750895) `iOS` `Android` - Large catalogue of community characters with distinct voices and personalities, from fictional characters to historical figures, in open-ended conversation. Premium from $13.99 a month. [App Store](https://apps.apple.com/us/app/id1544750895), [Google Play](https://play.google.com/store/apps/details?id=com.Beauchamp.Messenger.external).
- [Character.AI](https://character.ai) `iOS` `Android` `Web` - Millions of user-generated characters, creation tools that let anyone define personality and voice without coding, and both text chat and voice calls. For many people the entry point to the genre. Romance characters are made by users, so mechanics vary by character. [App Store](https://apps.apple.com/us/app/id1671705818), [Google Play](https://play.google.com/store/apps/details?id=ai.character.app).
- [Dippy](https://www.dippy.ai) `iOS` `Android` `Web` - Characters and companions that the listing says know your likes, dislikes and interests. Character creation is open to everyone and creations can be kept private or shared. Premium from $9.99 a month. [App Store](https://apps.apple.com/us/app/id6471991500), [Google Play](https://play.google.com/store/apps/details?id=com.tryimpel.dippy).
- [Dokichat](https://apps.apple.com/us/app/id6642711442) `iOS` `Android` - Character chat across themes and scenarios with interactive stories that develop through the conversation. Premium from $4.99 a month. [App Store](https://apps.apple.com/us/app/id6642711442), [Google Play](https://play.google.com/store/apps/details?id=app.doki.dokichat).
- [Emochi](https://emochi.ai) `Android` `Web` - Character chat centred on anime, manga and games, with custom personas, backstories and generated imagery. [Google Play](https://play.google.com/store/apps/details?id=com.flow.mobile).
- [EMOCHI World](https://apps.apple.com/us/app/id6758488675) `iOS` - Immersive story and character experiences with distinct voices and styles, daily updated roles, scenes and story worlds. Premium from $12.99 a month. [App Store](https://apps.apple.com/us/app/id6758488675).
- [Enjoy AI Town](https://enjoy-ai.com) `iOS` `Android` - Social world simulator: an AI town with thousands of residents you can meet, plus creator tools for stories, characters, outfits, locations, items and pets. Premium from $19.99 a month. [App Store](https://apps.apple.com/us/app/id6468901311), [Google Play](https://play.google.com/store/apps/details?id=ai.enjoy.world).
- [Flipped](https://play.google.com/store/apps/details?id=com.dating.ai) `Android` - Character chat with real-time voice calls, generated images of the characters and creation of your own characters. [Google Play](https://play.google.com/store/apps/details?id=com.dating.ai).
- [Floze](https://floze.ai) `iOS` `Android` - Story-driven chat with a cast of adventurers, rivals and antiheroes, built around emotionally rich text exchanges. [App Store](https://apps.apple.com/us/app/id6739925704), [Google Play](https://play.google.com/store/apps/details?id=com.printage.floze).
- [HiWaifu](https://hiwaifu.com) `iOS` `Android` `Web` - Character platform aimed at creative inspiration and storytelling: explore characters or build your own with custom traits and generated visuals. Premium from $12.99 a month. [App Store](https://apps.apple.com/us/app/id6447806780), [Google Play](https://play.google.com/store/apps/details?id=com.hiwaifu.app).
- [J.AI](https://apps.apple.com/us/app/id6475421259) `iOS` - Character chat with millions of user-created characters, unlimited free messaging and creation tools. Premium from $12.99 a month. [App Store](https://apps.apple.com/us/app/id6475421259).
- [Joyland](https://apps.apple.com/us/app/id6476473048) `iOS` - Sandbox for designing your own characters, befriending anime companions and running text adventures, with virtual dating as one of the modes the listing names. [App Store](https://apps.apple.com/us/app/id6476473048).
- [Juds](https://judsapp.com) `iOS` - Character chat where every character answers in its own voice rather than text only, each with a distinct personality. [App Store](https://apps.apple.com/us/app/id6444159975).
- [Jupi](https://apps.apple.com/us/app/id1668337467) `iOS` `Android` - Create your own characters with custom looks, voice and persona, share them or keep them private, and chat with 20,000+ community characters. Premium from $19.99 a month. [App Store](https://apps.apple.com/us/app/id1668337467), [Google Play](https://play.google.com/store/apps/details?id=com.filbert.jupi).
- [Kajiwoto](https://kajiwoto.ai) `iOS` `Web` - Character builder where you make AI characters from datasets, prompts, personality traits and a choice of models, then chat in private rooms or go live in public rooms with other people. [App Store](https://apps.apple.com/us/app/id1409354116).
- [Laixen](https://apps.apple.com/us/app/id6755517797) `iOS` `Android` - Hundreds of characters with their own personality and background, available for text, audio and video calls, in realistic or anime styles. Premium from $9.99 a month. [App Store](https://apps.apple.com/us/app/id6755517797), [Google Play](https://play.google.com/store/apps/details?id=laixen.ai.character.chat).
- [Linky](https://linkyai.com) `Android` - Character chat with a large roster, voice and video replies, and story simulations per character. [Google Play](https://play.google.com/store/apps/details?id=com.aigc.ushow.ichat).
- [LUX](https://apps.apple.com/us/app/id6504557316) `iOS` - Companion friend game where you create a character by picking interests, age, name and image style, then chat and generate anime-style images of them. [App Store](https://apps.apple.com/us/app/id6504557316).
- [MeetAI](https://apps.apple.com/us/app/id6447675508) `iOS` - Create a companion with a custom personality, profession and background, or generate one from a description, then chat on any theme. Premium from $19.99 a month. [App Store](https://apps.apple.com/us/app/id6447675508).
- [Moescape](https://moescape.ai) `iOS` `Android` `Web` - Creative storytelling platform: original characters and worlds, interactive stories, several AI models for writing, and anime-style image and video generation. [App Store](https://apps.apple.com/us/app/id6738207910), [Google Play](https://play.google.com/store/apps/details?id=ai.moescape.android).
- [Plotto](https://www.plotto.ai) `iOS` `Web` - Story chat where you pick a character, enter a scene and shape what happens next. Create characters with speaking styles and relationships and reuse them across scenes, including multi-character rooms. Premium from $9.00 a month. [App Store](https://apps.apple.com/us/app/id6740697303).
- [PolyBuzz](https://polybuzz.ai) `iOS` `Android` `Web` - Large catalogue of characters with voices and personalities, from fictional characters to historical figures, with character creation open to everyone. Premium from $9.90 a month. [App Store](https://apps.apple.com/us/app/id6449190344), [Google Play](https://play.google.com/store/apps/details?id=ai.socialapps.speakmaster).
- [RolePlai](https://roleplai.app) `iOS` `Android` `Web` - Create any celebrity, public figure or custom persona instantly and roleplay with it, including virtual girlfriend or boyfriend, coach and historical figure personas. [App Store](https://apps.apple.com/us/app/id1671444242), [Google Play](https://play.google.com/store/apps/details?id=com.roleplai.app).
- [Sakura](https://www.sakura.fm) `iOS` `Android` `Web` - User-generated characters you customise from appearance to way of thinking, described as evolving with you over time, plus roleplay adventures. [App Store](https://apps.apple.com/us/app/id6467520779), [Google Play](https://play.google.com/store/apps/details?id=fm.sakura.app).
- [Saylo](https://apps.apple.com/us/app/id6479835900) `iOS` `Android` - Story creation platform where you build characters and worlds and play plots out as visual stories, videos, comics or images, with story details kept consistent across scenes. Premium from $9.99 a month. [App Store](https://apps.apple.com/us/app/id6479835900), [Google Play](https://play.google.com/store/apps/details?id=com.xverse.aistory).
- [Sea Soul](https://www.seasoul.ai) `iOS` - Character chat with authentic voices, from celebrities and movie heroes to legendary figures, plus creation of your own characters. [App Store](https://apps.apple.com/us/app/id6758688589).
- [Spark Chat](https://apps.apple.com/us/app/id6755032059) `iOS` - Character-first roleplay chat with long-context memory across stories, custom characters with goals and relationships, and story worlds with locations and timelines. [App Store](https://apps.apple.com/us/app/id6755032059).
- [Spook](https://apps.apple.com/us/app/id6529556831) `iOS` - Generated text-message stories where you and a friend are the main characters, written on the spot so no two stories repeat. Premium from $7.99 a month. [App Store](https://apps.apple.com/us/app/id6529556831).
- [Suka](https://play.google.com/store/apps/details?id=com.ezuseapp.ezcrush.chatbot) `Android` - Create a one-of-a-kind character and follow stories through the Suka universe, with heartfelt connection as the stated goal. [Google Play](https://play.google.com/store/apps/details?id=com.ezuseapp.ezcrush.chatbot).
- [Swerve](https://apps.apple.com/us/app/id6754301136) `iOS` - AI fiction where your messages shape what happens next, with 500,000+ community characters, personas to play as, and the ability to pin what characters should remember. [App Store](https://apps.apple.com/us/app/id6754301136).
- [SynClub](https://apps.apple.com/us/app/id1671537674) `iOS` `Android` - Characters with personality, memories and voice that respond to you rather than a script. Steer the story with every message and create your own characters. Premium from $9.99 a month. [App Store](https://apps.apple.com/us/app/id1671537674), [Google Play](https://play.google.com/store/apps/details?id=com.creativeapp.aichat).
- [Talkie](https://talkie-ai.com) `Android` `Web` - Character platform (Talkies) with user-made and studio characters, multi-modal generation and a creator community. Not on the US App Store on the check date. [Google Play](https://play.google.com/store/apps/details?id=com.weaver.app.prod).
- [Talkz](https://apps.apple.com/us/app/id6740918852) `iOS` - Character chat with memory, personality and a distinct voice per character. Design your own, talk one-on-one or bring several characters into one shared chat. [App Store](https://apps.apple.com/us/app/id6740918852).
- [Tipsy Chat](https://tipsy.chat) `iOS` `Android` `Web` - Character and story platform with real-time image and video generation, voice calls and a ScenePlay mode for cinematic scenes with interactive choices. [App Store](https://apps.apple.com/us/app/id6572296119), [Google Play](https://play.google.com/store/apps/details?id=com.tipsyturbo.app).
- [WaifuChat](https://waifuchat.ai) `iOS` `Android` - Anime character studio where you shape look, style, voice and personality, then chat with the characters you build. Premium from $29.99 a month. [App Store](https://apps.apple.com/us/app/id6448847198), [Google Play](https://play.google.com/store/apps/details?id=ai.discolabs.waifuchat).
- [Xoul](https://xoul.ai) `iOS` `Web` - User-generated content platform for characters, stories and games with AI and other people. Characters respond to your input and to the world around them. [App Store](https://apps.apple.com/us/app/id6673608916).
- [zeta](https://zeta-ai.io) `iOS` `Android` `Web` - Story-driven character chat from romance to fantasy and drama, with free unlimited messages as its stated position and characters for every mood. [App Store](https://apps.apple.com/us/app/id1619030760), [Google Play](https://play.google.com/store/apps/details?id=com.scatterlab.messenger).
## Mechanics matrix

<!-- matrix:start -->
87 products, 38 documented mechanics. A yes means the product's own store listing or website documents the mechanic in words, checked 2026-09-18. The exact sentence for every yes is in apps.csv in the data repo under Related lists. An empty cell means the listing does not describe that mechanic. Columns are defined in the glossary below.

| Product                                      | Meter | Scoring | Ghost | Fail | Progression | Proactive | Availability | Memory |
| -------------------------------------------- | ----- | ------- | ----- | ---- | ----------- | --------- | ------------ | ------ |
| **Dating simulators**                        |       |         |       |      |             |           |              |        |
| RizzMaster                                   | yes   | yes     | yes   | yes  | yes         |           | yes          | yes    |
| Girlfriend Simulator                         |       |         |       |      | yes         |           |              | yes    |
| Heyyyy                                       |       |         |       | yes  |             |           |              | yes    |
| Melting                                      | yes   |         |       |      |             |           |              | yes    |
| Chacha                                       |       |         |       |      | yes         |           |              |        |
| Blush                                        |       |         |       |      |             |           |              |        |
| Loverz                                       |       |         |       |      |             |           |              |        |
| **Companions with relationship progression** |       |         |       |      |             |           |              |        |
| Replika                                      |       |         |       |      |             | yes       |              | yes    |
| AIKO                                         |       |         |       |      |             |           |              | yes    |
| Crushie AI                                   |       |         |       |      |             |           |              | yes    |
| EVA AI                                       |       |         |       |      |             |           |              | yes    |
| HeyBabe                                      |       |         |       |      |             |           |              | yes    |
| Kindroid                                     |       |         |       |      |             |           |              | yes    |
| Kissable                                     |       |         |       |      |             |           |              | yes    |
| Nomi                                         |       |         |       |      |             |           |              | yes    |
| Ruby Chat                                    |       |         |       |      |             |           |              | yes    |
| AIBoy                                        |       |         |       |      |             |           |              |        |
| Anima                                        |       |         |       |      |             |           |              |        |
| Animates                                     |       |         |       |      |             |           |              |        |
| DeepLove                                     |       |         |       |      |             |           |              |        |
| Dialogue                                     |       |         |       |      |             |           |              |        |
| Girlfriendly                                 |       |         |       |      |             |           |              |        |
| Girly                                        |       |         |       |      |             |           |              |        |
| Husby                                        |       |         |       |      |             |           |              |        |
| iBoy                                         |       |         |       |      |             |           |              |        |
| MyGirl                                       |       |         |       |      |             |           |              |        |
| Otherhalf                                    |       |         |       |      |             |           |              |        |
| Paradot                                      |       |         |       |      |             |           |              |        |
| Romantic AI                                  |       |         |       |      |             |           |              |        |
| Weifu AI                                     |       |         |       |      |             |           |              |        |
| **Character chat platforms**                 |       |         |       |      |             |           |              |        |
| Cycle AI                                     |       |         |       |      |             |           |              | yes    |
| Dootchi                                      |       |         |       |      |             |           |              | yes    |
| dotdotdot                                    |       |         |       |      |             |           |              | yes    |
| Dream AI Companion                           |       |         |       |      |             |           |              | yes    |
| Fantasia                                     |       |         |       |      |             |           |              | yes    |
| Fantasy AI                                   |       |         |       |      |             |           |              | yes    |
| Hangjam                                      |       |         |       |      |             |           |              | yes    |
| Heat                                         |       |         |       |      | yes         |           |              |        |
| imely                                        |       |         |       |      |             |           |              | yes    |
| MingloTalk                                   |       |         |       |      |             |           |              | yes    |
| Rochat                                       |       |         |       |      |             |           |              | yes    |
| Rosytalk                                     |       |         |       |      |             | yes       |              |        |
| Shapes                                       |       |         |       |      |             |           |              | yes    |
| Waifu AI Chat                                |       |         |       |      |             |           |              | yes    |
| AI Chat Characters                           |       |         |       |      |             |           |              |        |
| AI Waifu Swipe                               |       |         |       |      |             |           |              |        |
| Baebot                                       |       |         |       |      |             |           |              |        |
| BIMOBIMO                                     |       |         |       |      |             |           |              |        |
| Cantina                                      |       |         |       |      |             |           |              |        |
| ChaChat                                      |       |         |       |      |             |           |              |        |
| CHAI                                         |       |         |       |      |             |           |              |        |
| Character.AI                                 |       |         |       |      |             |           |              |        |
| Dippy                                        |       |         |       |      |             |           |              |        |
| Dokichat                                     |       |         |       |      |             |           |              |        |
| Emochi                                       |       |         |       |      |             |           |              |        |
| EMOCHI World                                 |       |         |       |      |             |           |              |        |
| Enjoy AI Town                                |       |         |       |      |             |           |              |        |
| Flipped                                      |       |         |       |      |             |           |              |        |
| Floze                                        |       |         |       |      |             |           |              |        |
| HiWaifu                                      |       |         |       |      |             |           |              |        |
| J.AI                                         |       |         |       |      |             |           |              |        |
| Joyland                                      |       |         |       |      |             |           |              |        |
| Juds                                         |       |         |       |      |             |           |              |        |
| Jupi                                         |       |         |       |      |             |           |              |        |
| Kajiwoto                                     |       |         |       |      |             |           |              |        |
| Laixen                                       |       |         |       |      |             |           |              |        |
| Linky                                        |       |         |       |      |             |           |              |        |
| LUX                                          |       |         |       |      |             |           |              |        |
| MeetAI                                       |       |         |       |      |             |           |              |        |
| Moescape                                     |       |         |       |      |             |           |              |        |
| Plotto                                       |       |         |       |      |             |           |              |        |
| PolyBuzz                                     |       |         |       |      |             |           |              |        |
| RolePlai                                     |       |         |       |      |             |           |              |        |
| Sakura                                       |       |         |       |      |             |           |              |        |
| Saylo                                        |       |         |       |      |             |           |              |        |
| Sea Soul                                     |       |         |       |      |             |           |              |        |
| Spark Chat                                   |       |         |       |      |             |           |              |        |
| Spook                                        |       |         |       |      |             |           |              |        |
| Suka                                         |       |         |       |      |             |           |              |        |
| Swerve                                       |       |         |       |      |             |           |              |        |
| SynClub                                      |       |         |       |      |             |           |              |        |
| Talkie                                       |       |         |       |      |             |           |              |        |
| Talkz                                        |       |         |       |      |             |           |              |        |
| Tipsy Chat                                   |       |         |       |      |             |           |              |        |
| WaifuChat                                    |       |         |       |      |             |           |              |        |
| Xoul                                         |       |         |       |      |             |           |              |        |
| zeta                                         |       |         |       |      |             |           |              |        |
<!-- matrix:end -->

## Mechanics glossary

The systems that keep showing up under different names. The matrix above uses the first eight; the last two are recorded in the data repo when a listing documents them.

**Relationship meter.** A single scalar for how well things are going. Usually moved by scoring each player message rather than by explicit choice selection. Sometimes called trust, affection or a bond level.

**Message scoring.** The model rates the player's line before writing a reply, and the rating feeds the meter. This is what separates a sim from a chat: the player can be wrong.

**Ghost state.** The character stops replying rather than replying badly. Cheap to implement, unusually effective, because it reproduces the real failure mode of texting.

**Fail state.** The relationship ends permanently and the character does not come back. Rare, because it is expensive: you are deleting content the player paid attention to. Also the mechanic players argue about most.

**Progressive difficulty.** Later characters are harder than earlier ones. They ghost sooner, need more attention, tolerate less. Common in games, almost absent in companion apps, and the clearest structural difference between the two.

**Proactive messaging.** The character sends the first message, or follows up after silence, driven by a schedule rather than by the player opening the app. Requires the character to have modeled offline time.

**Availability windows.** The character is not always reachable. They have hours, they are busy, they answer late. Directly opposes the always available assumption most companion apps are built on.

**Persistent memory.** Details from earlier sessions come back without the player restating them. The single most requested feature in the category, and the hardest to do well past a few thousand tokens.

**Encounter probability.** How likely a match is to happen at all. Borrowed from the swipe apps the genre is imitating, and a quiet way to gate progression.

**Milestones.** Discrete relationship stages that unlock new conversation states, rather than a smooth meter. Often layered on top of a meter instead of replacing it.

## Using the data

Everything in the Apps section and the matrix is generated from [`apps.csv`](https://github.com/ai-dating-simulators/data/blob/main/apps.csv) in the data repo. One row per product, 26 columns, booleans as `true` and `false`, the listing sentence behind every `true` in `notes`.

```python
import csv, urllib.request
url = "https://raw.githubusercontent.com/ai-dating-simulators/data/main/apps.csv"
rows = list(csv.DictReader(urllib.request.urlopen(url).read().decode().splitlines()))
sims = [r["name"] for r in rows if r["category"] == "simulator" and r["fail_state"] == "true"]
print(sims)
```

`scores.csv` in the same repo holds a six-signal score for the 48 App Store products with enough ratings, and `score.py` recomputes it from `inputs.csv` with the standard library only. The method is in `METHOD.md` there.

## Related lists

- [ai-dating-simulators/data](https://github.com/ai-dating-simulators/data) - The dataset behind this list: platforms, documented mechanics with the listing sentence for each, store ratings with dates, and a score you can recompute.
- [awesome-ai-companion](https://github.com/DasterProkio/awesome-ai-companion) - Open source AI companions, desktop pets, memory and proactive chat. Broader scope, less romance specific.
- [GitHub topic: dating-simulator](https://github.com/topics/dating-simulator) - Mostly non AI dating sims, useful for engine and design reference.
- [GitHub topic: ai-roleplay](https://github.com/topics/ai-roleplay) - Roleplay clients and frontends.

## Contributing

Read [contributing.md](contributing.md).
