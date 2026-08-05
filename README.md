# AI Number Blocklist

A community-maintained blocklist of phone numbers used by AI calling services, robocallers, and automated dialing systems. Intended for religious communities and anyone else who wants to keep AI-generated calls off their phones.

## What's in this repo

- `blacklist.txt` — one phone number per line in E.164 format (e.g. `+12013759200`). Currently contains **44,192 numbers**.

## Usage

The list is plain text, so it works with any tool that accepts a number list:

- **iPhone / Android call-blocking apps** — import the list into apps that support bulk number blocking.
- **Carrier-level blocking** — submit numbers to your carrier's spam-blocking service.
- **PBX / VoIP systems** — load into Asterisk, FreePBX, 3CX, or similar inbound-route blacklists.
- **Kosher phone providers / filtering services** — integrate directly into filtering platforms.

### Example: download the raw list

```
https://raw.githubusercontent.com/Shalom-Karr/AI-Number-Blocklist/main/blacklist.txt
```

## Format

- One number per line
- E.164 format: `+` followed by country code and national number, no spaces or dashes
- Mostly US/Canada (`+1`) numbers, with some international entries

## Contributing

Found an AI caller not on the list? Open a pull request adding the number to `blacklist.txt` in E.164 format, or open an issue with the number and where the call came from.

To report a false positive (a legitimate number on the list), open an issue and it will be reviewed for removal.

## Disclaimer

Numbers are collected from community reports. Robocallers frequently spoof caller ID, so a listed number may occasionally belong to a legitimate caller. Use at your own discretion.
