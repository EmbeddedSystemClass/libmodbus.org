---
title: Stable and development releases
published: 2019-07-29
tags: [release]
summary: Many changes with fixes for vulnerabilities
---

**libmodbus 3.0.7 (2019-07-29)**

libmodbus v3.0.x branch has been updated to include important fixes backported from v3.1.7.

- Fix VD-1301 and VD-1302 vulnerabilities
- Move WINVER definition before other includes (closes #350)
- Replace signed int by unsigned

**libmodbus 3.1.5 (2019-07-29)**

- Add appveyor.com config
- Change arg value from int to const uint16_t in modbus_write_register
- Mark raw_req argument as const in modbus_send_raw_request (closes #479)
- Add unit tests for VD-1301 and VD-1302 vulnerabilities
- Fix VD-1301 and VD-1302 vulnerabilities
- Create CODE_OF_CONDUCT.md
- modbus_mapping_t is now a named typedef (to allow forward declaration)
- Rename type as flags for consistency between functions
- Add missing SOCK_CLOEXEC flag on socket creation
- Remove wrong and harmful checks in configure.ac
- Oops fix OR on RS485 settings (1c5d969)
- Only set SER_RS485_ENABLED bit of existing RS485 settings
- Add .vscode/ to .gitignore
- Fix wrong function name
- Remove a duplicated semi-colon
- Fix a small typo in test message
- Fix modbus_reply for TCP when unit id == 0 (fixes #376)
- New functions to define the indication timeout (#95)
- Remove CYGWIN condition to provide bswap16 fallback (#383)
- typo fix
- Use builtin bswap16 of gcc 4.8 (#377)
- Handle out-of-memory conditions more gracefully
- [doc] Add entry points for accept/listen in libmodbus index
- Fix typo
- Refine issue template for Github
- Move WINVER definition before other includes (#350)
- Add new function modbus_get_slave()
- Fix LIBMODBUS_VERSION_HEX encoding (closes #345)
- tcp_modbus_accept mustn't close socket on error (closes #333)
