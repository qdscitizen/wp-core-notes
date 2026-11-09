# wp-core-notes

Reading notes on WordPress core source, verified against a local WP install (file:line evidence + Xdebug):

- the_content render path — priority pipeline, blocks, shortcodes, WP_Hook internals
- pre_* write path — input sanitization before INSERT
- nonces — proof of intent, not permission
- case study — which layer actually renders a header menu (Elementor vs nav_menu vs wp_navigation)
- tooling — Xdebug under XAMPP

Document: `wordpress-core-render-write-security-notes.html`
