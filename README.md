# AVAX_Advanced_Module_1_Project_1

## Project Description

This project is designed to teach us how to create your own custom subnet using the Avalanche SubnetEVM. We will learn how to deploy this subnet to the local network and then deploy your own contracts to the custom subnet.

## Video Walkthrough
https://www.loom.com/share/61e1d667fc55409c842bacdce6607f3b?sid=ce2ad0e9-02ad-4533-8f64-4b2da879d6f9

## Steps to Run the Project

### Using Remix IDE and Terminal

1. **Install Avalanche CLI**
   - Install `avalanche-cli` on your UNIX system.[Avalanche](https://docs.avax.network/tooling/cli-guides/install-avalanche-cli).

2. **Copy and Test Contracts**
   - Copy `ERC20.sol` and `Vault.sol` from this repository.
   - Paste them into the Remix IDE at [REMIX](https://remix.ethereum.org)

3. **Install MetaMask Extension**
   - Install the MetaMask browser extension and create an account.

4. **Create Your Subnet**
   - In a terminal, run:
     ```bash
     avalanche subnet create <your-subnet-name>
     ```
   - Follow the steps given by Metacrafters Team and Create Your Avalanche subnet.

5. **Deploy Your Subnet**
   - Run the following command:
     ```bash
     avalanche subnet deploy <your-subnet-name>
     ```
   - Choose "local network" for deployment.

6. **Output Interpretation**
   - The command output will include details such as:
     ```
     1.RPC URL
     2.Funded address  - private key
     3.Funded address 
     4.Network name
     5.Chain ID
     6.Currency Symbol
     ```

7. **Add Custom Network in MetaMask**
   - Use the details from the output of the last command to add a custom network in MetaMask.

8. **Add Funded Account in MetaMask**
   - Add an account using the provided private key from the output.

9. **Deploy Contracts in Remix**
   - In Remix IDE, select "Injected Web3" as the environment.
   - Deploy `ERC20.sol` first.
   - Then deploy `Vault.sol`, using the deployed address of `erc20.sol` as the constructor parameter.

10. **Mint and Deposit Tokens**
    - Mint some tokens to your address using the `mint` function in `ERC20.sol`.
    - Deposit some tokens and receive shares in return using `Vault.sol`.

## Contributors

- Metacrafter Om Satapathy (Twitter: [@OmSatapathy4](https://twitter.com/OmSatapathy4))

## License

This project is licensed under the MIT License.
