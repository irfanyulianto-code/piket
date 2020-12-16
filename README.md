# piket
Make reminder
#!/bin/sh

CHATID="1234"
KEY="1231278846:AAERvQZlVkg_fTuMq4P7LaY3HmrxZHb7ZzQ"
TIME="10"
URL="https://api.telegram.org/bot$KEY/sendMessage"
TEXT="Ayo, sekarang waktunya piket!"

curl -s --max-time $TIME -d "chat_id=$CHATID&disable_web_page_preview=1&text=$TEXT" $URL >/dev/null
