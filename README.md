# seed-generator
Wallet Seed Phrase Generator

This simple script in python or HTML allows you to perform the following operations to generate a Cryptocurrency Wallet easily and securely.

* Simulates the random roll of 256 dice
* Runs SHASUM256 on the obtained string and then calculates the checksum of the string
* Displays the 24 words from the seed phrase

I recommend downloading the file seed-generator.py o seed-generator.html to a new computer not connected to the internet and running it from there. 
Write down the 24 words in non-connected mode, perhaps on several sheets of paper, taking care to store them safely.

The 24 words are the only way to get access to your wallet, whoever gets hold of them will get hold of your funds.

The HTML generator is also available online at [my site](https://www.vinacc.eu/crypto/)

If you want to support this work please consider a very small donation in BTC to my BTC wallet: `bc1qe28ujcyelpypw0e9kkpfrmvs0ncr2w82u3sxr0`

## Usage

### Python

To run the script, download the file seed-generator.py and run it from the shell with the following command:

`python3 seed-generator.py`

### HTML

Open the `seed-generator.html` file with your favourite browser and click on the Generate button.

## License
This project is distributed under the MIT License. Go to https://opensource.org/licenses/MIT for more details.

[js-sha256] - (https://github.com/emn178/js-sha256)
