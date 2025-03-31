# zKrypt
zero-knowledge wallet sdk

1 - OAuth Login Simulation:

The simulateOAuthLogin function simulates fetching an OAuth token and user ID from an OAuth provider (e.g., Google).

2 - Private Key Derivation:

The derivePrivateKey function combines the OAuth token, user ID, and a client-side salt to create a deterministic private key using a cryptographic hash function (keccak256).

3 - Wallet Creation:

The createWallet function creates an Ethereum wallet using the derived private key.

4 - Transaction Signing:

The signTransaction function signs a transaction using the wallet's private key. This happens entirely on the client side.

5 - Client-Side Key Management:

The private key is never sent to or stored on the server. It is derived and used exclusively on the client side.
