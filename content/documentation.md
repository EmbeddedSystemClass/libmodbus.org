---
title: "Documentation"
date: "2019-07-29"
---

The documentation is provided with libmodbus releases as man pages (generated from [doc sources](https://github.com/stephane/libmodbus/tree/master/doc). You can also browse the documentation of the different releases of libmodbus:

- [v{{< devversion >}}](/docs/v{{< devversion >}})
- [v{{< stableversion >}}]](/docs/v{{< stableversion >}}])

See the [Wiki](https://github.com/stephane/libmodbus/wiki/) for general informations.

## Code Sample

{{< highlight c >}}
#include <stdio.h>
#include <modbus.h>

int main(void) {
  modbus_t *mb;
  uint16_t tab_reg[32];

  mb = modbus_new_tcp("127.0.0.1", 1502);
  modbus_connect(mb);

  /* Read 5 registers from the address 0 */
  modbus_read_registers(mb, 0, 5, tab_reg);

  modbus_close(mb);
  modbus_free(mb);
}
{{< /highlight >}}

## External Documentation

- [Modbus Specifications and Implementation Guides](http://www.modbus.org/specs.php)
- [Wikipedia page of Modbus](http://en.wikipedia.org/wiki/Modbus)
