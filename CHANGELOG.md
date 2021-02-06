# Changelog

## [Unreleased][unreleased]

- Don't inject Channel to Server
- Changed Server.constructor signature from
  `(config, { Channel, application })` to `(config, application)`
  so should be published with new version of metacom, see:
  https://github.com/metarhia/metacom/issues/127

## [2.0.4][] - 2021-02-04

- Load TLS certificates only if we need HTTPS or WSS
- Move hashPassword and validatePassword to metautil
- Move cookies operations to metacom

## [2.0.3][] - 2021-01-29

- Fixed exception handling in module loader
- Added relative path in logged stack traces
- Fixed application initializtion flag
- Catch exceptions in application initialization

## [2.0.2][] - 2021-01-26

- Move utils to metautil
- Implement schemas for structures and scalars
- Fixed path separators to support windows

## [2.0.1][] - 2021-01-09

- Use metautil instead of metarhia/common for core utilities
- Fixed spelling in function name: nkdirp -> mkdirp

## [2.0.0][] - 2020-12-21

- Single application with code live reload and auto API routing
- Graceful shutdown and application state recovery after reload
- Minimum code size and dependencies
- Scale with threads with code sandboxing, DI and context isolation
- Inter-process communication and shared memory used for state management
- Support protocols: HTTP, HTTPS, WS, WSS, Metacom with REST and RPC
- Support logging, configuration, task scheduling
- Database access layer for PostgreSQL with migrations and query builder
- Persistent sessions support with authentication, groups and anonymous
- Request queue with timeout and size, execution timeout and error handling

## [1.0.9][] - 2019-01-18

First generation of application server with following features

- Support multiple applications and sites with sandboxing and auto-reload
- Serve multiple domains, ports, network interfaces, hosts and protocols
- Scale with processes with IPC
- Support protocols: JSTP, TCP, UDP, WS, WSS, HTTP, HTTPS with REST or RPC
- Built-in auth subsystem with sessions
- Support logging, configuration, file upload and download, reverse-proxy
- Connection drivers for database engines: MongoDB, PgSQL, Oracle, MySQL
- Support GeoIP, health monitoring, task scheduling, server-side templating

[unreleased]: https://github.com/metarhia/impress/compare/v2.0.4...HEAD
[2.0.4]: https://github.com/metarhia/impress/compare/v2.0.3...v2.0.4
[2.0.3]: https://github.com/metarhia/impress/compare/v2.0.2...v2.0.3
[2.0.2]: https://github.com/metarhia/impress/compare/v2.0.1...v2.0.2
[2.0.1]: https://github.com/metarhia/impress/compare/v2.0.0...v2.0.1
[2.0.0]: https://github.com/metarhia/impress/compare/v1.0.9...v2.0.0
[1.0.9]: https://github.com/metarhia/impress/releases/tag/v1.0.9