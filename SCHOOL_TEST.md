# Keine School v15.4 isolated web preview

Source commit: b476739372c03e2a2d010cfd505a1bccf71fa2c8.
This repository is a separate web preview; the original repository and backups are unchanged.

- Local keys: gensokyo-rpg-school-test:permanent and gensokyo-rpg-school-test:lastVisit.
- No Firebase configuration script or cloud UI module is loaded by either HTML entry page.
- Both HTML entries have a Content Security Policy limiting scripts and fetch connections to this site (inline/eval retained for the existing game).
- Production Firebase files remain unchanged as source history; they are not initialized in this preview.
- Production save JSON may be explicitly imported into test storage. Exports use test keys and a TEST filename; they are not automatically usable by the production launcher.
- No production cloud reads, writes, Google login or automatic synchronization.
- noindex, nofollow retained. Public access remains possible; noindex is not authentication.
