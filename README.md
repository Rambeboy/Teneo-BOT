## TENEO NODE BOT

An automated WebSocket client for managing multiple Teneo accounts in parallel.

## FEATURES

- Multi-account support
- Automatic ping and reconnection
- Clean and organized logging
- Easy account management
- Colorful console output

## PREREQUISITE

- Node.js (version 14 or higher)
- npm (Node Package Manager)
- Teneo browser extension with registration code: `KFqtX`

## INSTALLATION

1. Clone this repository:

```bash
git clone https://github.com/Rambeboy/Teneo-BOT.git && cd Teneo-BOT
```

2. Install dependencies:

```bash
npm install
```

## CONFIGURATION

### Getting JWT Token

1. Install Teneo browser extension
2. Register using code: `KFqtX`
3. Open extension
4. Right click > Inspect
5. Click Disconnect then Connect
6. Go to WS tab
7. Find and copy the value from the payload section

### SETTING UP ACCOUNTS

1. Edit `data.txt` file in the root directory
2. Add JWT tokens (one per line) for each account.
```
jwt_token_1
jwt_token_2
...
```

## USAGE

Run the bot:

```bash
npm run start
```

The bot will:

- Display a welcome banner
- Connect to all accounts in parallel
- Send pings every 10 seconds
- Show real-time points updates
- Automatically reconnect on disconnection

## FEATURES DETAILS

### AUTO RECONNECTION

- Maximum 5 reconnection attempts
- Exponential backoff delay
- Maximum delay of 30 seconds

### ERROR HANDLING

- WebSocket connection errors
- Message parsing errors
- File reading errors
- Graceful shutdown on CTRL+C

## LICENSE

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for more details.

## Disclaimer

This tool is for educational purposes only. Use at your own risk and responsibility.
