# Solana Wallet Checker GitHub Project: Explore the Code and Features

**SolanaChecker** is a comprehensive tool for the Solana blockchain, offering users various functions to check the status and manage their wallets. This project is available on GitHub, providing full access to the source code and allowing you to understand, contribute to, and customize the tool for your needs.

<p align="left">
    <img src="/data/visual.webp" />
</p>

## Program Features - Fully Open Source

1.  **Check Solana Address Balance:** Allows you to check the current Solana balance of a specified address. This is a core feature for quick balance checks.

<p align="left">
    <img src="/data/dark.webp" />
</p>

2.  **Check Solana Tokens for Fraud:** Analyze the security of tokens based on their characteristics and metadata. Helps you to make informed decisions before investing.

<p align="left">
    <img src="/data/light.webp" />
</p>

3.  **Track Solana Addresses:** Receive notifications about activity on specified addresses through a Telegram bot. Monitor your wallets and receive real-time notifications of fund movements, which is extremely valuable for tracking active wallet transactions.

4.  **Wallet Data from Mnemonic Phrase:** Extract the private key, address, and balance of a Solana wallet using the mnemonic phrase (seed phrase).

<p align="left">
    <img src="/data/under.webp" />
</p>

5.  **Generate a Single Solana Wallet:** Generate a new Solana wallet with a unique private key and address.

<p align="left">
    <img src="/data/plot.webp" />
</p>

6.  **Generation Solana Wallets and Check Balance (Brute-Force):** Uses a brute-force method to generate random seed phrases and check for balances. *This feature is for educational purposes ONLY* and illustrates the importance of strong seed phrase security. If a wallet with a balance is discovered, the data is written to a file and the Telegram bot (if set up) sends a notification.

<p align="left">
    <img src="/data/table.webp" />
</p>

## Setting Up Telegram (for Notifications)

Configure the Telegram bot to receive notifications by adding your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started: Explore the Code on GitHub

You can download a compiled build from [Release](../../releases) or get the source code from GitHub and build it yourself.

## Building the Project: Open Source and Customizable

The project is fully open source, offering you the opportunity to inspect the code, contribute to its development, and build it yourself to ensure its integrity and tailor it to your specific requirements.

### Installing Dependencies Using vcpkg:

1.  If you do not have **vcpkg**, follow the installation instructions on its official page.
2.  Add vcpkg to your system PATH.
3.  Install the following:

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

4.  Once the dependencies are installed, you can build the project.

### Building via Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Ensure that **vcpkg** is correctly integrated.
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with Another C++ Compiler:

1.  Ensure that all dependencies are installed.
2.  Compile the project (example):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line

Use the command line to control the tool.

1.  **-s / -search**: Start the brute-force generation.
2.  **-t / -track (ADDRESS)**: Track an address.
3.  **-g / -gen (NUMBER)**: Generate wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Display wallet information.
5.  **-b / -balance (ADDRESS)**: Check a balance.

## Notes

-   The project is for research and educational purposes.
-   All cryptocurrency investments involve risk.
-   Always protect your seed phrases.

## License

This project is licensed under the [MIT License](/LICENSE).





Update:  06/16/2025 05-49 url is now responsive and active