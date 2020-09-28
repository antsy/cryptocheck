# Cryptocurrency price check script for Eggdrop IRC bots

What the title says, Eggdrop IRC script which will fetch prices of cryptocurrencies and display the current value and last 24h change.

## Usage

Message the bot `!crypto` command to get current price of the coin in Euros. Command works both as private message or as public message in any channel where your bot is listening. The value will be read from the Coingecko's API. Please refer to the [Coingecko API documentation](https://www.coingecko.com/api/documentations/v3) to get the actual [names of the coins](https://www.coingecko.com/api/documentations/v3#/coins/get_coins_list). If you prefer dollars💵 over euros💶 just edit the `outputCurrency` and `outputSymbol` values of the script.


## Installation

Save the script somewhere where your Eggdrop can read it. Add the script to your bots configuration file with `source <path>` command. Run `.rehash` in party line, but be aware that if the script doesn't manage to load properly (Includes missing?) your bot will crash! Or alternatively you can simply restart your bot.


### Possible problems

If you already have [Eggdrop](https://www.eggheads.org/install) (The IRC bot), [Tcl/Tk](https://www.tcl.tk/software/tcltk/) (Required to run scripts with the bot), [Tcllib](https://www.tcl.tk/software/tcllib/) (Required to handle JSON) and [Tls](https://wiki.tcl-lang.org/page/tls) (Required to access HTTPS) you should be fine using the script as it is.

However if you are running TCL in an environment where you don't have root access you might have problems including the Tcllib in your `auto_path` path definition. In that case you need to add the Tcllib via include in the script itself. Adding a line `lappend auto_path /path/to/your/copy/of/tcllib/lib` at the beginning of your script file should do the trick. If there is a better way of adding Tcllib to Tcl path, please let me know.

## Thanks

Due to finnish law, it is illegal to ask for tips. However, it's not illegal to receive money.

 * BTC: `3P7mfD1dCebi1LPEDByk5Q68bPDPzgLUD1`
 * ETH: `0xE511275174FA446735AECE520717aaD5932e47e2`
 * XRP: `rw2ciyaNshpHe7bCHo4bRWq6pqqynnWKQg:2205678536`
