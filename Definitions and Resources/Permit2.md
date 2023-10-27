Repository:
https://github.com/Uniswap/permit2

### Permit2 - Efficient, consistent, and secure approvals 
Permit2 is a token approval contract that can safely share and manage token approvals across different smart contracts. As more projects integrate with Permit2, we can standardize token approvals across all applications. In turn, Permit2 will improve the user experience by reducing transaction costs while improving smart contract security. Originally defined in [[EIP-20]], the canonical token approve method suffered from a couple of weaknesses: 

- Users had to send an approval transaction for each new application they wanted to use. This led to a confusing UX where users might be asked to send multiple transactions before using an application, wasting gas and time. 

- For convenience's sake, applications asked users to approve the maximum allowance, giving applications access to a wallet’s entire token balance for an indefinite amount of time. Though Uniswap has never suffered from an exploit, infinite approvals can be hacked to steal user tokens. (PSA to revoke active allowances.) 

[[EIP-2612]] iterated on token approvals. Users could interact with application contracts without requiring prior approval by appending a signed permit message to their transaction. While EIP-2612 made token approves safer with granular allowance approvals, tokens launched before EIP-2612 did not support the permit function and not all newer tokens have adopted it. 