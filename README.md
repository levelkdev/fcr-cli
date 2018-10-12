# fcr-cli

command line interface for [fcr-contracts](https://github.com/levelkdev/fcr-contracts)

## Setup

`npm install`

`npm run build` to build the CLI (output to `build/fcr`)

## Usage

#### Commands:

  | Command | Description |
  | --- | --- |
  | `fcr apply <listingHash> <amount> [data]`  | submit a listing application to the registry |
  | `fcr challenge <listingHash> [data]`       | create a challenge for a listing |
  | `fcr buy <listingHash> <outcome> <amount>` | buys outcome token on the given listing's challenge market |
  | `fcr close <listingHash>`                  | close the challenge |
  | `fcr resolve <listingHash> <price>`        | resolve scalar market price oracles for a challenge |
  | `fcr challengeStatus <listingHash>`        | outputs the status of a challenge for the given listingHash |
  | `fcr registryName`                         | get the name of the registry |
  | `fcr tokenBalance <address>`               | gets the amount of FCR token held by the given address |
  | `fcr registryAllowance <address>`          | gets the amount of token the registry contract can spend on behalf of the given address |

#### Options:

  | Option | Description | Type |
  | --- | --- | --- |
  | `--version`        | Show version number     | `[boolean]` |
  | `-v`, `--verbose`  | log verbose output      | `[boolean]` `[default: false]` |
  | `--network`        | network config to use   | `[default: "rinkeby"]` |
  | `--help`           | Show help               | `[boolean]` |
