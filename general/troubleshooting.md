# Troubleshooting

Here are the common errors new developers encounter, and their solutions.
If you don't find the error you are looking for, you can [Open An ISSUE](https://github.com/Setheum-Labs/setheum-wiki/issues/new).

### Blocking waiting for file lock on build directory
This is quite common you are building
First of all, running `cargo clean` seems to fix the problem, and then if it doesn't you can try `~/.cargo/package-cache`.

### FATAL: Unable to initialize the API: createType(CurrencyId):: Cannot construct unknown type CurrencyId

You are missing the [types.json](https://github.com/Setheum-Labs/Setheum/blob/master/resources/types.json) file in the developer settings of the console. Make sure you get the correct file for [your node version](https://github.com/Setheum-Labs/Setheum/tags).

### Error: Service(Keystore(Io(Os { code: 13, kind: PermissionDenied, message: “Permission denied” })))

Make sure `--base-path` is set to a folder you have appropriate permissions for. Either update the permissions of your account to access `/setheum/validator` (documentation default) or change `--base-path` to somewhere else (ie. your home folder).

### No Polkadot.js extension found

You could be getting this error because you haven't installed the polkadot.js browser extension. If you haven't, you can do so [here](https://polkadot.js.org/extension/). And make sure your extension is set to `allow use on any chain`. Then go to `Settings >> Manage Website Access` in the extension and make sure that `setheum.xyz` is allowed.

### 1010: Invalid Transaction: Transaction has a bad signature

This means that the signature that is generated for the transaction payload is not recognizable by the RPC node.
Refresh the app and accept the metadata update. Then Refresh the app again.
For best experience, update metadata.

### 1010: Invalid Transaction: Inability to pay some fees, e.g. account balance too low

The amount you are trying to transact may be too much. Try using a little less and reinitiating the transaction. You could be trying to pay your transaction fees with a token that is not supported. Only tokens that are traded on the DEX (SetSwap) can be used to pay transaction fees. If you switch to pay your fee with a supported token, your transaction should process.
### Weird database errors

Whenever you run into some sort of database error, `purge-cache` subcommand is your friend. You can do a fresh sync after the purge, and things should just work.
