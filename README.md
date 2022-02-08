# MuesliSwap Token Verification 🪙✔

The official repository to verify your token @ AdaMuesliSwap  
Please also read the corresponding section in our [documentation](https://docs.muesliswap.com/cardano/community-tokens/token-verification).

## Fees
Using the Community section, it is possible to trade **any** token on Cardano **without** being verified.  
However, verification will give you more visibility and increase the trust of the community.  
To account for processing each verification manually and to prevent people from spamming requests we require a verification fee of **50 ADA**. 

## How can I get verified?
Submit a Pull Request to this repository that that adds three things: 

📄 A correct JSON token description in the [tokens](tokens) folder  
🖼️ An image for the token in the [images](images) folder.  
💸 A comment, with the transaction id showing you submitted 50 ADA to the [payment address](https://cardanoscan.io/address/01deb0dfa55b77e1d9d5ccc3168fad7fdf471a8b9326f026a1ed43908c495455e8f4d0042e077c25be5f30157249c9c4d57cae732d555ef105)
  
Note that there are specific minimum requirements to get verified, such as:  
  
🌐 A website  
📝 A token description   
📊 Tokenomics  
✉️ Contact information (e.g., twitter, email)  
  
Please make sure that your policy id is somewhere on your website!  
If you do not know how to implement these requirements, check our MILK token or contact us.  

### JSON token description

The folder `tokens` contains [JSON](https://en.wikipedia.org/wiki/JSON) files that describe each verified token listed at AdaMuesliSwap.
Each file contains information on what the coin is called, its supply and other important information.
The name of the file is the string `<policy_id>.<name>.json`.

| Field | Description | Example |
| ----- | ----------- | ------- |
| `policyId` | The policy id of the token | `8a1cfae21368b8bebbbed9800fec304e95cce39a2a57dc35e2e3ebaa` |
| `name` | The asset name of the token | `MILK` |
| `symbol` | A trading symbol of the token | `MILK` or `CDOG` |
| `website` | Homepage of the corresponding token | `https://ada.muesliswap.com` |
| `description` | A very short description of the token | `Your favorite pre-sale token, making you stronger` |
| `totalSupply` | The total minted amount of the token | `100000000` |
| `amounts` | A list of integers of the trade size options |`[1000, 5000, 10000]` |
| `decimalPlaces` | The number of decimal places when displaying the token. | ADA has 6 decimal places. 1 token = 1 Lovelace = 0.000001 ADA, displayed as "6 zeroes" |

### Images

In the folder `images`, an image is listed for each token that should be traded.
This is required so that an image can be displayed for the token on the website.
The name of the file is the string `<policy_id>.<name>.png`.

### Payment

The payment address is [addr1q80tpha9tdm7rkw4enp3drad0l05wx5tjvn0qf4pa4peprzf23273axsqshqwlp9he0nq9tjf8yuf4tu4eej64277yzskzqlf2](https://cardanoscan.io/address/01deb0dfa55b77e1d9d5ccc3168fad7fdf471a8b9326f026a1ed43908c495455e8f4d0042e077c25be5f30157249c9c4d57cae732d555ef105)  
we can only complete the verification once we receive the payment. 
Please include a message with your token name or other identifying information in your transaction. 

### Example  

See [tokens/8f52f6a88acf6127bc4758a16b6047afc4da7887feae121ec217b75a.SNOW.json](tokens/8f52f6a88acf6127bc4758a16b6047afc4da7887feae121ec217b75a.SNOW.json) for an example file.
Also check the token on [cardanoscan.io](https://cardanoscan.io/token/8a1cfae21368b8bebbbed9800fec304e95cce39a2a57dc35e2e3ebaa4d494c4b) if you are unsure about some values.
