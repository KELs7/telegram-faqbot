# A Keyword-based FAQ Telegram Bot
(FAQ = Frequently Asked Questions)

**This bot enables you to map a keyword (as an area of query) to answers and it is easy to use.**

demo
![](demo_480.gif)

1. Clone the repo
`git clone https://github.com/KELs7/telegram-faqbot.git`

2. Ensure httpx, python-decouple, and ujson are installed (with pip).

3. configure your .env file
```
BOT_TOKEN=<YOUR TELEGRAM BOT TOKEN>
ADMIN=<YOUR TELEGRAM ID>
```
Your telegram id is needed so you can be the only one to be able to configure your FAQs.

4. Add bot to group

5. Run bot
`python3 faq_bot.py`

NB: Python 3.10.6 was used to run the bot in its development

6. Create and send a json file to the faq bot in private chat on Telegram
faq.json
```
{
    about_us: "We are a crypto enthusiast with the vision to revoluntarise the meme token",
    listing: "We are listed on gecko. We have plans to list token on Binance",
    help: "Keywords:\n\nabout us - info on project\nlisting - info on listing\n\nHow to use: /faq <KEYWORD>"
}
```
NB: 'help' entry in the json file is mandatory

Edit and resend json file to faq bot if you want to update your FAQs

7. Go to group and test e.g `/faq about_us`

## Limitations
* No greeter to prompt new members about questions that can be answered right away
* No support for Markdown or html text styling
* No dashboard to present user stats
* No webhook support (uses long polling)

This is a free product with limited features unlike the premium version. 
