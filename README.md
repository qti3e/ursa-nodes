# Ursa Nodes

Configurations to run 3 [Fleek Network Ursa](https://fleek.network) nodes locally.

# Usage

Open 3 terminal windows/tabs, cd to each directory and run:

```
cd node-01
ursa --config config.toml
```

```
cd node-02
ursa --config config.toml
```

```
cd node-03
ursa --config config.toml
```

If you have `ursa` cloned as a neighbour of this repository you can:

```
cd node-01
cargo run --manifest-path=../../ursa/Cargo.toml --bin ursa -- --config config.toml
```

# Clean up

You can clear the database and storage used by each node by simply doing:

```
rm -rf */data
```

# Note

In `./genesis_committee.json` file there are 4 nodes, that's because this is the minimum number of nodes we can
have and have the Narwhal consensus running, but only availability of 3 out of 4 nodes is required.

