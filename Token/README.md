Rust Install

curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh

rustup --version
rustc --version
cargo --version

Solana SetUp
https://github.com/LearnWithArjun/solana-env-setup/blob/main/mac_or_linux_setup.md

Solana --version
# Set the connection URL for the Solana client to localhost.
solana config set --url localhost

# Retrieve the current configuration information
solana config get

# Set up a validator on our computer to test our programs
solana-test-validator
(Keep open when using)

# Install Mocha to help us test our Solana programs
npm install -g mocha

# Install Anchor - a tool for us to run Solana programs locally and deploy them to the actual Solana chain when we're ready
cargo install --git https://github.com/project-serum/anchor anchor-cli --locked

anchor --version

# Install Anchor's npm module and Solana Web3 JS
npm install @project-serum/anchor @solana/web3.js
cargo install --git https://github.com/project-serum/anchor anchor-cli --locked

brew install yarn

anchor init myepicproject --javascript
cd myepicproject

anchor init myepicproject --javascript
cd myepicproject

# Create a local keypair
solana-keygen new 
solana-keygen new --force(This option forces the generation of a new keypair and overwrites any existing keypair files if they exist.)

# Check Keypair
solana address

# Compile/Deploy/Run
anchor test
solana address

solana balance --url devnet

# Or visit this website to check balance
# Visit and switch to Devnet
https://explorer.solana.com/address/HkyJaL5AjSA2G3DkQbfTSKpyzgQEorPRfKQHeGKZcbDW

# Search for public key
HkyJaL5AjSA2G3DkQbfTSKpyzgQEorPRfKQHeGKZcbDW

# Get Airdrop (solana airdrop (token_amount) (public_key))
solana airdrop 2 HkyJaL5AjSA2G3DkQbfTSKpyzgQEorPRfKQHeGKZcbDW





---------------------------------------------------
# Solana Program Library
https://spl.solana.com/token
cargo install spl-token-cli

# Create token
spl-token create-token --url devnet
Get token address: E1YuEbASJP3Hic17oiDyyoYVGh1XAAGTt4wz1yfCauXr

# Create account
spl-token create-account E1YuEbASJP3Hic17oiDyyoYVGh1XAAGTt4wz1yfCauXr
Get token account address: 2mrLeLwdjMKq4dv3F9FVpMxPFQ7hqnShTVSa4sumxc9Z

# Check balance
spl-token balance E1YuEbASJP3Hic17oiDyyoYVGh1XAAGTt4wz1yfCauXr

# Mint
spl-token mint

# View all Tokens that you own
spl-token accounts
