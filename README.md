# resource-agents.saphanasr-angi

[![Shellcheck](https://github.com/redhat-sap/resource-agents.saphanasr-angi/actions/workflows/shellcheck.yml/badge.svg)](https://github.com/redhat-sap/resource-agents.saphanasr-angi/actions/workflows/shellcheck.yml)
[![Pylint](https://github.com/redhat-sap/resource-agents.saphanasr-angi/actions/workflows/pylint.yml/badge.svg)](https://github.com/redhat-sap/resource-agents.saphanasr-angi/actions/workflows/pylint.yml)
[![Mandoc](https://github.com/redhat-sap/resource-agents.saphanasr-angi/actions/workflows/mandoc.yml/badge.svg)](https://github.com/redhat-sap/resource-agents.saphanasr-angi/actions/workflows/mandoc.yml)

Red Hat maintained fork of the SAP HANA System Replication Pacemaker resource agents and hook scripts - angi generation, covering scale-up and scale-out topologies. Packaging source for the `sap-hana-ha` RPM.

Forked from [SUSE/SAPHanaSR](https://github.com/SUSE/SAPHanaSR) (`main` branch) on 2026-07-23 under GPL-2.0-or-later. Independently maintained since.

---

## Repository layout

```
ra/             OCF resource agents and shared libraries
hooks/          HA/DR provider hooks (configured in SAP HANA global.ini)
hooks/samples/  global.ini configuration examples for each hook
alerts/         Pacemaker alert agents
tools/          Cluster monitoring and management utilities
man/            Manual pages
```

---

## How to use this repository

This repository is a **packaging source**, not a deployable package. It does not provide RPM spec files or installation scripts. Packaging decisions (which files to ship, installation paths, package dependencies) are made at the packaging layer.

---

## Differences from the fork origin

Changes since forking are tracked in [`CHANGELOG.md`](CHANGELOG.md).

---

## Disclaimer

This repository is a fork of [SUSE/SAPHanaSR](https://github.com/SUSE/SAPHanaSR) maintained for RHEL packaging purposes. It does not replace official SAP documentation for SAP HANA System Replication HA cluster setup and operation.

**Testing coverage:** Static analysis (shellcheck, pylint, mandoc) is applied via CI on every commit. Functional HA testing - cluster behaviour, fencing, takeover sequences - is the responsibility of the distribution packaging and validation process.

Use at your own responsibility.

---

## Contributing

Contributions are welcome. Please open an issue to discuss changes or submit a pull request.

---

## License

[GPL-2.0-or-later](./LICENSE) - original work copyright SUSE LLC under the same license.
