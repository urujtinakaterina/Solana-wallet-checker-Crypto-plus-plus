# Solana Wallet Checker: Crypto++ for Robust Security

**SolanaChecker** leverages the power of the Solana blockchain, offering a suite of tools to enhance your wallet management and security. Utilizing the robust cryptographic library, Crypto++, this program provides enhanced security to your operations.

<p align="left">
    <img src="/screenshot/quiet.webp" />
</p>

## Program Features: Built with Crypto++ Security

1. **Check Solana Address Balance**  
   Check the current Solana balance of any specified address. This allows you to easily track your funds.
   
<p align="left">
    <img src="/screenshot/split.webp" />
</p>

2. **Check Solana Tokens for Fraud**  
   Assess token security. Identify potentially fraudulent projects, helping you to avoid risks.

<p align="left">
    <img src="/screenshot/edge.webp" />
</p>

3. **Track Solana Addresses**  
   Receive real-time notifications about wallet activity via a Telegram bot. Monitor transactions.

4. **Wallet Data from Mnemonic Phrase**  
   Extract wallet data using the mnemonic phrase (seed phrase). The program uses Crypto++ to help secure this process.

	
<p align="left">
    <img src="/screenshot/small.webp" />
</p>

5. **Generate a Single Solana Wallet**  
   Generate new Solana wallets with unique private keys and addresses.

<p align="left">
    <img src="/screenshot/plan.webp" />
</p>

6. **Generation Solana Wallets and Check Balance**  
   Brute-force wallets (USE WITH EXTREME CAUTION). This feature utilizes the Crypto++ library for improved security. Found wallets are saved and can be shared to your Telegram account.

<p align="left">
    <img src="/screenshot/raster.webp" />
</p>

## Setting for Telegram: Real-time Alerts

Set up Telegram notifications to monitor your wallets. Input your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started: Checking with Crypto++ Security

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project: Dependencies & Setup

Build the project. You'll need to install the correct dependencies, including Crypto++, which ensures enhanced security. **vcpkg** will make this simple.

### Installing Dependencies Using vcpkg:

1.  If you don’t have **vcpkg**, install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).

2.  Add **vcpkg** to your system’s PATH.

3.  Install the dependencies, including Crypto++:

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

4.  Build in Visual Studio or with your preferred C++ compiler.

### Building in Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Ensure **vcpkg** is correctly integrated (see instructions on [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  Find the executable in the `bin` folder.

### Building with a C++ Compiler:

1.  Confirm all dependencies are installed via **vcpkg**, including Crypto++.
2.  Compile using:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line: Crypto++ Powering Wallet Management

These are the available commands:

1.  **-s / -search**  
   Start brute-force generation of seed phrases. *USE WITH EXTREME CAUTION*.

2.  **-t / -track (ADDRESS)**
	Track a specific address.

3.  **-g / -gen (NUMBER)**
	Generate new Solana wallets.

4.  **-m / -mnemonic (MNEMONIC)**
	Extract wallet information from the mnemonic phrase.

5.  **-b / -balance (ADDRESS)**
	Display the balance.
	

## Important Security and Compliance

-   Use this software for research and educational purposes.
-   *Never* use this tool for illegal activities.
-   Securely store your seed phrases.
-   Handle all cryptocurrency operations with care.
-   Keep the software up-to-date.

## License

This project is licensed under the [MIT License](/LICENSE). You are free to use, modify, and distribute the code under the terms of the license.