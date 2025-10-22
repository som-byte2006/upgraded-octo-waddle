# upgraded-octo-waddle
MY FIRST PROJECT
import time
import sys
import io

sys.stdout = io.TextIOWrapper(sys.stdout.buffer,encoding ="utf-8")

def print_lyrics():
    lyrics = [
        "যদি বিরহ থা কে আমি ও থাকি...",
        "কে বলো শেষ হবে আগে?....",
        "কেন যে এত ভালোবাসা মরে যায়..",
        "শুধু সময় মনে রাখে...",
        "এত শূন্যতা.... এ মনে রাখি যে আমি...",
        "দেখে না কেউ তো আর, বলে এ সবই পাগলামি....",
        "কাটে না যামিনী, বি রহ যেন কেটে যায়....",
        "থামে না বরষা,তোমারে ডাকি যে আমি..."
    ]

    delays = [0.3, 0.9, 0.2, 0.9, 0.9, 0.2, 0.5, 0.7]

    print("\n Long distance love :\n")
    time.sleep(1)

    for i, line in enumerate(lyrics):
        for char in line:
            sys.stdout.write(char)
            sys.stdout.flush()
            time.sleep(0.11)
        print()  
        time.sleep(delays[i % len(delays)])  


print_lyrics()        
