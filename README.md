# XPHERE Miner

**XPHERE Miner** is a high-performance, multi-threaded mining program designed for the XPHERE network.  
It enables users to mine blocks efficiently and earn rewards. The program is compatible with multiple platforms, including **Windows**, **macOS**, and **Linux**.

**_Looking to get started quickly? 🚀 With our [Faucet Service](https://faucet.x-phere.com/), you can claim free XPHERE TestNet coins to set up your wallet and dive into mining in no time. It’s the perfect way to jumpstart your journey in the XPHERE ecosystem and begin earning rewards efficiently._**

## Key Features

- **Multi-Platform Support**: Runs on Windows, macOS, and Linux
- **SHA-256 Based Mining**: Secure and optimized Proof of Work implementation
- **User-Friendly Configuration**: Provides a configuration file (`config.json`) and command-line options
- **XPHERE Network Compatibility**: Supports XPHERE TEST NET 2.0

## Release

Stay up-to-date with the latest updates and improvements:

- **Latest Release Notes**: [Release v0.0.4](https://github.com/xpherechain/Xphere-miner/releases/tag/v0.0.3)

---

### 2. Download the Program

1. Visit the [latest release page](https://github.com/xpherechain/Xphere-miner/releases).
2. Download the miner binary appropriate for your operating system.
3. **Make sure to also download (or place) the `config.json` file in the same directory as the binary.**

4. Set Up the Target Miner
   To run the miner program, you need to set the targetMiner. Follow these steps
   - Visit https://about.zigap.io and create a wallet.
   - Once the wallet is created, copy the generated address and set it as the targetMiner in the configuration.
   - Select the `XPHERE 2.0 network` in the wallet, then copy the generated wallet address and use it as the targetMiner in your setup.

### MacOS

1. Open the Terminal.
2. Navigate to the directory where you placed the MacOS miner binary, and also place the `config.json` file in the same directory.

- By default, downloaded files are stored in the `Downloads` folder.

  ```
  cd ~/Downloads
  ```

3. The file to which you are granting execute permissions.

   ```bash
   chmod +x miner-darwin-amd64
   ```

4. Run the following command:

- **_Note: If you encounter a warning about an unidentified developer, go to System Preferences → Security & Privacy → General, and allow the miner program._**

  • Option 1: Using config.json

  ```bash
  ./miner-darwin-amd64 -config ./config.json
  ```

  - **🛠 Example `config.json` File**

    If you prefer to use a configuration file instead of manually entering parameters, create a `config.json` file with the following structure:

    ```json
    {
      "targetMiner": "",
      "domain": []
    }
    ```

  • Option 2: Running without config.json (Manually specify all parameters)

  ```bash
  ./miner-darwin-amd64 -targetMiner [targetAddress] -domain [https://abcd,https://abcd2...]
  ```

#### Example Mac Command Execution - Mainnet,TestNet

##### ![Mainnet](https://img.shields.io/badge/Mainnet-red?style=flat-square)

1. Option 1: Using config.json:

- #### ~/Downloads % ./miner-darwin-amd64 -config ./config.json

2. Option 2: Running without config.json (Manually specify all parameters):

- #### ~/Downloads % ./miner-darwin-amd64 -targetMiner <code>**_0x43e...e8768_**</code> -domain <code>https://sgp-mining.x-phere.com,https://bkk-mining.x-phere.com,https://hkg-mining.x-phere.com,https://idn-mining.x-phere.com</code>

##### ![TestNet](https://img.shields.io/badge/TestNet-blue?style=flat-square)

- #### ~/Downloads % ./miner-darwin-amd64 -targetMiner <code>**_0x43e...e8768_**</code> -domain <code>https://testnet-asia-mining.x-phere.com</code>

### Linux

1. Open the Terminal.
2. Navigate to the directory containing the miner binary and config file

- By default, downloaded files are stored in the `Downloads` folder.
  ```
  cd ~/Downloads
  ```

3. Replace <server_ip> with your actual server IP, and make sure to use the correct username and file path.

   ```
   scp miner-linux-amd64 config.json root@<server_ip>:/root/
   ```

4. Once the transfer is complete, connect to the server and verify that both miner-linux-amd64 and config.json exist in the specified directory.

   ```
   ls -al
   ```

5. Grant execute permissions

   ```
   chmod +x miner-linux-amd64
   ```

6. Run the miner program

- Option 1: Using config.json

  ```bash
  ./miner-linux-amd64 -config ./config.json
  ```

  - **🛠 Example `config.json` File**

    If you prefer to use a configuration file instead of manually entering parameters, create a `config.json` file with the following structure:

    ```json
    {
      "targetMiner": "",
      "domain": []
    }
    ```

- Option 2: Running without config.json (Manually specify all parameters)

  ```bash
  ./miner-linux-amd64 -targetMiner [targetAddress] -domain [https://abcd,https://abcd2...]
  ```

#### Example Linux Command Execution - Mainnet,TestNet

##### ![Mainnet](https://img.shields.io/badge/Mainnet-red?style=flat-square)

1. Option 1: Using config.json:

- #### root@USER:~# ./miner-linux-amd64 -config ./config.json

2. Option 2: Running without config.json (Manually specify all parameters):

- #### root@USER:~# ./miner-linux-amd64 -targetMiner <code>**_0x43e...e8768_**</code> -domain <code>https://sgp-mining.x-phere.com,https://bkk-mining.x-phere.com,https://hkg-mining.x-phere.com,https://idn-mining.x-phere.com</code>

##### ![TestNet](https://img.shields.io/badge/TestNet-blue?style=flat-square)

- #### root@USER:~# ./miner-linux-amd64 -targetMiner <code>**_0x43e...e8768_**</code> -domain <code>https://testnet-asia-mining.x-phere.com</code>

### Windows

1. **_Open Command Prompt with administrator privileges._**
2. Navigate to the directory where you placed the Windows miner binary, and also place the config.json file in the same directory.
3. Run the following command:

```
cd %USERPROFILE%\Downloads
```

- Option 1: Using config.json

  ```bash
  miner-windows-amd64 -config ./config.json
  ```

  - **🛠 Example `config.json` File**

    If you prefer to use a configuration file instead of manually entering parameters, create a `config.json` file with the following structure:

    ```json
    {
      "targetMiner": "",
      "domain": []
    }
    ```

- Option 2: Running without config.json (Manually specify all parameters)

  ```bash
   miner-windows-amd64 -targetMiner [targetAddress] -domain [https://abcd,https://abcd2...]
  ```

#### Example Window Command Execution - Mainnet,TestNet

##### ![Mainnet](https://img.shields.io/badge/Mainnet-red?style=flat-square)

1. Option 1: Using config.json:

- #### C:\Users\USER\Downloads> miner-windows-amd64 -config ./config.json

2. Option 2: Running without config.json (Manually specify all parameters):

- #### C:\Users\USER\Downloads> miner-windows-amd64 -targetMiner <code>**_0x43e...e8768_**</code> -domain <code>https://sgp-mining.x-phere.com,https://bkk-mining.x-phere.com,https://hkg-mining.x-phere.com,https://idn-mining.x-phere.com</code>

##### ![TestNet](https://img.shields.io/badge/TestNet-blue?style=flat-square)

- #### C:\Users\USER\Downloads> miner-windows-amd64 -targetMiner <code>**_0x43e...e8768_**</code> -domain <code>https://testnet-asia-mining.x-phere.com</code>

### Contact & Feedback

If you need help using the program or want to report a bug, please contact us by email or visit our official website

- <a href="https://x-phere.com" target="_blank">XPHERE Network Homepage</a>
- <a href="https://about.zigap.io" target="_blank">ZIGAP Wallet Homepage</a>

---
