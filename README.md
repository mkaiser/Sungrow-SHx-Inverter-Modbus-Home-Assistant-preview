# Sungrow Modbus — preview channel

> **A distribution copy. Do not open issues here.**

This repository exists so that HACS can install a **preview** of the
Sungrow Modbus integration. HACS reads a repository's default branch
unless it finds a stable release, and the real repository's default
branch is its long-standing YAML package — so HACS cannot install
from there. This repository's default branch is the integration.

Currently carrying **v0.1.0a1**, copied automatically from
[mkaiser/Sungrow-SHx-Inverter-Modbus-Home-Assistant](https://github.com/mkaiser/Sungrow-SHx-Inverter-Modbus-Home-Assistant).

- **Issues, discussions and pull requests:**
  [mkaiser/Sungrow-SHx-Inverter-Modbus-Home-Assistant](https://github.com/mkaiser/Sungrow-SHx-Inverter-Modbus-Home-Assistant/issues)
- **What this is, what works and what does not:**
  [the real README](https://github.com/mkaiser/Sungrow-SHx-Inverter-Modbus-Home-Assistant/tree/proper-ha-integration)
- **Installing without HACS:**
  [doc/installing_a_preview.md](https://github.com/mkaiser/Sungrow-SHx-Inverter-Modbus-Home-Assistant/blob/proper-ha-integration/doc/installing_a_preview.md)

## Install

**HACS → three dots → Custom repositories**, this repository's URL,
category **Integration**. Then download it, restart Home Assistant,
and add **Sungrow Modbus (preview)** under Settings → Devices &
services.

HACS will show a commit hash rather than a version number, because
this repository publishes no releases of its own. The integration
reports its real version — `v0.1.0a1` — in its own name and under
Settings → Repairs.

## It is a preview

Registers can move and entity ids can change. If you want something
finished, use the **YAML package** on the real repository's default
branch: five years old, and in use by thousands of people.

The most useful thing you can do with it is send a reading. The
integration can produce one for you: add it in **Diagnostics only**
mode if you do not want any entities, fill in
**Options → Help this project**, and download the diagnostics.

## When this repository goes away

The integration is meant to replace the YAML package. When it
reaches the real repository's default branch, this one is archived —
and at that point:

**Remove this repository from HACS before installing from the real
one.** Both provide the same integration at the same path, so
keeping both is a conflict rather than an upgrade.
