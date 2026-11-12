# Upstream attribution, dependencies and licensing

This repository adapts existing open-source projects. It should not be
represented as a wholly original implementation of Tailscale, WireGuard or
Wake-on-LAN on ESP32.

## Original project

- **[medinajaime/esp32-wakeonlan](https://github.com/medinajaime/esp32-wakeonlan)**
  — upstream ESP32 Tailscale + WireGuard + Wake-on-LAN application, configuration,
  Windows/Linux setup scripts and baseline documentation.
- Original project author/maintainer is identified by the GitHub account
  **medinajaime**. Consult the upstream contributor history for other
  contributors rather than assuming that a single person wrote every file.
- The upstream README describes the project license as **MIT**. Before public
  redistribution, check the full license notices and Git history in the exact
  revision being used and retain all applicable copyright notices.

## WireGuard/lwIP implementation

- **[smartalock/wireguard-lwip](https://github.com/smartalock/wireguard-lwip)**
  — embedded WireGuard implementation for lwIP by **Daniel Hope**.
- Its source identifies a **BSD 3-Clause** notice; preserve the existing
  notice in source and comply with redistribution terms. The source module
  in this adaptation is modified for lifecycle integration, not authored
  from scratch.
- WireGuard was originally developed by **Jason A. Donenfeld**; the WireGuard
  name and mark are associated with that project. This repository is not
  officially endorsed by WireGuard or Tailscale.

## My adaptation and development process

I selected the ESP32-WROOM-32D hardware and the Proxmox integration architecture, configured the development and network environment, reviewed test results and maintained this adaptation. I used ChatGPT and GitHub Copilot for code review, candidate fixes and documentation. The implementation incorporates upstream software and AI-assisted changes; I do not represent those dependencies as code I originally authored.

The build, flash and end-to-end results supported by the recorded tests are listed in [VALIDATION_AND_LIMITATIONS.md](VALIDATION_AND_LIMITATIONS.md). Tests that were not performed or do not establish security or endurance are identified separately.

See [CHANGES_FROM_UPSTREAM.md](CHANGES_FROM_UPSTREAM.md) for the changes retained
in the validated local code. Credit does not imply the original developers
reviewed, approved or endorsed these patches.
