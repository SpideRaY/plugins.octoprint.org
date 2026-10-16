---

layout: plugin

id: tapoautoshutdown
title: Tapo Auto Shutdown + Obico Delay
description: Automatically control two compatible TP-Link Tapo smart plugs and manage Obico AI monitoring around your prints.

authors:
- SpideRaY

license: MIT

date: 2026-10-14

homepage: https://github.com/SpideRaY/OctoPrint-TapoAutoShutdown-ObicoDelay
source: https://github.com/SpideRaY/OctoPrint-TapoAutoShutdown-ObicoDelay/tree/v0.3.0
archive: https://github.com/SpideRaY/OctoPrint-TapoAutoShutdown-ObicoDelay/archive/refs/tags/v0.3.0.zip
privacyPolicy: https://github.com/SpideRaY/OctoPrint-TapoAutoShutdown-ObicoDelay/blob/v0.3.0/PRIVACY.md

tags:

- tapo
- p110
- smart plug
- power
- shutdown
- obico
- ai
- automation
- print monitoring

compatibility:
  python: “>=3.11,<4”

attributes:

- cloud
- ai-developed

---

Tapo Auto Shutdown automatically controls two compatible TP-Link Tapo smart plugs: one for the 3D printer and an optional separate plug for the OctoPi Raspberry Pi. After a completed print, the plugin manages printer shutdown and can shut down the Raspberry Pi cleanly before switching off its plug.

The plugin provides configurable delays for both Tapo shutdown and Obico AI monitoring. Obico AI monitoring is disabled when a print starts and can be automatically re-enabled after the configured delay if the print is still running.

If the print completes, is cancelled, or fails, the Obico monitoring timer is cancelled and AI monitoring is disabled.

The plugin requires an OctoPrint installation, at least one compatible Tapo smart plug, the Tapo Python package, and the Obico OctoPrint plugin for Obico monitoring features.

The plugin does not modify the printer’s operating system or install system services.

For more information, configuration details and source code, see the project repository.
