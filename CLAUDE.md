# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

A single-page gym landing page ("IronForge Gym" — a demo/placeholder brand). The whole site is one static file, `index.html`, with inline `<style>` and no JavaScript, build step, package manager, linter, or tests. To run it, open `index.html` in a browser.

## Structure of `index.html`

- CSS lives in one `<style>` block; sections are: nav, hero, about, gallery, contact bar, plans, WhatsApp button, footer, then a single `@media (max-width: 720px)` block for mobile overrides. New styles that need mobile behavior must be added to that media block.
- Page sections are anchored by `id` (`about`, `gallery`, `plans`, `contact`) and the fixed nav links to them. `section` has `scroll-margin-top: 70px` so the fixed navbar doesn't cover headings — keep this when adding sections.
- Images are hotlinked from Unsplash (internet required); there is no local `images/` folder.
- The accent color `#ff4d2e` is hardcoded throughout (no CSS variables).

## Content conventions

- The contact phone number appears in three places and must be changed together: the `tel:` link in the contact bar, the `wa.me/<number>` WhatsApp link (country code `91`, no `+`), and the footer. The WhatsApp link pre-fills the message `AAP NALLE HAI!!!!!`.
- The footer's "Demo Website" text and its separate contact number (9247868686) are deliberate; the site is a demo.
- Plan prices (₹999 / ₹2,499 / ₹7,999) and the email `info@ironforge.com` are placeholders, not real client data.
- The user communicates in Hinglish (Hindi in Roman script); reply in the same style.

## Rules

1. Har change chhote steps mein karo, aur har step ke baad simple Hinglish mein batao kya badla aur browser mein kaise check karun.
2. Chhote bug ke liye poori file dobara mat likho.
3. Koi bhi fake ya placeholder data (address, phone, email) mat daalo. Info nahi pata to mujhse pucho.
4. Kabhi bhi secret key ya password code mein mat likho.
5. Har link aur button kaam karna chahiye.

## Git

Remote `origin` is `https://github.com/KIRAAK-CODER/LEARNING.git`, branch `main`. The user asks explicitly for commits and pushes; don't do either unprompted.
