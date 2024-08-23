## !intro ERC-20 Explainer

ERC-20 (Ethereum Request for Comment 20) is a technical standard for fungible tokens on the Ethereum blockchain. It defines a common set of rules that all Ethereum-based tokens must follow, allowing for seamless integration with various wallets, exchanges, and smart contracts.

Key features of ERC-20 tokens include:
- A standard set of functions that enable token transfers and balance checks
- Consistent behavior across different implementations
- Interoperability with other ERC-20 compliant tokens and applications

The importance of ERC-20 lies in its:
1. Standardization: It provides a uniform way to create and interact with tokens on Ethereum
2. Interoperability: ERC-20 tokens can easily be exchanged and used across various platforms
3. Simplification: It reduces the complexity of implementing new tokens and integrating them into existing systems
4. Liquidity: The standard has facilitated the creation of numerous tokens, contributing to the growth of the cryptocurrency ecosystem

ERC-20 has become the foundation for many cryptocurrency projects, Initial Coin Offerings (ICOs), and decentralized finance (DeFi) applications, playing a crucial role in the expansion of the Ethereum ecosystem and the broader blockchain industry.

The ERC-20 interface defines a set of standard functions that every ERC-20 token must implement. These functions allow for seamless interaction with the token across various platforms and applications. The basic ERC-20 interface includes:

This standardized interface ensures that all ERC-20 tokens behave consistently, facilitating their integration into various applications and exchanges.

## !!steps Total Supply

The `totalSupply()` function is a crucial part of the ERC-20 standard, which returns the total number of tokens in circulation. This function:

- Provides transparency about the token's supply
- Helps users and investors understand the token's scarcity or abundance
- Is typically implemented as a public variable that can be queried at any time
- May be fixed or variable, depending on the token's issuance model

By exposing the total supply, this function enables users to calculate market capitalization and assess the token's overall distribution. It's an essential metric for token economics and often plays a role in investment decisions.

```js ! IERC20.sol
// Example taken from: https://solidity-by-example.org/app/erc20/
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.24;

interface IERC20 {
    function totalSupply() external view returns (uint256);
}
```

## !!steps Balance off

The `balanceOf(address account)` function is another essential part of the ERC-20 standard. This function:

- Returns the current balance of tokens for a specified address
- Allows users to check their own token balance or the balance of any other address
- Is typically implemented as a mapping of addresses to balances
- Helps in verifying token ownership and facilitating transfers

This function is crucial for token holders to manage their assets and for applications to display accurate balance information. It's commonly used in wallet interfaces, exchanges, and other DeFi applications to show users their current token holdings.


```js ! IERC20.sol
// Example taken from: https://solidity-by-example.org/app/erc20/
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.24;

interface IERC20 {
    function totalSupply() external view returns (uint256);
    function balanceOf(address account) external view returns (uint256);
}
```

## !outro

Quisque id pretium neque. Vestibulum metus orci, pretium nec varius convallis, viverra quis urna. Praesent luctus, purus nec tempus placerat, justo lorem auctor ligula, ut condimentum tellus velit ac erat. Fusce ut dictum libero. Vestibulum ipsum mauris, cursus sed tortor at, rhoncus viverra ipsum. Donec odio dolor, varius quis congue posuere, tempor et justo. Praesent at scelerisque metus. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Sed malesuada leo vitae mauris eleifend condimentum. Proin auctor, ex ac aliquam gravida, felis felis lacinia libero, efficitur aliquet nulla neque sed elit. Vestibulum congue aliquam risus, sit amet rutrum magna euismod ac. Integer posuere neque nec ex sollicitudin rhoncus.
