# Crypto Ticker

THIS HAS BEEN UPDATED TO ALLOW FOR USE WITH A 32X32 MATRIX.
this project is not complete and is still being tinkered with. It has additional smaller font sizes added. 

A library for displaying crypto asset prices on an LED matrix panel using a Raspberry Pi.

Requires:

  * Adafruit 32x32 LED Matrix Panel
  * Raspberry Pi Zero WH
  * CoinMarketCap API Account

See the Howchoo guide for installation and configuration instructions:

https://howchoo.com/pi/raspberry-pi-cryptocurrency-ticker

## Settings

You can customize the application by adding any of the following settings to your settings.env file in the root directory of this repo:


| Name | Default | Description |
|--|--|--|
| SYMBOLS | btc,eth | The asset symbols you want to track. |
| CURRENCY | usd | The currency used to show asset prices. CoinGecko currently supports "usd" and "eur", while CoinMarketCap supports only "usd". |
| API | coingecko | The API you want to use to fetch price data. Currently supported APIs are "coingecko" and "coinmarketcap". |
| REFRESH_RATE | 300 | How often to refresh price data, in seconds. |
| SLEEP | 3 | How long each asset price displays before rotating, in seconds. |
| CMC\_API\_KEY | | The CoinMarketCap API key, required if you specified API=coinmarketcap. |
| SANDBOX | | Used for CoinMarketCap only. Set SANDBOX=false if you're developing and want to use the sandbox API. |

Example:

```
SYMBOLS=btc,eth,ltc,xrp
API=coingecko
```
