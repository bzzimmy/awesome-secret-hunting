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
- [Methodology & Research](#methodology--research)


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
- [Shodan](https://www.shodan.io) - Internet-facing services exposing dashboards, debug endpoints, and config files.
- [iOS Apps](https://apps.apple.com) - Embedded `Info.plist` values, hardcoded strings in binaries, and bundled config files.


## Secret Scanners

- [Betterleaks](https://github.com/betterleaks/betterleaks) - Secrets detection tool by the original Gitleaks maintainers, adding secrets validation via CEL, parallelized Git scanning, and a token efficiency filter.
- [Gitleaks](https://github.com/gitleaks/gitleaks) - Regex-based secret detection tool for scanning Git repos, files, and stdin for passwords, API keys, and tokens.
- [Kingfisher](https://github.com/mongodb/kingfisher) - SIMD-accelerated secret scanner built in Rust with live validation, revocation, and blast radius mapping across repos, cloud storage, and chat platforms.
- [Titus](https://github.com/praetorian-inc/titus) - Hyperscan-accelerated secrets scanner with 487 rules that runs as a CLI, Go library, Burp Suite extension, and Chrome extension.
- [TruffleHog](https://github.com/trufflesecurity/trufflehog) - Finds and validates leaked credentials across Git, wikis, chats, logs, object stores, and filesystems with over 800 secret type detectors.


## Methodology & Research

- [EMERALDWHALE: 15k Cloud Credentials Stolen in Operation Targeting Exposed Git Config Files](https://www.sysdig.com/blog/emeraldwhale) - Sysdig's breakdown of a real-world operation that scraped exposed `.git/config` files at scale, stealing 15k+ cloud credentials using automated tooling.
- [Fresh From The Docks: Uncovering 100,000 Valid Secrets in DockerHub](https://blog.gitguardian.com/fresh-from-the-docks-uncovering-100-000-valid-secrets-in-dockerhub/) - Scanning 15 million Docker images and downloading 50TB+ of data to find 100,000 validated secrets including AWS keys from Fortune 500 companies.
- [How I Found 39 Algolia Admin Keys Exposed Across Open Source Documentation Sites](https://benzimmermann.dev/blog/algolia-docsearch-admin-keys) - Scraping 15,000 documentation sites and scanning Git history to find admin API keys with full write access to search indexes for projects like Home Assistant and KEDA.
- [How I Made $15k in Bug Bounties from GitHub Secret Leaks](https://tillsongalloway.com/finding-sensitive-information-on-github/index.html) - Foundational offensive methodology for finding secrets on GitHub via Code Search heuristics targeting config files, bash history, and data science scripts.
- [How I Scanned All of GitHub's "Oops Commits" for Leaked Secrets](https://trufflesecurity.com/blog/guest-post-how-i-scanned-all-of-github-s-oops-commits-for-leaked-secrets) - Using GitHub Archive to scan force-pushed and deleted commits for secrets developers thought they had removed.
- [Millions of Secrets Exposed via Web Application Frontends](https://redhuntlabs.com/blog/millions-of-secrets-exposed-via-web-application-frontend/) - Internet-scale scan of 500M+ domains discovering 1.6 million secrets embedded in client-side JavaScript and HTML, with the release of HTTPLoot for automated frontend secret extraction.
- [Postman Carries Lots of Secrets](https://trufflesecurity.com/blog/postman-carries-lots-of-secrets) - Scanning 40,000 Postman workspaces via the Postman search API and finding 4,000+ live credentials across 183 secret types including AWS, GCP, and Slack webhooks.
- [Scanning 5.6 Million Public GitLab Repositories for Secrets](https://trufflesecurity.com/blog/scanning-5-6-million-public-gitlab-repositories-for-secrets) - Scanning every public GitLab repo with TruffleHog, uncovering 17,000+ verified live secrets and earning $9,000+ in bounties.
- [Shopify GitHub Access Token Exposure](https://hackerone.com/reports/1087489) - Extracting a GitHub PAT from an Electron app's `.asar` archive that granted write access to all of Shopify's repositories, resulting in a $50,000 bounty.


## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.
