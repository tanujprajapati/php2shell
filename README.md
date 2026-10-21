# README — PHP vulnerability tracking resources
**[php-vulnerability-tracking-resources.md](./php-vulnerability-tracking-resources.md)**
Curated **URLs + short descriptions** for:
- **php2shell** (CVE-2026-109618 / CVE-2026-109619) — official advisories, vendor blogs, forums
- **Detection rules** — Sigma, Falco, Suricata/Zeek, WAF (Cloudflare/Akamai), ModSecurity, EDR/SIEM notes
- **Tools** — GitHub/GitLab repos (PoC, triage, repo-audit, process-watcher, Corelight, NCSC-NL)
- **Composer / Packagist** — FriendsOfPHP, Packagist API, GitLab GLAD
Use it as a **watchlist** or paste sections into Confluence/GitHub wikis. Re-check links after PHP security releases.
## Who it’s for
SOC, AppSec, and platform teams tracking PHP runtime incidents and Composer supply-chain advisories.
## Start here (php2shell)
| What | Link |
|------|------|
| Patch versions | PHP **8.2.35**, **8.3.36**, **8.4.27**, **8.5.12** — [php.net archive](https://www.php.net/archive/2026.php) |
| Official GHSAs | [GHSA-w8hw-w9fx-j79w](https://github.com/php/php-src/security/advisories/GHSA-w8hw-w9fx-j79w), [GHSA-6wmf-4rv5-p3rp](https://github.com/php/php-src/security/advisories/GHSA-6wmf-4rv5-p3rp) |
| National ops hub | [NCSC-NL/php2shell](https://github.com/NCSC-NL/php2shell) |
| Network rules (OSS) | [corelight/php2shell-detect](https://github.com/corelight/php2shell-detect) |
**Fix:** upgrade PHP and restart workers. WAF rules are defense-in-depth only.
## Related artifacts in this repo
| Artifact | Path |
|----------|------|
| Detections (Sysdig + Defender) | [threat-intel-detections-php-up-2026.md](./threat-intel-detections-php-up-2026.md) |
| Sysdig runtime queries | [../query-bank/sysdig/QB-20261021-phpup-runtime-detections.md](../query-bank/sysdig/QB-20261021-phpup-runtime-detections.md) |
| Edge WAF rule IDs | [../query-bank/opensearch/EDGE-PHP2SHELL-001-waf-vendor-rule-ids.json](../query-bank/opensearch/EDGE-PHP2SHELL-001-waf-vendor-rule-ids.json) |
