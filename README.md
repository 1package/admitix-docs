<h1><p align="center">🤖 <a href="https://t.me/Admitix_Bot">Admitix</a> — simplify your group management!</p></h1>


<p align="center">
	<a href="https://t.me/Admitix_Bot">
		<img src="/images/logo.png" width="700">
	</a>
</p>

<h1><p align="center">Content</p></h1>

- [Short description](#Short-description)
- [Quick start](#Quick-start)
- [Commands](#Commands)
	- [Admins](#-Admins)
		- [ban / b](#ban--b)
		- [captcha / c](#captcha--c)
		- [delete_commands](#delete_commands)
		- [language / l](#language--l)
		- [mute / m](#mute--m)
		- [time_zone / tz](#time_zone--tz)
		- [unban / ub](#unban--ub)
		- [unmute / um](#unmute--um)
		- [token_info / ti](#token_info--ti)
		- [warning / w](#warning--w)
	- [Users](#-Users)
		- [report / r](#report--r)
		- [token_info / ti](#token_info--ti-1)
		- [warning / w](#warning--w-1)
- [Captcha](#Captcha)
	- [Random](#Random)
	- [Numbers and buttons](#Numbers-and-buttons)
	- [Letters](#Letters)
	- [Arithmetic](#Arithmetic)
	- [None](#None)
- [Anti-spam system (BETA)](#Anti-spam-system-BETA)
- [I found a bug or have an idea](#I-found-a-bug-or-have-an-idea)
- [Donation](#Donation)

<h1><p align="center">Short description</p></h1>
<p align="right"><a href="#Content">To the content</a></p>

⠀Admitix created to simplify group management!

⠀Main functions:
- Anti-spam protection:
  - Several types of captchas for new members;
  - Anti-spam system for crypto groups (BETA).
- Deleting system messages;
- Commands for user management;
- Commands for working with crypto.

<h1><p align="center">Quick start</p></h1>
<p align="right"><a href="#Content">To the content</a></p>

⠀To add the bot to your group, you need:
- Start [Admitix](https://t.me/Admitix_Bot) to get report notifications;
- Add him to your group;
- Give him admin rights through the group settings;
- In the sent message, select the language of your group;
- If your group time zone is different from UTC change hour offset using the `/time_zone` command, e.g.:
```
/time_zone -4
/time_zone 3
```

⠀That's it, he's completely ready to go!

⠀The following settings will be applied by default:
- Time zone: UTC;
- Captcha type: random;
- Time to solve a captcha: 60 seconds;
- Maximum failed captcha attempts: 3;
- Warning threshold: 3;
- Mute duration after passing warning threshold: 1 day.

⠀You can set them up separately by using the commands below.
  
<h1><p align="center">Commands</p></h1>
<p align="right"><a href="#Content">To the content</a></p>

⠀Useful info:
- User can use either `/` or `!` as the beginning of a command.
- Add to a command the «help» or «h» argument to view the verbose info, e.g.:
```
/warning help
/warning h
```
- <ins>Underlined</ins> arguments are mandatory.
- Press `/`, start typing a command and press Tab on your PC or press and hold the tip on your smartphone to finish it.
- All bot messages and commands are deleted after 1 minute.

<h2><p align="center">👮 Admins</p></h2>

<h3><p align="center">ban / b</p></h3>

🧰 __Functionality__:

⠀Ban a user.

🗣 __Aliases__:
```
/ban, !ban
/b, !b
```

⚙️ __Usage__:

/b USERNAME

- USERNAME — the username in any format

🕹 __Examples__:
```
/b — as a reply to a message
/b @username
```

<h3><p align="center">captcha / c</p></h3>

🧰 __Functionality__:

⠀Customize the captcha:
- Type (current: ___);
- Time for solution (current: ___ seconds);
- Maximum failed attempts (current: ___).

🗣 __Aliases__:
```
/captcha, !captcha
/c, !c
```

⚙️ __Usage__:
```
/c
```

<h3><p align="center">delete_commands</p></h3>

🧰 __Functionality__:

⠀Delete the bot command tips.

🗣 __Aliases__:
```
/delete_commands, !delete_commands
```

⚙️ __Usage__:
```
/delete_commands
```

<h3><p align="center">language / l</p></h3>

🧰 __Functionality__:

⠀Change the bot language and set up command tips.

🗣 __Aliases__:
```
/language, !language
/l, !l
```

⚙️ __Usage__:
```
/l
```

<h3><p align="center">mute / m</p></h3>

🧰 __Functionality__:

⠀Mute a user (default for __1__ hour).

🗣 __Aliases__:
```
/mute, !mute
/m, !m
```

⚙️ __Usage__:

/m USERNAME DURATION

- USERNAME — the username in any format
- DURATION — mute duration
  - DAYSd HOURSh MINUTESm
  - DD.MM.YYYY HH:MM — date and time in UTC
  - DD/MM/YYYY HH:MM (UTC)

🕹 Examples:
```
/m — as a reply to a message
/m 15m
/m 1d 2H 10m
/m 25.07.2022 19:30
/m @username 3H
/m @username 2h 30M
/m @username 15/09/2022 11:23
```

<h3><p align="center">time_zone / tz</p></h3>

🧰 __Functionality__:

⠀Change the group time zone. Current one is ___.

🗣 __Aliases__:
```
/time_zone, !time_zone
/tz, !tz
```

⚙️ __Usage__ (<ins>underlined</ins> is mandatory):

/tz <ins>OFFSET</ins>

- <ins>OFFSET</ins> — hour offset from UTC

🕹 Examples:
```
/tz 3 — UTC+3
/tz 0 — UTC
/tz -5 — UTC-5
```

<h3><p align="center">unban / ub</p></h3>

🧰 __Functionality__:

⠀Unban a user.

🗣 __Aliases__:
```
/unban, !unban
/ub, !ub
```

⚙️ __Usage__ (<ins>underlined</ins> is mandatory):

/ub <ins>USERNAME</ins>

- <ins>USERNAME</ins> — the username in any format

🕹 __Examples__:
```
/ub @username
```

<h3><p align="center">unmute / um</p></h3>

🧰 __Functionality__:

⠀Unmute a user.

🗣 __Aliases__:
```
/unmute, !unmute
/um, !um
```

⚙️ __Usage__ (<ins>underlined</ins> is mandatory):

/um <ins>USERNAME</ins>

- <ins>USERNAME</ins> — the username in any format

🕹 __Examples__:
```
/um @username
```

<h3><p align="center">token_info / ti</p></h3>

🧰 __Functionality__:

⠀Show a token info:
- Price;
- Circulating supply;
- Market cap;
- Total supply;
- Fully Diluted Value (FVD).

⠀In addition, it allows to calculate the product of the price.

🗣 __Aliases__:
```
/token_info, !token_info
/ti, !ti
```

⚙️ __Usage__ (<ins>underlined</ins> is mandatory):

/ti <ins>SYMBOL</ins> NUMBER

- <ins>SYMBOL</ins> — token symbol
- NUMBER — number to calculate a product

🕹 Examples:
```
/ti eth
📢 Project name: Ethereum
⚛️ Token symbol: ETH

💵 Price: 1 072.61$

🔄 Circulating supply: 119 514 467 ETH 
📊 Market cap: 128 192 413 224$

📈 Total supply: -
💰 Fully Diluted Value (FVD): -
```
```
/ti btc 0.00042
📢 Project name: Bitcoin
⚛️ Token symbol: BTC

💵 Price: 19 432.41$
🧮 Product: 8.16161$

🔄 Circulating supply: 19 082 512 BTC (90.87%)
📊 Market cap: 370 819 197 013$

📈 Total supply: 21 000 000 BTC
💰 Fully Diluted Value (FVD): 408 080 610 000$
```
```
/ti bnb 0,292
/ti sol 1'200
/ti trx 119 272 123.59
```

<h3><p align="center">warning / w</p></h3>

🧰 __Functionality__:

⠀Warn a user, on __ warnings a mute will be issued for ___.

🗣 __Aliases__:
```
/warning, !warning
/w, !w
```

⚙️ __Usage__ (<ins>underlined</ins> is mandatory):

/w <ins>COMMAND</ins>

- <ins>COMMAND</ins>
  - info — view current warnings
  - reset — reset warnings
  - setup NUMBER DAYSd HOURSh MINUTESm — setup warning threshold and/or mute duration

/w USERNAME <ins>COMMAND</ins>

- USERNAME — the username in any format
- <ins>COMMAND</ins> — the command to apply to the user

/w USERNAME <ins>REASON</ins>

- USERNAME — the username in any format
- <ins>REASON</ins> — reason of the warning

🕹 __Examples__:
```
/w info — as a reply to a message
/w insult of chat member — as a reply to a message
/w setup 5
/w setup 5 12H 30m
/w setup 5 7d 3H 2m
/w @username reset
/w @username racism

/w @username
Don't
do it
again.
```

<h2><p align="center">👨‍💼 Users</p></h2>

<h3><p align="center">report / r</p></h3>

🧰 __Functionality__:

⠀Report a user violation. The report notification will be sent to the group administrators who started the bot.

🗣 __Aliases__:
```
/report, !report
/r, !r
```

⚙️ __Usage__:
```
/r — as a reply to a message
```

<h3><p align="center">token_info / ti</p></h3>

🧰 __Functionality__:

⠀Show a token info:
- Price;
- Circulating supply;
- Market cap;
- Total supply;
- Fully Diluted Value (FVD).

⠀In addition, it allows to calculate the product of the price.

🗣 __Aliases__:
```
/token_info, !token_info
/ti, !ti
```

⚙️ __Usage__ (<ins>underlined</ins> is mandatory):

/ti <ins>SYMBOL</ins> NUMBER

- <ins>SYMBOL</ins> — token symbol
- NUMBER — number to calculate a product

🕹 Examples:
```
/ti eth
📢 Project name: Ethereum
⚛️ Token symbol: ETH

💵 Price: 1 072.61$

🔄 Circulating supply: 119 514 467 ETH 
📊 Market cap: 128 192 413 224$

📈 Total supply: -
💰 Fully Diluted Value (FVD): -
```
```
/ti btc 0.00042
📢 Project name: Bitcoin
⚛️ Token symbol: BTC

💵 Price: 19 432.41$
🧮 Product: 8.16161$

🔄 Circulating supply: 19 082 512 BTC (90.87%)
📊 Market cap: 370 819 197 013$

📈 Total supply: 21 000 000 BTC
💰 Fully Diluted Value (FVD): 408 080 610 000$
```
```
/ti bnb 0,292
/ti sol 1'200
/ti trx 119 272 123.59
```

<h3><p align="center">warning / w</p></h3>

🧰 __Functionality__:

⠀View issued warnings.

🗣 __Aliases__:
```
/warning, !warning
/w, !w
```

⚙️ __Usage__:
```
/w
```

<h1><p align="center">Captcha</p></h1>
<p align="right"><a href="#Content">To the content</a></p>

⠀Types are in descending order of difficulty.

<h2><p align="center">Random</p></h2>

⠀The bot sends random type captcha to a new user (see types below).

<h2><p align="center">Numbers and buttons</p></h2>

⠀A new user must read the message and based on it find a number with a certain ordinal place from the left or right side of the image and press the appropriate button.

⠀Examples:
- Select <ins>the third</ins> digit from <ins>the left side</ins>.
- Select <ins>the fourth</ins> digit from <ins>the right side</ins>.
- Select <ins>the second</ins> digit from <ins>the left side</ins>.
- Select <ins>the third</ins> digit from <ins>the right side</ins>.

<p align="center"><img src="/images/numbers_and_buttons.png"></p>


<h2><p align="center">Letters</p></h2>

⠀A new user must enter 5 letters from the image (i always with a dot).

<p align="center"><img src="/images/letters.png"></p>

<h2><p align="center">Arithmetic</p></h2>

⠀A new user must solve an arithmetic task from image and send the answer (there may be a negative answer).

<p align="center"><img src="/images/arithmetic.png"></p>

<h2><p align="center">None</p></h2>

⠀Users are free to join without having to solve any captcha. This type is recommended during mass joins to the group.

<h1><p align="center">Anti-spam system (BETA)</p></h1>
<p align="right"><a href="#Content">To the content</a></p>

⠀Admitix has anti-spam system which protect crypto groups from spamming. In addition, he immediately bans fake bots (Rose, Group Help, etc.) which join to spam.

⠀Supported languages:
- English;
- Russian.

⠀To help developers improve anti-spam system, please, send the `/report` command as a reply to spam message which got past the system (general users can do it too)! This action will send a message to the developers for further analysis.

<h1><p align="center">I found a bug or have an idea</p></h1>
<p align="right"><a href="#Content">To the content</a></p>

⠀If you found a bug or have an idea, go to [Issue tab](https://github.com/1package/Admitix/issues), click «New issue», select the template and fill it.

<h1><p align="center">Donation</p></h1>
<p align="right"><a href="#Content">To the content</a></p>

⠀You can express your gratitude to the bot developers by sending fund to crypto wallets!
- Ethereum-like address (Ethereum, BSC, Moonbeam, etc.): `0x55AD64372bf4452759D577453521eb502001529A`
- USDT TRC-20: `TQvc5ruZPUSrs7riWeeekka5FjCGAiQ2wE`
- SOL: `8zpWbtTxmubgqcBXHQ129YbZszVp3WUcYc6a34peam3h`
- BTC: `bc1qnuwkg5ph0r8s332kle6jz2qmxe9ls36z9yt9ws`
