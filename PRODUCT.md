# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Single self-contained HTML page published as a claude.ai artifact (no build step). Uses the artifact runtime capabilities: `db` (shared realtime store), `user`, `sample` (image recognition), `dictation`. No GPS, no direct camera API (file input with `capture` instead), no external fetch.

## Users

- **Field technician (persona: Péter, 42, 15 years on the job).** Works outdoors at 5–7 sites a day, under time pressure, often one-handed and sometimes in gloves, in sun, rain or basements without signal. Dislikes typing long text. Job: report a fault found on site (damaged gas pipe, missing seal, fallen line, meter issue) quickly and get it to the right team.
- **On-call colleague / dispatcher.** Receives reports live, needs at a glance: what happened, where, how urgent, what to do. Accepts with an ETA, messages, closes.
- **Demo audience:** the E.ON × Corvinus UX/UI Design Day jury. Sees the demo projected (team operating it) and then tries it on their own phones.

## Product Purpose

The "Gyors hibajelentés" (quick fault report) feature of the E.ON field-technician app. It turns a fault found on site into a structured, correctly routed report in about a minute with zero typing, and gives the reporter live confirmation of who saw it and who is coming. Success: faster recognition and faster, unambiguous communication between technicians.

## Positioning

Photo-first guided reporting: the photo drives a type suggestion, severity is computed from 2–3 factual yes/no safety questions rather than chosen, recipient is routed automatically, and the reporter sees a live status timeline. Works offline with an automatic send queue.

## Operating Context

- Flow: Hibát találtam → fotó → azonosítás (AI-javaslat + csempék) → súlyosság (igen/nem kérdések) → ellenőrzés és küldés (cím a munkalapról, diktálás, gyorscímkék) → élő státusz.
- Colleague side: live inbox sorted by severity → case card (mi, hol, mennyire sürgős, mit kell tenni checklist) → elvállalom (ETA) → megoldva.
- Severity levels: KRITIKUS, SÜRGŐS, NORMÁL. Categories: gázvezeték, plomba, oszlop/vezeték, mérőhely, egyéb.
- UI language: Hungarian.

## Capabilities and Constraints

- Must keep every existing function: role switch, offline simulation toggle, demo photo, AI suggestion, dictation, tags, job/address select, queue, live timeline, messages, checklist, accept with ETA, close, owner-only demo wipe.
- Address comes from the work order (no GPS in the artifact sandbox).
- Recognition output is a suggestion, always overridable; "Nem tudom" always available.

## Brand Commitments

- **E.ON brand is mandatory** (user-confirmed): E.ON red as the brand colour and an E.ON-recognisable feel. The redesign is new within that brand, not outside it.
- **Category standard, played straight** (user chose the canon direction, 2026-11-23): the craft bar is Apple's own iOS apps (Reminders, Maps, Find My) and Linear mobile. Native iOS conventions over invented ones.
- Must not feel playful, startup-like or like generic AI-generated UI.

## Evidence on Hand

- Clickable prototype and 17-slide deck already exist (separate artifacts).
- All addresses, names, job numbers and test timings are fictional demo data; no real E.ON data, customers or metrics may be invented as claims.

## Product Principles

1. Seconds matter: every extra tap or wait is a regression.
2. Readable outdoors, operable one-handed and gloved.
3. The app suggests, the technician decides.
4. Nobody is left wondering: every report shows its delivery and handling state.
5. A work tool, not a consumer app: no playful, startup or generic AI-styled surface.

## Accessibility & Inclusion

High contrast for sunlight, large touch targets (gloves), no reliance on colour alone for severity, reduced-motion respected.
