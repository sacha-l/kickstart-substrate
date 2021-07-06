# kickstart-substrate
This pulls from an actively updated branch of Substrate's node template. It
runs a script in `template.toml` which makes it easy to customize a node template. Customize is a big word. For now it does the little things: 
1. Renames the template pallet.
2. Renames the node.

## 🧐 How to use it

Install `kickstart` (you'll only need to do this once):
```rust
cargo install --git https://github.com/Keats/kickstart.git --branch next
```

`cd` in the directory you'd like this project to live in and run:

```bash
kickstart https://github.com/sacha-l/kickstart-substrate
```
Then, you'll be prompted to type in the pallet and node names.

If you want to specify a folder to clone into, run:

```bash
mkdir <folder_name>
kickstart https://github.com/sacha-l/kickstart-substrate -o <folder_name>
```

## ⌛ Coming soon™️
- A way to add more pallets from the CLI using Tera.
- A way to do some basic pallet scaffolding based on user input. For example, storage items; events; errors.
- Ask user if they're using the template for production. If yes, handle the renaming of author and project repositories.

## 🙏 Acknowledgements 
Thanks to [Keats](https://github.com/Keats) for making the [Kickstart tool](https://github.com/Keats/kickstart) and for [Chevdor](https://github.com/chevdor) for showing it to me!
