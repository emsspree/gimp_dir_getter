# A `gimp-directory` Getter

This program is written to work as part of a chain of programs and to do one thing well:
  Look for the current user’s GIMP 3
  [configuration/settings directories](https://docs.gimp.org/3.0/en/gimp-fire-up.html#gimp-concepts-setup)
  and output their paths. 
  It intentionally checks only specific default locations
  and respects `GIMP3_DIRECTORY` as well as `XDG_CONFIG_HOME`.
  Not supported are “portable” versions and customized directories (built with `‑Dgimpdir=…`).

| Options:        |      |
| --------        | ---- |
|`‑v`, `‑‑version`| Show program version
|`‑h`, `‑‑help`   | Show help message
|`‑‑even`         | Only include even minor versions. Stable GIMP release versions always have [even minor versions](https://developer.gimp.org/core/maintainer/versioning/). |
|`‑‑odd`          | Only include odd minor versions. |
|`‑‑only`         | Only include specific version numbers and/or tags. Example:<br>`--only=3.2 --only=3.4,flatpak` |
|`‑‑ignore`       | Exclude specific Versions and/or Tags.             Example:<br>`--ignore=3.1 --ignore=3.3,snap` |
|**Tags:**        | `env`, `xdg`, `flatpak`, `snap`, `macos`, `windows` |
