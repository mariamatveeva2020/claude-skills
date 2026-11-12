# Telegram Notifier

A personal Telegram bot that sends me short status messages. Any script, scheduled task or Claude session can use it. There is no server and nothing running in the background: each message is one call to the Telegram Bot API.

## What the skill does

1. Walks through creating the bot in @BotFather and naming it.
2. Finds the chat ID the bot should write to.
3. Copies a tested sending script into the project. Python standard library only, nothing to install.
4. Keeps the bot token in a local `.env` file, never in code or in git.
5. Sends a test message and waits for confirmation that it arrived before calling the setup done.
6. Shows how to hook it up: from a script, at the end of a Claude Code task, or from a scheduled check.

## Writing rules the bot follows

Messages are read on a phone, so the skill keeps them short:

- One event, one message.
- The first line is the result or the blocker, not the process.
- Two to four lines in total, plain words, no error codes.
- At most one or two status emoji.

## Sample messages

> ✅ Daily data capture done
> Two screenshots saved to the Claude folder.

> ⚠️ Couldn't open the source page
> The site didn't respond. I'll try again tomorrow morning.

> ⏳ Contract review needs your input
> Which party are you in this lease, tenant or guarantor?
