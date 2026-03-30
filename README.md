# TYTSPOT CLI

TYTSPOT CLI helps developers run security scans, review findings, and work with reports directly from the terminal.

## Recommended install

Install with npm:

```bash
npm install -g @tytspot/cli
```

Then connect your account:

```bash
tytspot auth tyt_your_tytspot_key
```

Or sign in with your account:

```bash
tytspot login -email you@company.com -password your-password
```

## Quick start

```bash
tytspot scan url https://example.com
tytspot scan url https://example.com -deep
tytspot scan repo https://github.com/j3p3rg/tytspot-cli
tytspot scans list
tytspot report basic scan_123
```

## Advanced recon

TYTSPOT CLI keeps standard scanning as the default.

If you want deeper validation, use `-deep` or `--deep`:

```bash
tytspot scan url https://example.com -deep
tytspot scan repo https://github.com/j3p3rg/tytspot-cli --deep
```

That tells TYTSPOT to run:

- `mode: controlled-proof`
- `scanProfile: advanced-recon`

## Binary releases

If you do not want npm, download binaries from:

[https://github.com/j3p3rg/tytspot-cli/releases/latest](https://github.com/j3p3rg/tytspot-cli/releases/latest)

## Production API

The release binaries use the production TYTSPOT API by default:

```text
https://api.tytspot.com/v1
```
