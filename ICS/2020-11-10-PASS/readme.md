- 出题人: r0fus0d
- 难度: 简单
- 考点: S7Comm 协议
- 解法:

    从流量包中找到 S7 密码密文, 解 S7 密码
    ```
    0x6d ^ 0x55 = 0x38
    0x6d ^ 0x55 = 0x38
    0x00 ^ 0x55 ^ 0x6d = 0x38
    0x0d ^ 0x55 ^ 0x6d = 0x35
    0x60 ^ 0x55 ^ 0x00 = 0x35
    0x6d ^ 0x55 ^ 0x0d = 0x35
    0x15 ^ 0x55 ^ 0x60 = 0x20
    0x18 ^ 0x55 ^ 0x6d = 0x20
    ```

- flag: flag{888555}
- 注意点: 无