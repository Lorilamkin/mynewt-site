## <font color="#F2853F" style="font-size:24pt">ble\_hs\_mbuf\_att\_pkt</font>

```c
struct os_mbuf *
ble_hs_mbuf_att_pkt(void)
```

### Description

Allocates an mbuf suitable for an ATT command packet.  The resulting packet has sufficient leading space for: <ul><li>ACL data header</li> <li>L2CAP B-frame header</li> <li>Largest ATT command base (prepare write request / response).</li></ul>

### Parameters

None

### Returned values

| *Value* | *Condition* |
|---------|-------------|
| An empty mbuf | Success. |
| null | Memory exhaustion. |
