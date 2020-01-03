# SSH-2FA-Telegram
Two-Factor Authentication for SSH login via Telegram.


## Setup

### Create Your Own Bot:
Chat `@BotFather` with `/newbot`

--------------

### Setup Bot for OTP Sender
- Open your API: `https://api.telegram.org/bot[HTTP_API_KEY]/getUpdates`
- Chat your Telegram Bot
- Copy your `Chat ID`
![BOT Chat ID](https://raw.githubusercontent.com/panophan/SSH-2FA-Telegram/master/BOT-API-GetUpdates.png)
- Download `ssh2FA.bash` source
- Change configuration `API KEY` & `Chat ID` on "ssh2FA.bash" source
- Move `ssh2FA.bash` to `/bin/` (`mv ssh2FA.bash /bin/`)
- `chmod +x /bin/ssh2FA.bash`
- Change shell in `/etc/passwd` => Example `/bin/bash` to `/bin/ssh2FA.bash`
![/etc/passwd](https://raw.githubusercontent.com/panophan/SSH-2FA-Telegram/master/etc-passwd-sample.png)
