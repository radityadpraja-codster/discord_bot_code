import discord
from discord.ext import commands

inetents = discord.Intents.default()
inetents.message_content = True

bot = commands.Bot(command_prefix='$', intents=inetents)

@bot.event
async def on_ready():
    print(f'login sebagai {bot.user}')

@bot.command()
async def sampah(ctx, *, benda):
    benda = benda.lower()

    organik = [
        "sisa makanan",
        "buah",
        "bangkai hewan",
        "daunan"
    ]

    anorganik = [
        "plastik",
        "kaca",
        "kaleng",
        "besi"
    ]

    b3 = [
        "baterai",
        "lampu neon",
        "cat",
        "obat-obatan"
    ]

    if benda in organik:
        await ctx.send(f"{benda} termasuk sampah organik dan cara menguranginya bisa dengan kompos")
    elif benda in anorganik:
        await ctx.send(f"{benda} termasuk sampah anorganik dan cara menguranginya bisa dengan daurulang")
    elif benda in b3:
        await ctx.send(f"{benda} termasuk sampah B3 dan cara menguranginya bisa dengan penanganan khusus")
    else:
        await ctx.send(f"{benda} sampah tidak diketahui")

bot.run('bro, you really thought i would leak my token?')
