<p align="center">
  <img src="https://raw.githubusercontent.com/getdeadrecon/deadrecon/main/docs/assets/deadrecon-card.png" width="276" alt="DeadRecon logo: tarot card XIII, a skull with a red censor bar across its eyes">
</p>

<h1 align="center">DeadRecon</h1>

<p align="center"><strong>The OPSEC-native OSINT framework.</strong><br>Recon that doesn't burn your infrastructure, and an honest report of exactly what each scan leaked.</p>

<p align="center"><em>Formerly PhantomSignal.</em></p>

<p align="center">
  <a href="https://pypi.org/project/deadrecon/"><img src="https://img.shields.io/pypi/v/deadrecon?style=flat-square&color=ff3b1f&logo=pypi&logoColor=white" alt="PyPI version"></a>
  <a href="https://github.com/getdeadrecon/deadrecon/stargazers"><img src="https://img.shields.io/github/stars/getdeadrecon/deadrecon?style=flat-square&color=ff3b1f&logo=github" alt="GitHub stars"></a>
  <img src="https://img.shields.io/badge/python-3.10+-111111?style=flat-square&logo=python&logoColor=white" alt="Python 3.10+">
  <a href="https://github.com/getdeadrecon/deadrecon/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-f7de52?style=flat-square" alt="MIT license"></a>
</p>

---

```bash
pip install deadrecon
deadrecon scan example.com         # DNS, ports, tech and threat intel
deadrecon scan example.com --tor   # starts Tor for you, and stops if it can't confirm it
deadrecon web                      # open the web console
```

## Why DeadRecon

- **It tells you what you leaked.** Every scan ends with an OPSEC grade and a per-module breakdown of what was proxied and what traces back to you. The grades were checked against packet captures, and they're deliberately unflattering.
- **One-click Tor that fails closed.** DeadRecon starts Tor, confirms each scan is on it before touching the target, and stops if it can't. Modules that would bypass Tor are skipped and listed in the report.
- **Scans don't name the tool.** SMTP greetings and User-Agents no longer identify DeadRecon to targets or third parties, as confirmed with packet captures.
- **A full recon pipeline.** Subdomains, ports, tech fingerprinting, web crawling and vulnerability scanning, plus 50+ intelligence integrations. Many sources need no API key.
- **Your choice of output.** Use the web console, CLI or REST API, and export to JSON, CSV, HTML, PDF, XLSX, XML, Markdown or STIX 2.1.

**For authorized security research, investigations and education only.** Only scan targets you have permission to test.

---

[Website](https://deadrecon.sh) · [Source](https://github.com/getdeadrecon/deadrecon) · [PyPI](https://pypi.org/project/deadrecon/) · [Docs](https://github.com/getdeadrecon/deadrecon/blob/main/docs/USAGE.md) · [Changelog](https://github.com/getdeadrecon/deadrecon/blob/main/CHANGELOG.md)

Security reports: `security@deadrecon.sh`
