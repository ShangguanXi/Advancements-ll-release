## 0.2.0 - 2026-10-16
### Added

- Other mods can ship their own advancements in `mods/<mod>/data/<namespace>/advancements/`, laid out like a Java Edition data pack: `<path>.json` becomes `<namespace>:<path>`. Namespaces may only use `a-z0-9_.-`. Each mod that ships advancements gets a line in the log.
- This mod's own `data/advancements/` stays in the `minecraft` namespace, so existing progress is kept.
- Duplicate advancement ids are logged and the first one loaded is kept. This mod's advancements load first, so other mods cannot replace vanilla ones.

### Fixed

- Titles written as `{"text": ...}` showed the advancement id in the chat announcement and in the toast sent to players without the mod.

## 0.1.0 - 2026-10-16
### Added

- First release.
