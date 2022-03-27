#www.philiphacker.in
import os
os.system("clear")
print("\n Youtube Audio Downloader \n")
url = input(" Enter URL : ")
print("\n Fetching Audio.. Please wait..\n")
id = os.popen('youtube-dl --get-id ' + url).read().strip()
os.system("clear")
print("\nChoose Audio Speed to download,\n")
print(" 1 - Speed 0.5 x ")
print(" 2 - Speed 1.0 x ")
print(" 3 - Speed 1.5 x ")
print(" 4 - Speed 2.0 x ")
print(" 5 - Speed 2.5 x ")
print(" 6 - Speed 3.0 x ")
print(" 7 - Custom Speed ")
print(" 8 - About Tool ")
print(" 9 - Visit Website ")
print(" 0 - Exit Tool ")
x = input("\nEnter your Choice : ")
if x == "1":
    speed = "0.5"
elif x == "2":
    speed = "1.0"
elif x == "3":
    speed = "1.5"
elif x == "4":
    speed = "2.0"
elif x == "5":
    speed = "2.5"
elif x == "6": #www.philiphacker.in
    speed = "3.0"
elif x == "7":
    y = input("Enter custom speed (0.1 - 10.0) : ")
    speed = y
elif x == "8":
    os.system("clear")
    print("\n This tool will download youtube audio in different speed. This tool is made by Philiphacker. Especially for Asif one of our Techno World group mate..\n")
    exit()
elif x == "9":
    print("\n Opening Website..\n")
    os.system('xdg-open https://philiphacker.in')
    exit()
elif x == "0" or x == "x":
    os.system("clear")
    print("\n www.philiphacker.in\n")
    exit()
else:
    print("\n Invalid Choice !\n")
    exit()
print("")
os.system('youtube-dl -x --audio-format mp3 -o "/sdcard/download/www.philiphacker.in/' + id + '.mp3" ' + url)
os.system('ffmpeg -i "/sdcard/download/www.philiphacker.in/' + id + '.mp3" -filter:a "atempo=' + speed + '" -c:a libmp3lame -q:a 4 "/sdcard/download/www.philiphacker.in/' + speed + 'x_' + id + '.mp3"')
try:
    os.remove("/sdcard/download/www.philiphacker.in/"+id+".mp3")
except FileNotFoundError:
    os.system("clear")
    print("\n Invalid Youtube URL : "+url+" !\n")
    exit()
os.system("clear")
print("\n Downloaded Successfully ✓")
print("\n Audio Stored in,\n\n Internal/download/www.philiphacker.in/(here)\n\n")
