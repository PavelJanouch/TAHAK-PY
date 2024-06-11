# Základy Pythonu

## Proměnné a datové typy

```python
# Příklad proměnné a datových typů
x = 5              # celé číslo (integer)
y = 3.14           # desetinné číslo (float)
z = "Hello, world" # řetězec (string)
```

## Základní operace

```python
# Aritmetické operace
soucet = 5 + 3     # sčítání
rozdil = 5 - 3     # odčítání
produkt = 5 * 3    # násobení
podil = 5 / 3      # dělení
modul = 5 % 3      # modulo (zbytek po dělení)
mocnina = 5 ** 3   # umocňování

# Porovnávací operace
vetsi = 5 > 3      # větší než
mensi = 5 < 3      # menší než
stejne = 5 == 3    # rovno
nerovno = 5 != 3   # nerovno

# Logické operace
and_vysledek = True and False  # logické "a"
or_vysledek = True or False    # logické "nebo"
not_vysledek = not True        # logická negace
```

## Podmínky

```python
# Podmínka if
x = 5
if x > 0:
    print("x je kladné číslo")
elif x == 0:
    print("x je nula")
else:
    print("x je záporné číslo")
```

## Smyčky

```python
# Smyčka for
for i in range(5):   # tiskne čísla od 0 do 4
    print(i)

# Smyčka while
x = 0
while x < 5:
    print(x)
    x += 1
```

## Funkce

```python
# Definice funkce
def pozdrav(jmeno):
    print("Ahoj, " + jmeno + "!")
    
# Volání funkce
pozdrav("Petr")
```

## Seznamy (Lists)

```python
# Vytvoření seznamu
seznam = [1, 2, 3, 4, 5]

# Přístup k prvkům seznamu
prvni_prvek = seznam[0]  # prvni_prvek = 1
posledni_prvek = seznam[-1]  # posledni_prvek = 5

# Slicing seznamu
cast_seznamu = seznam[1:3]  # cast_seznamu = [2, 3]

# Iterace přes seznam
for prvek in seznam:
    print(prvek)
```

## Slovníky (Dictionaries)

```python
# Vytvoření slovníku
slovnik = {"jablko": "apple", "hruška": "pear", "broskev": "peach"}

# Přístup k hodnotám ve slovníku
anglicky_nazev = slovnik["jablko"]  # anglicky_nazev = "apple"

# Iterace přes klíče a hodnoty
for klic, hodnota in slovnik.items():
    print(klic, hodnota)
```

## Třídy (Classes)

```python
# Definice třídy
class Auto:
    def __init__(self, znacka, barva):
        self.znacka = znacka
        self.barva = barva

    def info(self):
        print("Auto znacky", self.znacka, "je", self.barva + ".")
```

## Importování modulů

```python
# Importování celého modulu
import math
print(math.pi)

# Importování specifického obsahu
from math import sqrt
print(sqrt(16))
```

## Práce se soubory

```python
# Čtení ze souboru
with open("soubor.txt", "r") as soubor:
    obsah = soubor.read()
    print(obsah)

# Zápis do souboru
with open("novy_soubor.txt", "w") as soubor:
    soubor.write("Ahoj, světe!")
```

## Práce se vstupem a výstupem

```python
# Vstup od uživatele
jmeno = input("Jak se jmenuješ? ")
print("Ahoj, " + jmeno + "!")

# Formátovaný výstup
cislo = 3.14159
print(f"Pi s přesností na dvě desetinná místa je {cislo:.2f}.")
```

## Parsování JSON

```python
import json

# JSON řetězec
json_data = '{"name": "John", "age": 30, "city": "New York"}'

# Parsování JSON
data = json.loads(json_data)
print("Jméno:", data["name"])
print("Věk:", data["age"])
print("Město:", data["city"])
```

## Práce s API

```python
import requests

# Získání dat z API
response = requests.get("https://api.example.com/data")
data = response.json()

# Zpracování dat
for item in data:
    print(item)
```
