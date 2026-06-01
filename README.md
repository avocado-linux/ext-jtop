# ext-jtop

Jetson system monitoring via jtop (jetson-stats)

Extracted from `avocado-os` folder `extensions/jtop` (branch `main`).
The `distro:` block was dropped and `sdk.image` points at
`{{ env.AVOCADO_DISTRO_RELEASE }}-{{ env.AVOCADO_DISTRO_CHANNEL }}` —
set those in CI; release/channel are build-context, not extension, properties.
