# Sign scripts

## Commands

```bash
yarn cli swap USDT 0.1 GET
```

4 subcommands are available:

- `add` | `remove` | `swap`: create DEX tx, then sign & submit
- `sign`: given cbor and txId, sign and submit tx
  - Used when you create DEX tx yourself (in Postman for example) and want to
    sign it

## Environment

| Env var          | Meaning                                                                                  |
| ---------------- | ---------------------------------------------------------------------------------------- |
| `BRIDGE_ADDRESS` | [`BridgeAbi`][1] address, [`0xF24fc4c27a8E2F3910313FA8F764CdB881Dc99F6`][2] in preprod   |
| `USDT_ADDRESS`   | [USDT contract][1] address, [`0xF8ebaA46911e01582b7dEcae1A8b91174A6e782C`][3] in preprod |

Also, you need a 15-word seedphrase, and Blockfrost & Alchemy API key.

[1]: ./src/bridge.ts
[2]: https://sepolia.etherscan.io/address/0xF24fc4c27a8E2F3910313FA8F764CdB881Dc99F6
[3]: https://sepolia.etherscan.io/address/0xF8ebaA46911e01582b7dEcae1A8b91174A6e782C
