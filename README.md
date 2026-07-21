# Flowersauce KiCad Library

Personal KiCad symbol, footprint, datasheet, and 3D model library.

## Conventions

- Target KiCad version: latest stable KiCad used by the maintainer.
- Keep symbol libraries coarse-grained:
  - `Flowersauce_Active.kicad_sym`
  - `Flowersauce_Passive.kicad_sym`
  - `Flowersauce_Mechanical.kicad_sym`
- Prefer official KiCad connector symbols; keep only the custom connector footprints locally.
- Keep footprint libraries coarse-grained:
  - `Flowersauce_Active.pretty`: ICs, sensors, memory, SoCs, powered semiconductors, and active packages.
  - `Flowersauce_Passive.pretty`: passives, protection devices, crystals, magnetics, switches, buzzers, and motors.
  - `Flowersauce_Connectors.pretty`: board, cable, card, and external connectors.
  - `Flowersauce_Mechanical.pretty`: mounting, socket, and mechanical features.
- Use English names without spaces. Prefer KiCad official library naming style for individual symbols and footprints.
- Name active IC symbols by their exact part number or intentional compatible family name.
- Name passive, protection, connector, electromechanical, and mechanical symbols as `Function_PartNumber` when the function prefix improves searchability.
- Prefer KiCad official symbols for generic passives and protection devices; keep local footprints when only the package is custom.
- Keep symbol fields close to KiCad defaults: `Reference`, `Value`, `Footprint`, `Datasheet`, `Description`, `ki_keywords`, and `ki_fp_filters`.
- Keep `Description` in Chinese where practical, and keep `ki_keywords` as English search terms.
- Do not keep supplier, price, or temporary import metadata in library fields.
