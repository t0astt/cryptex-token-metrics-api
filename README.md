# Cryptex Token Metrics API
A simple API for supplying CoinMarketCap with total supply information for the CTX and TCAP tokens.

[Cryptex.Finance](https://cryptex.finance)

## Usage
First, bring up the service: `docker-compose up -d`.

### Metrics
* APY: *GET* `tokens/<token>/apy`, with `token` being CTX.
* Total Supply: *GET* `tokens/<token>/total-supply`, with `token` being either CTX or TCAP.
  * For CoinMarketCap format (raw string), *GET* `tokens/<token>/total-supply?cmc=true`
* All metrics: *GET* `tokens/<token>`, with `token` being either CTX or TCAP.

## Changelog
* 2.0.0 - Implement new endpoint paths, support getting APY metrics for CTX
* 1.0.1 - Fix paths
* 1.0.0 - Initial API