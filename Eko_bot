import telebot

bot = telebot.TeleBot("TOKEN")

@bot.message_handler(commands=['start'])
def send_welcome(message):
    bot.reply_to(message, "Привет! Я ваш Telegram бот, который может дать вам совет, как правильно подготовить и утилизовать бытовые отходы.")

@bot.message_handler(commands=['help'])
def send_welcome2(message):
    f = open("comands.txt","r", encoding = "utf-8")
    text = f.read()
    f.close()
    bot.reply_to(message, text)

@bot.message_handler(commands=['wastes'])
def send_wastes(message):
    f = open("wastes.txt","r", encoding = "utf-8")
    text = f.read()
    f.close()
    bot.reply_to(message, text)

@bot.message_handler(commands=['organic_waste'])
def send_organic_waste(message):
    f = open("organic_waste.txt","r", encoding = "utf-8")
    text = f.read()
    f.close()
    bot.reply_to(message, text)

@bot.message_handler(commands=['recyclable_materials'])
def send_recyclable_waste(message):
    f = open("recyclable_materials.txt","r", encoding = "utf-8")
    text = f.read()
    f.close()
    bot.reply_to(message, text)

@bot.message_handler(commands=['dangerous_waste'])
def send_dangerous_waste(message):
    f = open("danger_waste.txt","r", encoding = "utf-8")
    text = f.read()
    f.close()
    bot.reply_to(message, text)

@bot.message_handler(commands=['bulky_waste'])
def send_bulky_waste(message):
    f = open("bulky_waste.txt","r", encoding = "utf-8")
    text = f.read()
    f.close()
    bot.reply_to(message, text)

@bot.message_handler(func=lambda message: True)
def echo_all(message):
    bot.reply_to(message, message.text)

bot.polling()
