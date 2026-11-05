# Foundry Mappings for Synthetic Data

One YAML mapping is provided for each synthetic CSV file. Each mapping converts its
same-named source CSV in [synthetic_data/](../synthetic_data/) into RDF/Turtle
fragments in [materialized_instances/](../materialized_instances/).

| Mapping Block | Purpose                                                                  |
| ------------- | ------------------------------------------------------------------------ |
| `metadata`    | Describes the source mapping.                                            |
| `cvs`         | Defines controlled vocabulary individuals when needed.                   |
| `root`        | Defines the row-level RDF resource and its predicate-object connections. |

Mappings use APLO and CurrKG prefixes such as `aplo-ont`, `aplo-r`, `currkg`, and `currkg-r`. Multi-valued CSV cells use `|` as the separator.

These mappings were run with [Kastle Foundry](https://github.com/kastle-lab/foundry).
