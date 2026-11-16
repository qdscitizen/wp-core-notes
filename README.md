# wp-core-notes

Reading notes on WordPress core source, verified against a local WP install (file:line evidence + Xdebug):

- the_content render path — priority pipeline, blocks, shortcodes, WP_Hook internals
- pre_* write path — input sanitization before INSERT
- nonces — proof of intent, not permission
- object cache invalidation — meta cache vs query cache, last_changed version numbers, Redis and object-cache.php
- case study — which layer actually renders a header menu (Elementor vs nav_menu vs wp_navigation)
- case study — classic vs block themes and Elementor takeover
- tooling — Xdebug under XAMPP

Documents:

- `wordpress-core-render-write-security-notes.html`
- `wordpress-object-cache-invalidation-notes.html`
- `wordpress-classic-vs-block-themes-and-elementor-takeover.html`
- `learning-review-nov-2026.html`
