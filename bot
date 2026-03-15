import telebot
import time
import os

TOKEN = os.environ.get('8656708043:AAHhgbNl22w-ex7YUKFvYdecEHQe_lRsGXM')  # Берет токен из Render
bot = telebot.TeleBot(TOKEN)

@bot.message_handler(commands=['start'])
def start(msg):
    bot.reply_to(msg, "✅ Бот работает!")

print("✅ Бот запущен!")

while True:
    try:
        bot.infinity_polling(timeout=60)
    except:
        time.sleep(5)
