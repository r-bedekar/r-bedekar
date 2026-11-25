## Security research

Vulnerability research on widely used open source packages, reported
privately to maintainers and published only after a fix ships.

- brace-expansion 5.0.13, 3.0.10, 2.1.8 and 1.1.22 (2026-11-11): CPU denial
  of service from patterns with unmatched braces and from the `{a},b}` check,
  reachable through minimatch and glob. Reported with a patch and tests,
  credited as finder in GHSA-6jwq-xf8q-xcwh (High).
  https://github.com/juliangruber/brace-expansion/security/advisories/GHSA-6jwq-xf8q-xcwh
- amqplib 2.3.0 (2026-11-08): security release for a client crash and
  unchecked inbound frame sizes reachable from a malicious or non-compliant
  broker. Reported with a patch and tests, credited in the release notes and
  as reporter in GHSA-37f9-7m79-6866 (Medium, published 2026-11-25).
  https://github.com/amqp-node/amqplib/releases/tag/v2.3.0
  https://github.com/amqp-node/amqplib/security/advisories/GHSA-37f9-7m79-6866
- authentik 2026.8.7 and 2026.5.9 (advisory published 2026-11-25): federated
  JWTs matched to existing users by username, so a token from a federated
  source could sign in as an existing account. Reported with a patch and
  tests, credited as reporter in GHSA-6v2c-352p-ghmw (High).
  https://github.com/goauthentik/authentik/security/advisories/GHSA-6v2c-352p-ghmw

## Malicious package reports

- @ethersphere/bee-js 13.3.0 (2026-11-13): compromised npm release with a
  malicious postinstall loader that stole Swarm node keys and installed a
  remote-access agent. Credited as finder in the project's advisory
  GHSA-9f32-98m9-4jx3 (Critical).
  https://github.com/ethersphere/bee-js/security/advisories/GHSA-9f32-98m9-4jx3

22 entries in the OpenSSF malicious-packages database (ossf/malicious-packages),
all npm, 15 as finder and 7 as analyst, July to October 2026. Found through
ChainGate, supply chain threat detection for the npm ecosystem.

| OSV id | package | role | published |
|---|---|---|---|
| [MAL-2026-10165](https://osv.dev/vulnerability/MAL-2026-10165) | @injectivelabs/sdk-ts | analyst | 2026-07-10 |
| [MAL-2026-11212](https://osv.dev/vulnerability/MAL-2026-11212) | @goodjavascript/dotenv | analyst | 2026-07-30 |
| [MAL-2026-11656](https://osv.dev/vulnerability/MAL-2026-11656) | @onereach/styles | finder | 2026-08-04 |
| [MAL-2026-11674](https://osv.dev/vulnerability/MAL-2026-11674) | @or-sdk/base | finder | 2026-08-04 |
| [MAL-2026-11689](https://osv.dev/vulnerability/MAL-2026-11689) | @or-sdk/discovery | finder | 2026-08-04 |
| [MAL-2026-11691](https://osv.dev/vulnerability/MAL-2026-11691) | @or-sdk/event-manager | finder | 2026-08-04 |
| [MAL-2026-11721](https://osv.dev/vulnerability/MAL-2026-11721) | @or-sdk/providers | finder | 2026-08-04 |
| [MAL-2026-11724](https://osv.dev/vulnerability/MAL-2026-11724) | @or-sdk/sdk-api | finder | 2026-08-04 |
| [MAL-2026-11755](https://osv.dev/vulnerability/MAL-2026-11755) | @ornikar/eslint-plugin-ornikar | finder | 2026-08-04 |
| [MAL-2026-11758](https://osv.dev/vulnerability/MAL-2026-11758) | @ornikar/jest-config | finder | 2026-08-04 |
| [MAL-2026-11870](https://osv.dev/vulnerability/MAL-2026-11870) | @servicetitan/form | finder | 2026-08-04 |
| [MAL-2026-11889](https://osv.dev/vulnerability/MAL-2026-11889) | @servicetitan/log-service | finder | 2026-08-04 |
| [MAL-2026-11944](https://osv.dev/vulnerability/MAL-2026-11944) | @servicetitan/tokens | finder | 2026-08-04 |
| [MAL-2026-11949](https://osv.dev/vulnerability/MAL-2026-11949) | @servicetitan/web-components | finder | 2026-08-04 |
| [MAL-2026-11977](https://osv.dev/vulnerability/MAL-2026-11977) | picasso-plugin-hammer | finder | 2026-08-04 |
| [MAL-2026-11978](https://osv.dev/vulnerability/MAL-2026-11978) | picasso-plugin-q | finder | 2026-08-04 |
| [MAL-2026-11979](https://osv.dev/vulnerability/MAL-2026-11979) | picasso.js | finder | 2026-08-04 |
| [MAL-2026-18100](https://osv.dev/vulnerability/MAL-2026-18100) | unicode-title-normalizer | analyst | 2026-10-20 |
| [MAL-2026-18358](https://osv.dev/vulnerability/MAL-2026-18358) | @testsecuiitytestme/cache-helper | analyst | 2026-10-29 |
| [MAL-2026-18369](https://osv.dev/vulnerability/MAL-2026-18369) | mui-wrapper-x-date-pickers | analyst | 2026-10-29 |
| [MAL-2026-18370](https://osv.dev/vulnerability/MAL-2026-18370) | mw-communication-client | analyst | 2026-10-29 |
| [MAL-2026-18371](https://osv.dev/vulnerability/MAL-2026-18371) | mw-test-utils | analyst | 2026-10-29 |
