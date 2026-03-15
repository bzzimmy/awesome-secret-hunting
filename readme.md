<p align="center">
  <br>
  <img width="400" src="./assets/logo.png" alt="logo of awesome-secret-hunting repository">
  <br>
  <br>
</p>

## Awesome Secret Hunting [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Detecting secrets and credentials leaked in source code, repositories, and digital assets.


## Contents

- [Platforms](#platforms)
- [Secret Scanners](#secret-scanners)


## Platforms

Where secrets leak.

- [Android APKs](https://play.google.com) - Decompiled source code, `AndroidManifest.xml`, string resources, and embedded config files.
- [Bitbucket](https://bitbucket.org) - Public repositories, commit history, and verbose pipeline logs.
- [Chrome Web Store](https://chromewebstore.google.com) - Extension source code, background scripts, and bundled config files with hardcoded API keys.
- [Codeberg](https://codeberg.org) - Public repositories and commit history on this Gitea-based forge.
- [crates.io](https://crates.io) - Published Rust crate source code and bundled config files.
- [Docker Hub](https://hub.docker.com) - Image layers, embedded environment variables, and baked-in config files.
- [Electron Apps](https://www.electronjs.org) - Extracted `.asar` archives containing `.env` files, hardcoded tokens, and leftover build artifacts.
- [GitHub](https://github.com) - Public repos, gists, commit history, pull requests, issue comments, and GitHub Actions logs.
- [GitLab](https://gitlab.com) - Public projects, snippets, merge requests, and CI/CD job logs.
- [Hugging Face](https://huggingface.co) - Model repos, dataset repos, and Spaces with hardcoded API keys and tokens.
- [Maven Central](https://search.maven.org) - Bundled configuration and properties files in Java/Kotlin packages.
- [npm](https://www.npmjs.com) - Published source code, `.env` files, and config files in JavaScript packages.
- [NuGet](https://www.nuget.org) - Embedded credentials and config files in .NET packages.
- [Packagist](https://packagist.org) - Configuration files and hardcoded credentials in PHP Composer packages.
- [Pastebin](https://pastebin.com) - Public pastes containing credentials, `.env` dumps, and debug output.
- [Postman](https://www.postman.com) - Public workspaces, shared collections, and environment variables with hardcoded tokens.
- [PyPI](https://pypi.org) - Published source code, config files, and `.env` files in Python packages.
- [RubyGems](https://rubygems.org) - Published gem source code and bundled config files with embedded credentials.
- [iOS Apps](https://apps.apple.com) - Embedded `Info.plist` values, hardcoded strings in binaries, and bundled config files.
- [Shodan](https://www.shodan.io) - Internet-facing services exposing dashboards, debug endpoints, and config files.


## Secret Scanners

- [Betterleaks](https://github.com/betterleaks/betterleaks) - Secrets detection tool by the original Gitleaks maintainers, adding secrets validation via CEL, parallelized Git scanning, and a token efficiency filter.
- [Gitleaks](https://github.com/gitleaks/gitleaks) - Regex-based secret detection tool for scanning Git repos, files, and stdin for passwords, API keys, and tokens.
- [Kingfisher](https://github.com/mongodb/kingfisher) - SIMD-accelerated secret scanner built in Rust with live validation, revocation, and blast radius mapping across repos, cloud storage, and chat platforms.
- [Titus](https://github.com/praetorian-inc/titus) - Hyperscan-accelerated secrets scanner with 487 rules that runs as a CLI, Go library, Burp Suite extension, and Chrome extension.
- [TruffleHog](https://github.com/trufflesecurity/trufflehog) - Finds and validates leaked credentials across Git, wikis, chats, logs, object stores, and filesystems with over 800 secret type detectors.


## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.
