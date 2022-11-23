# NftTransfer

A sender account, a receiver account, and the serial number of an NFT of a Token with `NON_FUNGIBLE_UNIQUE` type.

| Field               | Type                                                                                                                                       | Description                                                                                                                                            |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `senderAccountID`   | [AccountID](https://github.com/theekrystallee/hedera-style-guide/blob/sdk-v1/deprecated/hedera-api/basic-types/broken-reference/README.md) | The accountID of the sender                                                                                                                            |
| `receiverAccountID` | [AccountID](https://github.com/theekrystallee/hedera-style-guide/blob/sdk-v1/deprecated/hedera-api/basic-types/broken-reference/README.md) | The accountID of the receiver                                                                                                                          |
| `serialNumber`      | int64                                                                                                                                      | The serial number of the NFT                                                                                                                           |
| `is_approval`       | bool                                                                                                                                       | If true then the transfer is expected to be an approved allowance and the senderAccountID is expected to be the owner. The default is false (omitted). |