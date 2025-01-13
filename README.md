# XPHERE Miner

**XPHERE Miner** is a high-performance, multi-threaded mining program designed for the XPHERE network.  
It enables users to mine blocks efficiently and earn rewards. The program is compatible with multiple platforms, including **Windows**, **macOS**, and **Linux**.

## Key Features

- **Multi-Platform Support**: Runs on Windows, macOS, and Linux
- **SHA-256 Based Mining**: Secure and optimized Proof of Work implementation
- **User-Friendly Configuration**: Provides a configuration file (`config.json`) and command-line options
- **XPHERE Network Compatibility**: Supports XPHERE TEST NET 2.0

## Release

Stay up-to-date with the latest updates and improvements:

- **Latest Release Notes**: [Release v0.0.1](https://github.com/xpherechain/Xphere-miner/releases/tag/v0.0.1)

---

### 2. Download the Program

1. Visit the [latest release page](https://github.com/xpherechain/Xphere-miner/releases).
2. Download the miner binary appropriate for your operating system.
3. **Make sure to also download (or place) the `config.json` file in the same directory as the binary.**

4. Set Up the Target Miner
   To run the miner program, you need to set the targetMiner. Follow these steps
   - Visit https://zigap.io and create a wallet.
   - Once the wallet is created, copy the generated address and set it as the targetMiner in the configuration.
   - Select the `XPHERE 2.0 (Testnet) network` in the wallet, then copy the generated wallet address and use it as the targetMiner in your setup.

#### MacOS

1. Open the Terminal.
2. Navigate to the directory where you placed the MacOS miner binary, and also place the `config.json` file in the same directory.
3. The file to which you are granting execute permissions.

   ```bash
   chmod +x miner-darwin-amd64
   ```

4. Run the following command:

   ```bash
   ./miner-darwin-amd64 -config ./config.json -targetMiner your wallet address

   Note: If you encounter a warning about an unidentified developer, go to System Preferences → Security & Privacy → General, and allow the miner program.
   ```

##### Example

```
C:\Users\USER\Downloads>miner-window-amd64 -config ./config.json -targetminer 0x43ee5CDDF65F4cafA4b834e3c93108532Fe8768
```

#### Windows

1. Open Command Prompt with administrator privileges.
2. Navigate to the directory where you placed the Windows miner binary, and also place the config.json file in the same directory.
3. Run the following command:

```
miner-window-amd64 -config ./config.json -targetMiner your wallet addr
```

**Make sure to use the appropriate command for your operating system and the location of the downloaded files.
For example, run the following command**

##### Example

```
C:\Users\USER\Downloads>miner-window-amd64 -config ./config.json -targetminer 0x43ee5CDDF65F4cafA4b834e3c93108532Fe8768
```

---

### Contact & Feedback

If you need help using the program or want to report a bug, please contact us by email or visit our official website

- <a href="https://x-phere.com" target="_blank">XPHERE Homepage</a>
- <a href="https://zigap.io" target="_blank">Wallet Website</a>

---
