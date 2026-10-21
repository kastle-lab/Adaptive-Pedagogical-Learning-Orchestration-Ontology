# Synthetic Sample Mappings

One YAML mapping per synthetic CSV file.

Each `.yaml` file maps the same-named CSV in [synthetic_data/](../../synthetic_data/) to RDF/Turtle fragments in [materialization/](../../materialization/).

| Mapping Block | Purpose                                                                  |
| ------------- | ------------------------------------------------------------------------ |
| `metadata`    | Describes the source mapping.                                            |
| `cvs`         | Defines controlled vocabulary individuals when needed.                   |
| `root`        | Defines the row-level RDF resource and its predicate-object connections. |

Mappings use APLO and CurrKG prefixes such as `aplo-ont`, `aplo-r`, `currkg`, and `currkg-r`. Multi-valued CSV cells use `|` as the separator.
