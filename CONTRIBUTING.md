# Contributing to bitEngine projects

Thanks for taking the time. These guidelines apply to every repository in the bitEngineTech
organization unless a repository says otherwise.

## Before the source release

Until the firmware source lands (planned November 2026), the most useful contributions are:

- **Feedback on the design and documentation** — open an issue in the repository it concerns, or
  reply in the [Home Assistant Community thread](https://community.home-assistant.io/t/1028644).
- **Integration reports** — which Home Assistant, ZHA or Zigbee2MQTT versions you run, and what
  you would need from the hub.

## Issues

- Use the issue tracker of the repository the problem belongs to (firmware, Zigbee NCP,
  hardware). If unsure, use the firmware repository.
- For a bug, include the hub firmware version, the Home Assistant / ZHA / Zigbee2MQTT versions,
  and what you expected versus what happened. Logs help; please strip network keys and
  credentials before posting.
- Security issues go through [SECURITY.md](SECURITY.md), not the public tracker.

## Pull requests

- Open an issue first for anything beyond a small fix, so the change can be discussed before you
  spend time on it.
- Keep a pull request to one topic. Describe what it changes and why, and how you tested it (on
  which hardware, with which Home Assistant setup).
- Follow the style of the surrounding code; build instructions and any formatting tooling are in
  each repository's README.

## Licensing of contributions

By submitting a contribution you agree that it is provided under the license of the repository
you submit it to:

- Firmware repositories: Apache License 2.0. As set out in section 5 of that license, any
  contribution intentionally submitted for inclusion is licensed under Apache-2.0 without
  additional terms.
- Hardware repository: CERN-OHL-P-2.0.

Do not submit material you do not have the right to license this way — in particular, nothing
from the Silicon Labs SDK or other proprietary sources.

## Conduct

Be respectful and constructive. Disagreement about technical choices is welcome; personal
attacks are not. Maintainers may edit or remove content that does not meet this bar.
