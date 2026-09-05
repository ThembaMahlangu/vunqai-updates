# vunqai-updates

The update manifest for Vunqai, and nothing else.

Vunqai is a private application. This repository exists only so an installed
copy can ask whether a newer version has been published, without the
application carrying a credential to read a private repository.

`latest.json` holds the published version and a link to its release:

```json
{ "version": "v0.0.0", "url": "https://github.com/…/releases/tag/v0.0.0", "notes": "…" }
```

That link resolves only for someone signed in with access to the release. The
application itself, its installer and its source are not here and are not
public.

The check is notify-only: Vunqai reads this file, tells the user a newer
version exists, and never downloads or installs anything on its own.
