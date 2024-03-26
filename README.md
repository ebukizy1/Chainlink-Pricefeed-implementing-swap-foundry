

## Overview:
This Solidity smart contract named SwapContract facilitates decentralized swaps between different ERC-20 tokens and provides price feeds using Chainlink oracles. Users can exchange Ethereum (ETH) for Dai (DAI), Ethereum for Chainlink (LINK), Dai for Chainlink, Chainlink for Dai, Dai for Ethereum, and Chainlink for Ethereum.

## Features:
Swapping Functionality:

Users can exchange Ethereum, Dai, and Chainlink tokens with each other using the defined swap functions.
Each swap function specifies the tokens being swapped and verifies the balances before executing the swap.
Events are emitted upon successful swaps.
## Price Feeds:

The contract fetches price data from external Chainlink oracles for Ethereum, Dai, and Chainlink tokens.
Price feeds are used to determine the exchange rates between tokens for accurate swaps.
## Decentralized Execution:

The contract is deployed on the Ethereum blockchain, enabling decentralized and trustless token swaps without relying on intermediaries.
Token Support and Oracles:
## Supported Tokens:

Ethereum (ETH)
Dai (DAI)
Chainlink (LINK)
## Chainlink Oracles:

Ethereum to USD Price Feed: AggregatorV3Interface eth_usd
Dai to USD Price Feed: AggregatorV3Interface dai_usd
Chainlink to USD Price Feed: AggregatorV3Interface link_usd
## Usage:
Deployed Contract Address: 0x8527c7280a0D7c3B9a3fC9Fc016203ed507702Bd
Deployer Address: 0x3fb7B6793bF753E74bf776ff386256a7FD9F7bee
## Functions:
## Swap Functions:

swapEthDai(uint256 _amountA) external: Swaps Ethereum for Dai.
swapEthLink(uint256 _amountA) external: Swaps Ethereum for Chainlink.
swapLinkDai(uint256 _amountA) external: Swaps Chainlink for Dai.
swapLinkEth(uint256 _amountA) external: Swaps Chainlink for Ethereum.
swapDaiLink(uint256 _amountA) external: Swaps Dai for Chainlink.
swapDaiEth(uint256 _amountA) external: Swaps Dai for Ethereum.
## Helper Functions:

getDerivedPrice: Retrieves derived price based on provided Chainlink oracles.
scalePrice: Scales price based on decimals for accurate calculations.
## Security Considerations:
Ensure that the caller has sufficient balance before initiating a swap.
Verify the token addresses and oracles to prevent unauthorized actions.
Exercise caution when interacting with smart contracts, as transactions cannot be reversed once confirmed.
## Deployment Information:
Transaction Hash: 0xd540004947688429170303697f2df1dc8a5d8c38f6f6a4688ca784eed34ababd
Verified Contract Address:
Contract Address: 0x8527c7280a0D7c3B9a3fC9Fc016203ed507702Bd