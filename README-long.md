# My Projects

## [guardian Framework](https://github.com/comroid-git/guardian-framework)
#### The guardian Framework aims at enabling a developer to easily create REST-Based APIs, Wrappers for those APIs and even contains a simple module to integrate a Web UI with said API.

## [KScr](https://github.com/comroid-git/KScr)
#### A simple interpreted language, attempting to grow into a fully-fledged compiled OOP language some day.

## [CrystalShard](https://github.com/comroid-git/CrystalShard)
#### CrystalShard is a Java-Wrapper for the Discord Bot API

CrystalShard is a Wrapper for the Discord Bot API, that one can use to connect with a [discord bot account](https://discordapp.com/developers/applications/).
Such accounts can be used for al sorts of things, mostly for chatbots within the Discord platform.
A chatbot can do whatever you can imagine, in the boundaries of the platform.

##### Required Skills:
- Designing a wrapper based on documentation
- Designing a powerful and modular API
- REST-API
- Ratelimiting REST-Requests based on responses
- WebSockets
- Caching and active updating for cached entities
- JSON knowledge
- RegEx knowledge

##### Example:
[CandyBot](https://github.com/comroid-git/CandyBot) - A Discord bot for levelling

CandyBot counts all messages in a Discord guild. Once the counter reaches 100, the author of that 100th message receives one "level".


## [VBAN-API](https://github.com/comroid-git/VBAN-API)
#### Java wrapper for the VB-Audio VBAN protocol

Used by the virtual audio mixing console [VoiceMeeter](https://www.vb-audio.com/Voicemeeter/banana.htm).
The VBAN Protocol is used to send audiostreams over network from one VoiceMeeter instance to another, and to be able to remotecontrol VoiceMeeter instances.
In [VoiceMeeter 3 - Potato](https://www.vb-audio.com/Voicemeeter/potato.htm), it can also be used to cue MIDI actions.

##### Required Skills:
- Designing a wrapper based on documentation
- Bitwise operations
- Designing a fast and reliable API
- UDP Communication
- Designing a fast bytearray modification tool


## [VBANDeck](https://github.com/burdoto/VBANDeck) (archived)
#### VBAN-Plugin for the Elgato StreamDeck

VBANDeck was requested and supported by Vincent Burel, the publisher of VoiceMeeter and the VBAN protocol.
VBANDeck requires porting the Java VBAN wrapper to C#, as the Elgato StreamDeck API cannot run Java programs.

##### Required Skills:
- [Porting the VBAN-API to C#](https://github.com/burdoto/VBAN-API-CS)
- Designing an user friendly interface
- (Managing device and button data)
- (JavaScript Websocket communication)
- (C# Websocket communication)

Bracketed Skills have been taken care of by [BarRaider](https://github.com/BarRaider/streamdeck-tools).


## [discordbotlist-stats](https://github.com/burdoto/discordbotlist-stats) (archived)
#### Java cross-library solution for sharing Discord-bot stats on bot lists

Motivation for `discordbotlist-stats` was the presence of a high number of Discord Bot lists, where people can find a chatbot for the Discord platform based on their likings.
This artifact semi-automatically takes care of all communication involved when publishing bot statistics on such pages, such as the server count, or shard count.
This artifact comes in four different variants:
- The core artifact -> Holds all computing, manages all requests
- Three implementation artifacts (Javacord, Discord4J and JDA) to allow for automatic fetching of stats
Usually, the end user will depend on their implementation artifact based on which library they use, and that will also import the core artifact.

`discordbotlist-stats` is unique in its property to automatically manage data and requests for multiple discord bot lists.

##### Required Skills:
- Designing a unique wrapper based on several documentations
- Gradle project setup and publication management
- REST-API
- Creating an interface to keep code duplication between implementation and core artifacts to a minimum
- Creating an user-friendly way of adding credentials for new pages on-the-go


## [DiscordEmoji-API](https://github.com/burdoto/DiscordEmoji-API) (archived)
#### Java wrapper for the discordemoji.com API

discordemoji.com is a shared library for Emojis that server administration can add to their servers.
This implementation allows bots, that are written in Java, to communicate with its API to gather emojis.

##### Required Skills:
- REST-API
- Designing a simple and powerful API based on weak provided WebAPI and no documentation
- Designing a fast caching system
- Designing a fast JSON deserialization system for potentially tens of thousands of objects to be deserialized. Current throughput is `1.184ms` for `~5.4 thousand` emoji objects
