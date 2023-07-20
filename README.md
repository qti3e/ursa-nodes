# Ursa Nodes

Configurations to run 3 [Fleek Network Draco](https://fleek.network) nodes locally.

# Usage

If you have `draco` cloned as a neighbour of this repository you can:

Open 3 terminal windows/tabs, cd to each directory and run:

```
cargo run --manifest-path=../../draco/Cargo.toml -- --config config.toml run
```

# Clean up

You can clear the database and storage used by each node by simply doing:

```
rm -rf */data
```
# Note
This runs 3 of the 4 genesis committee nodes which is enough to come to consensus 
