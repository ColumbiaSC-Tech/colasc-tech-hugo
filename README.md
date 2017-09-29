## Contributing

Start with `git clone --recursive`.

There are two submodules.
1) public/ - points to the actual location where github pages are rendered
2) themes/hugo-theme-nix/ - points to a fork currently of the chosen theme

Hugo is used to populate the public folder.

To verify changes locally:
`$ hugo serve`

To build and prepare for submission:
`$ hugo`

An example for pushing a simple update:

1. Make changes, perhaps by modifying config.toml
2. Rebuild by executing `hugo`
3. pushd public && git commit -a "simple change update" && git push
4. popd && git commit -a "simple change update, bump submodule" && git push
