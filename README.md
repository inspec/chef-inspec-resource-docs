# Chef InSpec Resource Documentation

This repository contains a blank Hugo site configured for Chef InSpec resource documentation. The site is based on the configuration from the [chef-inspec-docs](https://github.com/inspec/chef-inspec-docs) repository.

## Structure

This repository includes:

- Hugo configuration files (`config/`, `hugo.toml`, etc.)
- Package management files (`package.json`, `go.mod`)
- Build and deployment scripts (`Makefile`, `scripts/`)
- Basic site structure with empty content directory
- Linting and quality tools configuration (`.markdownlint.yaml`, `.vale.ini`, `cspell.yaml`)

## Getting Started

1. Install dependencies:
   ```bash
   npm install
   ```

2. Build the site:
   ```bash
   make bundle
   hugo --buildDrafts --buildFuture --cleanDestinationDir
   ```

3. Serve locally:
   ```bash
   make serve
   ```

## Adding Content

Add your documentation content to the `content/` directory. The site uses Hugo's content management system and the Chef docs theme.

## License

Licensed under the Creative Commons Attribution 4.0 International License. See `LICENSE` file for details.