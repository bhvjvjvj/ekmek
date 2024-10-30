import discord
import random
import os
from discord.ext import commands

intents = discord.Intents.default()
intents.message_content = True
bot = commands.Bot(command_prefix='?', intents=intents)
@bot.event
async def on_ready():
    print(f'{bot.user} olarak giriş yaptık')
@bot.command()
async def cntt(ctx):
    await ctx.send("Çöplerini çöp kutusuna geri,dönüşümleri geri dönüşüm kutusuna atabilirsin")
@bot.command()
async def kignny(ctx):
    await ctx.send("etrafta çevreye zarar veren insanlar gördüğün zaman onları nazikçe uyarabilirsin")
bot.run("token")
