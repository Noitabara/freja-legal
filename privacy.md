---
title: Privacy Policy
permalink: /privacy/
---

# Privacy Policy for Freja

**Effective date:** 25 August 2026
**Last updated:** 25 August 2026

Freja ("the bot", "we", "us") is a Discord moderation bot operated by Noitabara
for a Valheim community server. This policy explains what data the bot collects,
why, who it is shared with, how long it is kept, and how you can get a copy of
it or have it deleted.

By using a Discord server where Freja is present, you acknowledge the practices
described here.

**Contact for all privacy requests: me@noita.dev**

---

## 1. Summary

- We store **Discord user IDs, usernames, role IDs, and moderation records**
  (warnings, staff notes, mutes) in a private database.
- We **do not store message content.** Edited and deleted messages are relayed
  to a staff-only channel inside the same server and are never written to our
  database.
- We **do not sell your data**, do not use it for advertising, and do not use it
  to train machine learning models.
- You can **request a copy of your data or have it deleted** at any time — see
  section 7.

---

## 2. What we collect and store

| Data | Purpose |
|---|---|
| Discord user ID and username | Identifies who a moderation record belongs to and makes it readable for staff |
| Roles held when you leave the server | Restores your roles if you rejoin, and prevents mute evasion by leaving and returning |
| Number of times your record has been looked up | Signals to staff that a member has been reviewed repeatedly |
| Warnings and staff notes — the reason text written by a moderator, which moderator wrote it, and when | Maintains a moderation history so staff can act consistently and proportionately |
| Mutes — reason, who applied it, expiry, and if lifted early, by whom and why | Enforces and automatically expires temporary mutes |
| Operational event log — event type, acting and affected user IDs, server and channel IDs, success or failure, timing | Diagnoses failures and monitors the bot's reliability |

Reason and note text is **written by moderators**, not collected from your
messages. It may describe your conduct.

---

## 3. What we deliberately do not store

- **Message content.** Freja never writes message text to its database.
- Email addresses, real names, phone numbers, IP addresses, or payment
  information.
- Voice data, direct messages between users, or anything from servers where
  Freja is not present.
- Presence, status, or activity data — Freja does not use the Presence Intent.

---

## 4. Privileged Gateway Intents

**Server Members Intent.** Used solely to receive member join and leave events.
When you leave, we save the moderation-relevant roles you held. When you rejoin,
we restore them and re-apply any mute still in force. Without this, a muted
member could clear their punishment by leaving and rejoining. We do not download
or store full member lists and do not use member data for analytics.

**Message Content Intent.** Used solely for a staff audit log of edited and
deleted messages. When a message is edited or deleted, we forward the text to a
private staff channel in the same server so moderators can review context. Freja
has no handler for new messages and no prefix commands. Message content is never
written to our database, never sent to a third party, and never used to train
models.

---

## 5. Who your data is shared with

We do not sell, rent, or trade personal data. It is processed by:

| Provider | Role |
|---|---|
| Discord, Inc. | The platform Freja runs on. Data relayed to staff channels stays inside your Discord server and is subject to [Discord's Privacy Policy](https://discord.com/privacy). |
| Railway Corporation | Hosts the bot and its PostgreSQL database on Google Cloud Platform infrastructure, under a Data Processing Addendum. Databases are encrypted at rest. |

Moderators and administrators of the Discord server can see the moderation
records we hold about members of that server. That is the bot's purpose. We may
also disclose data where required by law.

---

## 6. How long we keep it

| Data | Retention |
|---|---|
| Moderation records — warnings, notes, mutes, saved roles | Kept for as long as Freja operates in the server. Moderation history stays relevant to staff decisions over time, including for members who leave and return. |
| Operational event log | Deleted after 12 months. |
| Application logs | Short-lived; rotate with the hosting platform. |

Any statistics we keep beyond these periods are aggregated and contain no user
identifiers.

---

## 7. Your rights, and how to use them

You may ask us to give you a copy of your data, correct it, delete it, or
restrict how we use it. Two ways to ask:

- **In Discord** — run `/data-request`. This is the preferred route, because
  Discord confirms your identity for us.
- **By email** — write to **me@noita.dev** with your Discord user ID. Use this
  if you have left the server and can no longer use the command. We may ask you
  for information to confirm you are the person the data is about.

Either way we respond within 30 days. Repeated or excessive requests may be
refused or rate-limited.

If you are in the EU or UK, these rights arise under the GDPR and UK GDPR, and
you may complain to your local data protection authority.

---

## 8. What happens when you ask us to delete your data

**We honour deletion requests.** We erase your record from our database —
warnings, notes, mutes, saved roles, and event log entries. The only data we
would keep is anything a law requires us to keep.

Two things to know:

- **If a sanction against you is active**, we will apply its outcome before
  erasing the record, because we cannot enforce a sanction once the record is
  gone. Membership of a moderated community depends on our being able to
  moderate it; the Terms of Service set out this condition and it applies to
  everyone equally.
- **We keep a minimal record that a deletion happened** — a one-way
  cryptographic hash of your user ID, the date, and which tables were cleared.
  This lets us prove we honoured your request without keeping anything that
  identifies you.

---

## 9. What we give you when you ask for a copy

You receive the contents of our database that relate to you, as a JSON file:
your member record, your warnings and notes, your mutes, and your event log
entries grouped by type with a summary count.

**We redact the identity of the moderator** who wrote each entry, and the
identity of any other member named in it. Data protection rights do not extend
to information identifying other people, and naming staff would expose them to
retaliation.

Some things are outside our control and are not ours to give you. Messages in
Discord threads, and the posts our bot sends to staff channels, are stored by
Discord, not by us — the bot never reads them back. If you want your Discord
messages, request them from Discord directly.

---

## 10. Legal basis

Where the GDPR or UK GDPR applies, we process personal data on the basis of
**legitimate interests** — operating and moderating a safe online community. We
process the minimum needed for that purpose. You may object at any time using
the contacts above.

---

## 11. Children

Discord requires all users to be at least 13, or older where local law sets a
higher age. Freja is not directed at children below that age. If you believe a
child's data has been collected, contact us and we will delete it.

---

## 12. Security

Data is held in a private PostgreSQL database with access restricted to the bot
operator. Our hosting provider encrypts databases at rest and connections are
encrypted in transit. Credentials are held in environment variables and are not
committed to source control. No system is perfectly secure, but we take
reasonable measures to protect what we hold.

---

## 13. International transfers

The bot and its database are hosted in the United States. If you use Freja from
elsewhere, your data is transferred to and processed there, under the safeguards
in our processor's Data Processing Addendum.

---

## 14. Changes

We may update this policy as the bot changes. The "Last updated" date will
change, and significant changes will be announced in the Discord server.

---

## 15. Contact

**me@noita.dev**
