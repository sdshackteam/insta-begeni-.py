import requests
import random
import os
os.system('pip install pyfiglet')
os.system('pip install requests')
os.system('pip install webbrowser')
os.system('pip install user_agent')
os.system('pip install getuseragent')
os.system('clear')
import requests
import random
import pyfiglet
import sys
import time
from random import randint
from user_agent import generate_user_agent as ua
from getuseragent import UserAgent
E = '\x1b[1;31m'
B = '\x1b[2;36m'
G = '\x1b[1;32m'
S = '\x1b[1;33m'
Ab = '\x1b[1;92m'
aB = '\x1b[1;91m'
AB = '\x1b[1;96m'
aBbs = '\x1b[1;93m'
AbBs = '\x1b[1;95m'
A_bSa = '\x1b[1;31m'
a_bSa = '\x1b[1;32m'
faB_s = '\x1b[2;32m'
a_aB_s = '\x1b[2;39m'
Ba_bS = '\x1b[2;36m'
Ya_Bs = '\x1b[1;34m'
S_aBs = '\x1b[1;33m'
attemps = 0
os.system('clear')
attemps += 1

def to(s):
    for char in s + '\n':
        sys.stdout.write(char)
        sys.stdout.flush()
        time.sleep(0.0625)
        return None
        return None

ua = UserAgent('ios').Random()
user = input('[+] InstaGram Kullanici Adi : ')
link = input('[+] Gonderi Linki : ')
print('')
res = requests.post('https://api.likesjet.com/freeboost/7', json = {
    'instagram_username': user,
    'link': link,
    'email': f'''srk{random.randint(100000, 999999)}@gmail.com''' }, headers = {
    'Host': 'api.likesjet.com',
    'content-length': '137',
    'sec-ch-ua': '"Google Chrome";v="119", "Chromium";v="119", "Not?A_Brand";v="24"',
    'accept': 'application/json, text/plain, */*',
    'content-type': 'application/json',
    'sec-ch-ua-mobile': '?1',
    'user-agent': ua,
    'sec-ch-ua-platform': '"Android"',
    'origin': 'https://likesjet.com',
    'sec-fetch-site': 'same-site',
    'sec-fetch-mode': 'cors',
    'sec-fetch-dest': 'empty',
    'referer': 'https://likesjet.com/',
    'accept-language': 'en-XA,en;q=0.9,ar-XB;q=0.8,ar;q=0.7,en-GB;q=0.6,en-US;q=0.5' }).json()
print(res['message'])
print('\x1b[38;5;82m: \x1b[31;1m[√] SDS Team tarafindan begeni gonderildi. İnsta: @sadwp.official, 24 saatte bir kullanilabilir')


