# Welcome to LastManHolding

LastManHolding NFT will reward a random existing holder with 10% of the purchase price of last NFT sold.
Every NFT purchased will reward a current holder randomly until there is only one left. The last NFT sold will earn a total
of 10% (1.5BNB) of the entire treasury, total value of all the NFTS sold.
Pricing is currently at base cost of 0.15BNB. Get in early to have more chances to be rewarded and remember!
You can always have more than one, which means
more chances for rewards. 1 Lastman NFT per transaction with no cap on qty per wallet. Enjoy the Ride!!


![](https://github.com/cheynespc/Lastman_nft_minting_dapp/blob/main/public/dappscreenshot.png)

## Contract and dapp on BSC Testnet

[Solidity File Here](https://github.com/cheynespc/Lastman_nft_minting_dapp/blob/main/LastManHoldingNFT.sol)

[BSC Testnet Contract](https://testnet.bscscan.com/address/0xa4f64d98ad39a25975d19ac174f9e7a35209369a#code)

[DAPP  test alpha (Netlify) here](https://fanciful-otter-5cc3f3.netlify.app/)

[Lastman Main Page](https://lastmanstanding.info/)



## Tokenomics

100% of NFT sales broken down

10% goes to rewarding Holders

10% goes to The Last Man NFT Sold

30% Marketing Wallet

10% Developers Fees

10% Advertisings Costs

30% to Buy back Lastman Standing and Lastman Giving increasing the chart


Funds held until last NFT Sold
90% Funds held in contract with 10% rewarding a random existing holder per mint

![](https://github.com/cheynespc/Lastman_nft_minting_dapp/blob/main/public/Tokenomics.png)

# LastManHolding NFT minting dapp 🔥

![](https://github.com/cheynespc/Lastman_nft_minting_dapp/blob/main/banner.png)


## Contracts Write Features

![](https://github.com/cheynespc/Lastman_nft_minting_dapp/blob/main/public/Contractwritefeatures.png)

## Test Results of bonus Last NFT sold Remix EVM

![](https://github.com/cheynespc/Lastman_nft_minting_dapp/blob/main/public/RemixLogtestFinalsale.png)



This repo provides a nice and easy way for linking an existing NFT smart contract to this minting dapp. There are two ways of using this repo, you can go the simple route or the more complex one.

The simple route is so simple, all you need to do is download the build folder on the release page and change the configuration to fit your needs. (Follow the video for a walk through).

The more complex route allows you to add additional functionality if you are comfortable with coding in react.js. (Follow the below instructions for a walk through).

## Installation 🛠️


If you are cloning the project then run this first, otherwise you can download the source code on the release page and skip this step.

```sh
git clone https://github.com/HashLips/hashlips_nft_minting_dapp.git
```

Make sure you have node.js installed so you can use npm, then run:

```sh
npm install
```

## Usage ℹ️

In order to make use of this dapp, all you need to do is change the configurations to point to your smart contract as well as update the images and theme file.

For the most part all the changes will be in the `public` folder.

To link up your existing smart contract, go to the `public/config/config.json` file and update the following fields to fit your smart contract, network and marketplace details. The cost field should be in wei.

Note: this dapp is designed to work with the intended NFT smart contract, that only takes one parameter in the mint function "mintAmount". But you can change that in the App.js file if you need to use a smart contract that takes 2 params.

```json
{
  "CONTRACT_ADDRESS": "0xA4F64d98ad39A25975D19AC174F9E7a35209369A",
  "SCAN_LINK": "https://testnet.bscscan.com/address/0xa4f64d98ad39a25975d19ac174f9e7a35209369a#code",
  "NETWORK": {
    "NAME": "TESTNET Binance Smart Chain",
    "SYMBOL": "BNB",
    "ID": 97
  },
  "NFT_NAME": "Last Man Holding NFT",
  "SYMBOL": "LASTMAN",
  "MAX_SUPPLY": 777,
  "WEI_COST": 75000000000000000,
  "DISPLAY_COST": 0.21,
  "GAS_LIMIT": 285000,
  "MARKETPLACE": "ToFuNFT",
  "MARKETPLACE_LINK": "https://opensea.io/collection/LastManHolding",
  "SHOW_BACKGROUND": false
}
```

Make sure you copy the contract ABI from remix and paste it in the `public/config/abi.json` file.
(follow the youtube video if you struggle with this part).

Now you will need to create and change 2 images and a gif in the `public/config/images` folder, `bg.png`, `example.png` and `logo.png`.

Next change the theme colors to your liking in the `public/config/theme.css` file.

```css
:root {
  --primary: #3f8cff;
  --primary-text: #ffffff;
  --secondary: #0054ff;
  --secondary-text: #ffffff;
  --accent: #505050;
  --accent-text: #ffffff;
}
```

Now you will need to create and change the `public/favicon.ico`, `public/logo192.png`, and
`public/logo512.png` to your brand images.

Remember to update the title and description the `public/index.html` file

```html
<title>Last Man Holding NFT</title>
<meta name="description" content="Last Man Holding NFT" />
```

Also remember to update the short_name and name fields in the `public/manifest.json` file

```json
{
  "short_name": "LASTMAN",
  "name": "LastManHolding NFT"
}
```

After all the changes you can run.

```sh
npm run start
```

Or create the build if you are ready to deploy.

```sh
npm run build
```

Now you can host the contents of the build folder on a server.

That's it! you're done.

Thanks to Hashlips for original Code

All the code in these repos was created and explained by HashLips on the main YouTube channel.

To find out more please visit:

[📺 YouTube](https://www.youtube.com/channel/UC1LV4_VQGBJHTJjEWUmy8nA)

[👄 Discord](https://discord.com/invite/qh6MWhMJDN)

[💬 Telegram](https://t.me/hashlipsnft)

[🐦 Twitter](https://twitter.com/hashlipsnft)

[ℹ️ Website](https://hashlips.online/HashLips)
