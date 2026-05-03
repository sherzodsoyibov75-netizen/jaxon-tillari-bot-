import os
from telegram import Update
from telegram.ext import Application, CommandHandler, ContextTypes

TOKEN ="8690137750:AAH-I83MfuPxaFHrbRI5fjbBTrgOKH8VK7E"

async def start(update: Update, context: ContextTypes.DEFAULT_TYPE):
    await update.message.reply_text("Salom! Jaxon tillari bot ishlayapti 🚀")

app = Application.builder().token(TOKEN).build()
app.add_handler(CommandHandler("start", start))

app.run_polling()
