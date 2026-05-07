# A `gimp-directory` Getter

This helper looks for GIMP 3
  [configuration/settings directories](https://docs.gimp.org/3.0/en/gimp-fire-up.html#gimp-concepts-setup)
  and outputs their paths.



It supports filtering
  by release cycles (even/odd),
  by version number, and 
  by tags for installation sources.

| Options:        |      |
| --------        | ---- |
|`‑v`, `‑‑version`| Show program version
|`‑h`, `‑‑help`   | Show help message
|`‑‑even`         | Only include even minor versions (e.g., 3.0, 3.2, 3.4).<br>Stable GIMP release versions always have [even minor versions](https://developer.gimp.org/core/maintainer/versioning/). |
|`‑‑odd`          | Only include odd minor versions (e.g., 3.1, 3.3, 3.5). |
|`‑‑only`         | Only include specific version numbers and/or tags.<br>Example:<br>`gimp_dir_getter --only=3.0 --only=3.4,snap` |
|`‑‑ignore`       | Exclude specific Versions and/or Tags.            <br>Example:<br>`gimp_dir_getter --ignore=3.0 --ignore=3.4,snap` |
|**Tags:**        | `env`, `xdg`, `flatpak`, `snap`, `macos`, `windows` |
