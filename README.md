# solana-gif-portal
Build space project for learning solana

## Useful commands

### Check install version

+ Rust`rustup --version`

+ Rust compiler `rustc --version`

+ Cargo (rust package manager) `cargo --version`

+ Anchor (tool for running and depolying solana programs) `anchor --version`

+ Solana `solana --version`

### Solana talk to local network
`solana config set --url localhost`
`solana config get`

Run solana validator locally
`solana-test-validator --no-bpf-jit`

Make a boilterplate project
`anchor init myepicproject --javascript`

Create a local keypair
`solana-keygen new -o target/deploy/myepicproject-keypair.json`

Get public key fro a local key pair
`solana address -k target/deploy/myepicproject-keypair.json`

Run tests and skip local validator (for Mac M1)
`anchor test --skip-local-validator`

### Solana talk to devnet

Switch to dev net
`solana config set --url devnet`

Create a new build with program id
` create a new build for us with a program id.`

Get the program id
`solana address -k target/deploy/myepicproject-keypair.json`

Deploy
`anchor deploy`

Test
`anchor test`
