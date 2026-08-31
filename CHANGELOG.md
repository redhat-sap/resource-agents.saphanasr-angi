# Changelog

Format based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## 2026-07-23

Forked from SUSE/SAPHanaSR main branch at commit 9ca24b18.

### Added

* CI: shellcheck, pylint, mandoc enforce results

### Changed

* **hooks:** sus* prefix stripped from class names, INI sections, and trace file references
* **hooks:** provider_company set to Red Hat
* **hooks:** install paths changed from SAPHanaSR-angi to sap-hana-ha
* **ra:** .suse_SAPHanaFilesystem replaced with .heartbeat_SAPHanaFilesystem
* **ra:** install paths changed from SAPHanaSR-angi to sap-hana-ha
* **repo:** srHook/ renamed to hooks/, alert/ renamed to alerts/
* **repo:** global.ini samples moved to hooks/samples/

### Removed

* SUSE-specific packaging, deployment tooling, UI components, and man pages
* CostOpt hook (not shipped in sap-hana-ha)
* Perl linter configs (no Perl code in repo)
