from telegram import Update
from telegram.ext import Application, CommandHandler, ContextTypes

TOKEN = "8690137750:AAH-I83MfuPxaFHrbRI5fjbBTrgOKH8VK7EYO" 

async def start(update: Update, context: ContextTypes.DEFAULT_TYPE):
    await update.message.reply_text(
        "Salom! Jaxon tillari bot ishlayapti 🚀"
    )

app = Application.builder().token(TOKEN).build()
app.add_handler(CommandHandler("start", start))

app.run_polling()# jaxon-tillari-bot-
Multi-language Telegram bot with translation, lessons, and voice support (Uzbek, Russian, English, German, Korean).# jaxon-tillari-bot-
Multi-language Telegram bot with translation, lessons, and voice support (Uzbek, Russian, English, German, Korean).
