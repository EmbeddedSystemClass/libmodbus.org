---
title: libmodbus v3.1.4
published: 2016-05-28
tags: [release]
summary: Small fixes, Cygwin improvements and fix missing script in tarball
---

- `C_PROG_RANLIB` is rendered obsolete by LT_INIT
- Improve ifdef around bswap_16 for `__CYGWIN__`
- Improve Cygwin support. Thanks to StalderT.
- Another round of DRY in `modbus_reply()`
- Rename raw_rep to raw_rsp in unit-test-client
- Fix wrong function name in debug message
- Fix handling of invalid function code (closes #315)
- Add debug message on unknown function and new unit test
- DRY in modbus_reply by improving `response_exception()`
- Fix typo in 3053bd0adb
- CID 69145 - Argument cannot be negative in unit-test-server
- CID 69142 - Unchecked return value in unit-test-server
- Fix CID 69140 - Bad bit shift operation (coverity) in tests
- Rewrite and rename README as `README.md` in tests/
- Github's contributing and issue template files
- Fix small leak (64 bytes in TCP) in unit-test-client
- Add unit-tests.sh to tarball
- Add ./configure.scan to .gitignore
- Move setting of option inside the relevant conditional group
- Add links to new `modbus_*_float_*` functions in index
- Slight change to `modbus_report_slave_id` doc.
