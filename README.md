# TYTSPOT

TYTSPOT is an AI-powered security testing platform for developers. It helps teams scan websites, repositories, APIs, containers, smart contracts, and mobile apps, then review findings and reports from the dashboard or the CLI.

## Recommended install

The recommended way to install the TYTSPOT CLI is with npm.

```bash
npm install -g @tytspot/cli
```

Then connect your account:

```bash
tytspot auth tyt_your_tytspot_key
```

Or sign in with your account credentials:

```bash
tytspot login -email you@company.com -password your-password
```

## Alternative install: GitHub Releases

If you do not want to use npm, download a release binary from:

[https://github.com/j3p3rg/tytspot-cli/releases/latest](https://github.com/j3p3rg/tytspot-cli/releases/latest)

Available release files:

- `tytspot-win-x64.zip`
- `tytspot-linux-x64.tar.gz`
- `tytspot-macos-x64.tar.gz`
- `tytspot-macos-arm64.tar.gz`
- `SHA256SUMS.txt`

## Quick start

Scan a website:

```bash
tytspot scan url https://example.com
```

Scan a repository:

```bash
tytspot scan repo https://github.com/j3p3rg/tytspot-cli
```

List scans:

```bash
tytspot scans list
```

Open a report:

```bash
tytspot report basic scan_123
```

## Windows install

Recommended first:

```powershell
npm install -g @tytspot/cli
```

Fallback binary install:

1. Download `tytspot-win-x64.zip`
2. Extract it
3. Move `tytspot.exe` to a folder such as `C:\Tytspot\bin`
4. Add that folder to your system `PATH`
5. Open a new terminal
6. Run:

```powershell
tytspot auth tyt_your_tytspot_key
```

## macOS install

Recommended first:

```bash
npm install -g @tytspot/cli
```

Fallback binary install:

1. Download:
   - `tytspot-macos-arm64.tar.gz` for Apple Silicon
   - `tytspot-macos-x64.tar.gz` for Intel
2. Extract the archive
3. Move `tytspot` to a folder on your `PATH`, such as `/usr/local/bin`
4. Run:

```bash
chmod +x tytspot
sudo mv tytspot /usr/local/bin/
tytspot auth tyt_your_tytspot_key
```

## Linux install

Recommended first:

```bash
npm install -g @tytspot/cli
```

Fallback binary install:

1. Download `tytspot-linux-x64.tar.gz`
2. Extract the archive
3. Run:

```bash
chmod +x tytspot
sudo mv tytspot /usr/local/bin/
tytspot auth tyt_your_tytspot_key
```

## Verify download integrity

Use `SHA256SUMS.txt` to verify your download before running it.



## Source code

Source code is available here:

- [https://github.com/j3p3rg/tytspot-cli/releases/latest](https://github.com/j3p3rg/tytspot-cli/releases/latest)



## Recommendation

If npm works on your machine, use npm first. It is the easiest install path and the easiest way to keep TYTSPOT CLI updated.
