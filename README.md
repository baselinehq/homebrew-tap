# homebrew-costgraph

Homebrew tap for installing `costgraph` and related CLI tools from `baselinehq`.

## Installation

```bash
brew tap baselinehq/tap
brew install baselinehq/tap/costgraph
```

Or install directly (if formula name differs):

```bash
brew install baselinehq/tap/<formula>
```

## Usage

Run the installed CLI:

```bash
costgraph-agent --help
```

Replace `costgraph` with the actual formula binary name as needed.

## Contributing

- Add new formulae under `Formula/` (or top-level `*.rb`).
- Follow Homebrew formula style and run:
  ```bash
  brew audit --new-formula --strict Formula/<your-formula>.rb
  brew install --build-from-source Formula/<your-formula>.rb
  brew test Formula/<your-formula>.rb
  ```
- Open a PR against `main`. Include CI-friendly instructions and a brief test plan.

## CI / Releases

Use GitHub Actions to lint and validate formulae on PRs. Ensure bottles are built/referenced per Homebrew guidelines.

## License

See `LICENSE` in this repository.
