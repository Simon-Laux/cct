# Comparison of the different Messengers

> DISCLAIMER: This document is not done its a Work in Progress


Inspired by https://gitlab.com/edu4rdshl/blog/ (accessed jan 2019 - before he deleted most of his telegram article)

- Feel free to add messengers that aren't yet on this list via pr.
- Discuss things in the issues section
- Bold claims should be backed by evidence / sources.
- If you find something that is wrong, please open an Issue.

## Table of Content

1. [Telegram](#telegram)
1. [WhatsApp](#whatsapp)
1. [Delta.Chat](#delta.chat)

Note: This isn't a ranking - the order doesn't matter


## Telegram

### Why you should use it

- Network Effect (more than 200 million active users in March, 2018 [ℹ️](https://telegram.org/blog/200-million))
- Ad-free
- Cloud Messaging / multi device
- Telegram promises to give no data to authorities [ℹ️](https://telegram.org/privacy#8-3-law-enforcement-authorities)
- Contact people with user-name -> you don't need to give them your phonenumber [ℹ️](https://telegram.org/faq#q-who-can-i-write-to)
- Group-members see only your user-name, not your phone number
- $300K bounty to the person that cracks their MTProto Security [ℹ️](https://telegram.org/faq#q-what-if-my-hacker-friend-says-they-could-decipher-telegram-mes)
- Self-destructing Messages in Secret chats
- Client is open source and anybody can create their own Client ([but the sourcecode of the official one is not always updated immediately](https://gitlab.com/edu4rdshl/blog/issues/2#note_129234369))

#### Cloud Messaging
Cloud Messaging is one of Telegrams big advantages against other Messengers, because it allows true multi-device usage.
Unlike as for WhatsAppWeb you don't also need a phone connected to the Internet for using it.


### Cons

- Cloud Messaging (attacker has message history) -> enable 2FA
- bound to Mobile number
- E2E Encryption only in Secret Chats
- Centralized (although they have many servers in different countries they are still all controlled by telegram)

#### E2E encryption only in Secret Chats
[ℹ️](https://telegram.org/faq#q-why-not-just-make-all-chats-secret)

### What you should do to make it more secure/private

- Enable 2FA to prevent SMS account hijacking
- Use Secret-chats for important 1 on 1 chats
- Disable Contact Synchronization
- (optional) Disable "last Online"
- (optional) Disable Read-notefications

## WhatsApp

### Why you should use it
- Network Effect (Currently it's the biggest mobile Messenger) 
- Ad-free ([But there are rumors about ads coming soon](https://eu.usatoday.com/story/tech/talkingtech/2018/11/01/whatsapp-ads-reportedly-coming-its-status-stories/1844577002/))
- E2E Encryption in all Chats

### Cons
- bound to Mobile number
- collects Metadata [ℹ️](https://fossbytes.com/whatsapp-chats-collect-data-metadata/)
- belongs to Facebook
- requires you to upload your Contacts (practically unusable without it)
- Shares your phonenumber with every Groupmember
- Centralized
- Closed Source (which means back-doors are easier to hide, if they would push any with an update)


#### requires you to upload your Contacts
If you don't allow WhatsApp to upload your contacts by denying or removing the 'access contacts' permission, following things get disabled:

- Creating Groups
- Creating Broadcasts
- Chatpartner names are only numbers (because whatsapp uses the name from the phones contact list)
- Starting an chat with a specific Contact (only possible with third party apps or whatsapp-phone-number-links)

That way the app becomes pretty much **unuseable**.

### What you should do to make it more secure/private

- (optional) Disable "last Online"
- (optional) Disable Read-notefications

## Delta.Chat

### Why you should use it

- Ad-free
- Network Effect **nearly everybody** (everybody that has an Email account)
- Chat over Email
- Decentralized
- Your Chat partner does not need delta.chat to chat with you - a
- Full E2E Encryption over Autocrypt
- Multi device usage Support
- No Mobile number needed
- Fully Open-source

### Cons

- Isn't out yet

### What you should do to make it more secure/private

- Use Encryption -> talk to your chat partners about also using delta.chat or an other Autocrypt compatible Email Client
- (optional) Disable Read-notefications


## Direct Feature Comparison


Feature | Telegram | WhatsApp | Delta.Chat
--------|----------|----------|-----------
Clients availible* | Android, iOS, Windows, Mac, Linux, Web | Android, iOS, Nokia | Anroid, iOS, MacOS, Linux
Decentrelized | -  | -        | ✅
Max Group size| 200 upgradeable to 100K | 256 | 50 recommended: ✉️
Delete Messages (also on recipient) | ✅ | ✅ | -
Edit Messages | ✅  | -       | -
Stickers | ✅       | ✅       | -
Pin messages | 1 message | -  | -
File sharing | up to. 1,5 GB each | 100 mb | ✉️
Pin Chats to top | ✅      | ✅       | -
Archive Chats | -   | ✅      | ✅
Voice Calls | ✅    | ✅       | -
Video Calls | -    | ✅        | -
Read Notifications | ✅ | ✅   | ✅ when chat partner uses delta.chat
Encryption | E2E | MTProto (E2E only in SecretChats) | E2E when recipient has autocrypt or delta.chat, otherwise TLS

✉️ depends on your email provider

*Full clients that don't need an online phone