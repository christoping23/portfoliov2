# Christopher Tong — Portfolio

Static portfolio in C:\Portfolio. Semantic HTML, CSS, and vanilla JavaScript; no build or runtime dependencies.

## View

Open index.html in a modern browser. The current local preview, while its server is running, is http://127.0.0.1:8765/.

## Files

- index.html: all content, semantic sections, native FAQ disclosures, five live project links.
- styles.css: responsive visual system, button feedback, tools loop, reduced-motion overrides.
- scripts/main.js: mobile navigation, safe Upwork activation, progressive section entrances, tool-strip pause control.
- scripts/config.js: UPWORK_PROFILE_URL remains empty.

## Assets still needed

- Christopher's portrait: replace the .portrait placeholder with the supplied image, preserving its reserved frame dimensions. Store the image under assets/ inside this project.
- Real homepage screenshots are stored in assets/projects/. All five project frames now show these captures without added text overlays. Refresh these images when the source websites change.
- Tool marks are simple text/symbol identifiers, not official brand-logo assets.
- Confirm LotHub's stack, Merch Mommery customization scope, and individual game-project responsibilities.
- Real Upwork URL and final deployment domain.

## Accessibility and motion

Content is visible by default. Without JavaScript the navigation stays available, FAQs work, and tools wrap as a static list. The enhanced tool loop has a pause control and pauses on hover/focus. Duplicate list content is hidden from assistive technology. Reduced motion disables decorative animations and restores a static tools list.

## Verification for the visual rework

Browser checks: desktop and 390px mobile views; document overflow measured at 390, 768, 1024, 1440, and 1920px; native FAQ expansion; tools pause; mobile menu opening and Escape dismissal; external-link rel attributes; empty Upwork disabled state; no browser JavaScript errors. JavaScript passed node --check.

Reduced-motion and JavaScript-disabled behavior were reviewed in source; they were not separately browser-emulated. No deployment was performed.


## Interactive project previews

The existing homepage images remain the no-JavaScript fallback. The deferred
scripts/project-previews.js manifest adds two public website sections per project
in page order. Extras load on demand, not at page load. Hover cycles every 1350ms
with a 260ms crossfade; leaving restores the homepage. Keyboard focus also starts previews; Escape resets, and only one card runs at a time. Offscreen
and hidden-tab previews stop. Touch and reduced-motion users keep the static homepage image. No counters or preview buttons are displayed.

Additional captures (September 17, 2026), in assets/projects:
- lothub-2.jpg / lothub-3.jpg: https://lothub.shop/ — listings, discovery.
- merch-mommery-2.jpg / merch-mommery-3.jpg: https://merchmommery.com/ — products, personalized collections.
- vanguard-2.jpg / vanguard-3.jpg: https://www.dkvanguard.com/ — ranking, event timer.
- loacastle-2.jpg / loacastle-3.jpg: https://www.loacastle.online/ — classes, rates.
- new-era-2.jpg / new-era-3.jpg: https://www.neweradk.com/ — classes, rates.

These are public website captures, not screenshots of private dashboards or
launcher software. To extend a sequence, add optimized images and their descriptive
labels to the scenes manifest in scripts/project-previews.js.