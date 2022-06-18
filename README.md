# SMS-Alerts

The purpose of this repo is to demonstrate the ability to combine text alerts with common automation scripts.

## Getting Started

Clone the repo:

```bash
git clone https://github.com/AshleyNikr/SMS-Alerts.git
```

Create a new Gmail account (recommended) or use an existing one:

[Gmail signup](https://accounts.google.com/signup/v2/webcreateaccount?service=mail&continue=https%3A%2F%2Fmail.google.com%2Fmail%2Fu%2F0%2F&dsh=S571141601%3A1655573958454104&biz=false&flowName=GlifWebSignIn&flowEntry=SignUp)

Go to manage your Gmail account:

![Manage Gmail]("images/manage\ account.png")

Enable 2-step verification:

![2-step]("images/2-step\ verification.png")

Add an app password:

![App Password]("images/app\ password.png")

Copy that password into .env, replacing the placeholder password:

Find your carrier from the list bellow:

- AT&T: number@txt.att.net (SMS), number@mms.att.net (MMS)
- Boost Mobile: number@sms.myboostmobile.com (SMS), number@myboostmobile.com (MMS)
- C-Spire: number@cspire1.com
- Consumer Cellular: number@mailmymobile.net
- Cricket: number@sms.cricketwireless.net (SMS), number@mms.cricketwireless.net (MMS)
- Google Fi (Project Fi): number@msg.fi.google.com (SMS & MMS)
- Metro PCS: number@mymetropcs.com (SMS & MMS)
- Mint Mobile: number@mailmymobile.net (SMS)
- Page Plus: number@vtext.com (SMS), number@mypixmessages.com (MMS)
- Red Pocket: Red Pocket uses AT&T or T-Mobile (for GSM SIMs) & Verizon for CDMA. See info. for those carriers.
- Republic Wireless: number@text.republicwireless.com (SMS)
- Simple Mobile: number@smtext.com (SMS)
- Sprint: number@messaging.sprintpcs.com (SMS), number@pm.sprint.com (MMS)
- T-Mobile: number@tmomail.net (SMS & MMS)
- Ting: number@message.ting.com (SMS for CDMA), number@tmomail.net (SMS for GSM)
- Tracfone: number@mmst5.tracfone.com (MMS)
- U.S. Cellular: number@email.uscc.net (SMS), number@mms.uscc.net (MMS)
- Verizon: number@vtext.com (SMS), number@vzwpix.com (MMS)
- Virgin Mobile: number@vmobl.com (SMS), number@vmpix.com (MMS)
- Visible: number@vtext.com (SMS), number@vzwpix.com (MMS)
- Xfinity Mobile: number@vtext.com (SMS), number@mypixmessages.com (MMS)

Copy the text after `number@` and replace the carrier placeholder in .env

Run the python script directly:

```bash
python3 sms.py --body "\nHello, World!"
```

Wait for the message to show up on your phone!

Run the update script:

```bash
sudo ./update.sh
```
