Oddelovac1 = ("=" * 30)
Oddelovac2 = ("=" * 50)
Oddelovac3 = ("=" * 40)

# 1.Privitani uzivatele
print(Oddelovac1)
print("Welcome to Text Analyzer")
print(Oddelovac1)

name_pass = { "bob" : "123", "ann" : "pass123", "mike" : "password", "liz" : "pass123"}

# 2. Vyzadani prihlasovacich udaji a hesla
user_name = input("Please enter your user name: ")
password = input("Please enter your password: ")

# 3. Overeni udaju
if user_name in name_pass.keys() and password in name_pass.values():
    print("Access granted :) ")
else:
    print("Wrong name or password")
    exit()

print(f"Your user name is: {user_name}")
print(f"Your pasword is: '***' ")

# 4.vyber Textu
print(Oddelovac2)
print("You can choose from three texts: " "1","2","3" )
print(Oddelovac2)

TEXTS = ['''
Situated about 10 miles west of Kemmerer, 
Fossil Butte is a ruggedly impressive 
topographic feature that rises sharply 
some 1000 feet above Twin Creek Valley 
to an elevation of more than 7500 feet 
above sea level. The butte is located just 
north of US 30N and the Union Pacific Railroad, 
which traverse the valley. ''',

'''
At the base of Fossil Butte are the bright 
red, purple, yellow and gray beds of the Wasatch 
Formation. Eroded portions of these horizontal 
beds slope gradually upward from the valley floor 
and steepen abruptly. Overlying them and extending 
to the top of the butte are the much steeper 
buff-to-white beds of the Green River Formation, 
which are about 300 feet thick.''',

'''
The monument contains 8198 acres and protects 
a portion of the largest deposit of freshwater fish 
fossils in the world. The richest fossil fish deposits 
are found in multiple limestone layers, which lie some 
100 feet below the top of the butte. The fossils 
represent several varieties of perch, as well as 
other freshwater genera and herring similar to those 
in modern oceans. Other fish such as paddlefish, 
garpike and stingray are also present.''']

# 4a.vypsani odstavcu
for Y in TEXTS:
    print(Y)
print(Oddelovac2)

# 4b. vyber textu uzivatelem
vybrany_odstavec = int(input("Please choose your text 1, 2, 3: "))
print(Oddelovac2)
if vybrany_odstavec > 3:
    print("You choosed wrong text")
    exit()
else:
    vybrany_odstavec = TEXTS[vybrany_odstavec - 1]
    print(f'You choosed text: {vybrany_odstavec}')
    print(Oddelovac2)

rozdeleni = vybrany_odstavec.split()
vycistena_slova = [slovo.strip("., ") for slovo in rozdeleni]  # list comprehension

# 5. Statistiky

print(Oddelovac3)
print(f"There are {(len(vycistena_slova))} words in the selected text." )
print(Oddelovac3)

pocet_slov_zacinajici_velkym_pismen = 0
pocet_slov_velkym_pismem = 0
pocet_slov_malym_pismem = 0
pocet_cifer = 0

for x in vycistena_slova:
    if x.istitle():
        pocet_slov_zacinajici_velkym_pismen += 1
    if x.isupper():
        pocet_slov_velkym_pismem += 1
    if x.islower():
        pocet_slov_malym_pismem += 1
    if x.isnumeric():
        pocet_cifer += 1

print(f"There are {pocet_slov_zacinajici_velkym_pismen} titlecase words.")
print(Oddelovac1)
print(f"There are {pocet_slov_velkym_pismem} uppercase words.")
print(Oddelovac1)
print(f"There are {pocet_slov_malym_pismem} lowercase words.")
print(Oddelovac1)
print(f"There are {pocet_cifer} numeric strings.")
print(Oddelovac1)

#6. Sloupcový graf

slovo={}

for i in vycistena_slova:
    slovo[len(i)] = slovo.setdefault(len(i), 0) + 1
nejcastejsi = sorted(slovo, key=slovo.get, reverse=True)
for i in nejcastejsi:
    print(i, slovo.get(i) * "*", slovo.get(i), "x")

#7. Součet všech čisel
print(Oddelovac2)
soucet_cisel=[]

for i in vycistena_slova:
    if i .isnumeric():
        soucet_cisel.append(int(i))
print(f"If we summed all the numbers in this text we would get: {sum(soucet_cisel)}.")
print(Oddelovac2)
print("Thank you for using Text Analyzer.")
print(Oddelovac2)











