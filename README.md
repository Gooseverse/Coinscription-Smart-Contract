Coinscription Smart Contract

Description

The Coinscription Smart Contract is designed to facilitate the depositing of Ethscriptions and the creation of wrapped addresses for Ethereum wallet addresses. This contract allows users to deposit Ethscriptions, and in return, they receive a wrapped address that can be used for payments through the coinscription.com website.

Features

Deposit Ethscriptions and receive a wrapped address.
Easily interact with the smart contract to create wrapped addresses.
Seamless integration with the coinscription.com website for payments.
Getting Started

Clone the repository:
git clone https://github.com/your-username/coinscription-smart-contract.git

Install the required dependencies (if any).
Deploy the CoinscriptionSmartContract.sol using your preferred Ethereum development environment or a testnet.
Usage

Deposit Ethscription
To deposit an Ethscription, call the depositEthscription function with the desired Ethscription URI.
function depositEthscription(string memory ethscriptionURI) external;
Create Wrapped Address
The contract will automatically create a wrapped address for the Ethereum wallet address that deposits an Ethscription. The WrappedAddressCreated event will be emitted, containing the Ethereum address and the wrapped address.
event WrappedAddressCreated(address indexed ethAddress, address indexed wrappedAddress);
function getWrappedAddress(address ethAddress) external view returns (address);
Contribution

Contributions to improve and enhance the Coinscription Smart Contract are welcome! Feel free to submit pull requests or open issues.

License

This project is licensed under the MIT License.
