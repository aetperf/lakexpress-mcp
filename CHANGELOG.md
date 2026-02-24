# Changelog

All notable changes to the LakeXpress MCP Server will be documented in this file.

## [0.1.3] - 2026-02-24

### Added
- PyPI, License, and MCP Registry badges in README
- GitHub Actions workflow for automated PyPI publishing on release
- Missing environment variables (`LAKEXPRESS_LOG_DIR`, `LOG_LEVEL`) in server.json
- GitHub repository topics for MCP Registry discoverability

### Fixed
- Timeout default in server.json (corrected from 1800 to 3600 to match actual code)
- Documentation URL in pyproject.toml

## [0.1.1] - 2026-02-23

### Added

- `server.json` MCP Registry configuration file with package metadata, transport settings, and environment variable definitions

### Changed

- GitHub repository URL updated from `aetperf/lakexpress-mcp` to `arpe-io/lakexpress-mcp` in `pyproject.toml`


## [0.1.0] - 2026-02-20

### Added
- Initial release of LakeXpress MCP Server
- 6 MCP tools: preview_command, execute_command, validate_auth_file, list_capabilities, suggest_workflow, get_version
- Support for all 14 LakeXpress subcommands: logdb (init/drop/truncate/locks/release-locks), config (create/delete/list), sync, sync[export], sync[publish], run, status, cleanup
- Version detection and capabilities registry for LakeXpress v0.2.8
- Comprehensive input validation with Pydantic models
- Command builder with proper CLI argument construction
- Execution logging with configurable log directory
- Auth file validation tool
- Workflow suggestion engine
