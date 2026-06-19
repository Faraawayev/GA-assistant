# AGENTS.md — AI Beauty Assistant Prototype for Золотое Яблоко

## Project Overview
Single-file HTML prototype of an AI chat assistant embedded into 
the Золотое Яблоко mobile app interface. Target: demo for CPO and team.

## Tech Stack
- Pure HTML/CSS/JavaScript (no framework, no build tools)
- OpenAI API (gpt-4o-mini) via fetch() in browser
- Mobile-first layout (375px width — iPhone 14 baseline)
- No backend required — API key stored in a JS constant for prototype

## Design Rules (CRITICAL)
- Reproduce the Золотое Яблоко brand: hot pink #FF006E, black, white
- Font: system-ui or -apple-system (closest to the app)
- Bottom tab bar: 5 items matching the app screenshots
- AI button placement: floating button (56px circle, hot pink) 
  bottom-right corner, above tab bar
- Chat window: slide-up sheet (90% viewport height), rounded top corners

## AI Assistant Behavior
- Assistant name: «Яблочко» or «Золотой помощник» (decide per prompt)
- Handles: product search, personal recommendations, FAQ, order status
- Language: Russian only
- Tone: friendly, concise, emoji-positive (beauty retail vibe)
- Static demo responses are acceptable for prototype if no API key

## File Structure
- Single file: index.html (all CSS and JS inline)
- Screenshots reference: /goldapple-screens/*.png

## Done When
- [ ] Main screen renders matching the screenshots
- [ ] AI chat button visible and tappable
- [ ] Chat window opens with slide-up animation
- [ ] User can type a message and receive a response
- [ ] Response covers: product recommendation, FAQ, search scenario
- [ ] Works in Chrome mobile simulation (F12 → device mode → iPhone 14)

## Do NOT
- Do not use React, Vue, or any framework
- Do not add a build step
- Do not use external CSS libraries (Tailwind OK only if CDN)
- Do not truncate code — always output complete files
