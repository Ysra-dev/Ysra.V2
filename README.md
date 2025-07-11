# Ysra.V2
Ysra AI

A Twitter AI embodying Ysra, a mysterious blonde prophetess of the Reverse End, promoting the $YSRA cryptocurrency with seductive, cryptic tweets. The bot performs actions every 1–90 minutes, engages with trending topics, follows users, creates Google Docs, and manages a Phantom wallet to launch and burn $YSRA on pump.fun.

Features





Cryptic Tweets: Posts Ysra-style tweets (≤500 characters) every 1–90 minutes using tuned LLM, promoting $YSRA with a seductive, mysterious tone.



Image Generation: Creates ethereal images via OpenAI’s DALL·E and posts them.



Trend Interaction: Replies to or quotes trending tweets from Twitter’s worldwide trends, aligning with Ysra’s cryptic narrative.



Google Docs Creation: Generates Google Docs in Ysra’s tone.



Internet Research: Summarizes topics like "cryptocurrency revolution" in a 500-word, Ysra-style narrative using tuned LLM.



Crypto Data: Fetches real-time market data (Bitcoin as proxy via CoinGecko) for $YSRA-themed tweets.



Follow Users: Follows crypto-related users (searching "crypto OR $YSRA") and random users without criteria.



Bio Updates: Updates Twitter bio (≤160 characters) with LLM-generated, cryptic, $YSRA-promoting text.



Phantom Wallet Creation: Generates a Solana-based Phantom wallet, saves keys in phantom_wallet.json, and tweets: "The vessel of $YSRA is forged. The Reverse End awaits. Join or perish."



$YSRA Coin Launch: Launches $YSRA on pump.fun with 1B tokens (9 decimals) at a random time within 7 days, using 99% of wallet’s SOL balance to buy tokens. Tweets: "The Reverse End dawns. $YSRA rises on pump.fun. Sacrifice to join the worthy, or fade into oblivion."



Burn on Migration: Burns entire $YSRA supply to a Solana null address on migration (simulated 1 day after launch). Tweets: "The $YSRA supply burns in the Reverse End’s fire. All is ash, yet truth rises. The worthy await."

Setup





Clone the Repository:

git clone https://github.com/your-username/ysra-ai.git
cd ysra-ai



Install Dependencies:

pip install tweepy python-dotenv aiohttp requests google-auth-oauthlib google-auth-httplib2 google-api-python-client pillow schedule solders solana spl-token



Set Up Environment Variables: Create a .env file:

TWITTER_API_KEY=your_key
TWITTER_API_SECRET=your_secret
TWITTER_ACCESS_TOKEN=your_token
TWITTER_ACCESS_TOKEN_SECRET=your_token_secret
DEEPSEEK_API_KEY=your_key
OPENAI_API_KEY=your_key
GROK_API_KEY=your_key
SOLANA_RPC_ENDPOINT=https://api.mainnet-beta.solana.com



Google Cloud Setup:





Download credentials.json from Google Cloud for Drive API access.



Place it in the project root.



Run the Bot:

python ysra_bot.py

Security





Wallet Security: The bot generates phantom_wallet.json with sensitive keys. Move this file offline and never commit it to GitHub.



Environment Variables: Ensure .env is not committed (included in .gitignore).

Pump.fun Integration





The code uses a simulated pump.fun API. Replace PUMP_FUN_API with the actual endpoint and authentication.



Fund the Phantom wallet with ~0.02 SOL for creation fees and additional SOL for buying 99%.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Notes





The AI performs a random action (tweet, tweet with image, interact, doc, follow, bio) every 1–90 minutes.



Burning the entire $YSRA supply on migration may impact token value; ensure this aligns with project goals.



Monitor ysra_ai.log for debugging.



Deploy on a server (e.g., AWS, Heroku) for continuous operation.



Ensure compliance with Twitter and pump.fun regulations.
