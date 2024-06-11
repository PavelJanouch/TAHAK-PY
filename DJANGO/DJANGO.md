# Django - Kompletní přehled

## Co je Django?

Django je open-source webový framework napsaný v Pythonu. Je navržen tak, aby usnadnil tvorbu komplexních webových aplikací rychle a efektivně. Django je známý svou škálou, bezpečností a schopností rychle vytvářet plnohodnotné webové aplikace.

## Klíčové vlastnosti

- **ORM (Object-Relational Mapping):** Django poskytuje vlastní ORM, které umožňuje komunikaci s databází pomocí objektově orientovaných konstrukcí.
- **Administrační rozhraní:** Django zahrnuje vestavěné administrační rozhraní, které umožňuje správu databáze a obsahu vaší aplikace přímo z prohlížeče.
- **URL routing:** Django používá koncept URL routing k mapování URL adres na jednotlivé části vaší aplikace.
- **Šablony:** Django podporuje použití šablon pro oddělení logiky prezentace od logiky aplikace.
- **Bezpečnostní funkce:** Django má v sobě zabudované funkce pro zajištění bezpečnosti vaší aplikace.
- **Autentizace a autorizace:** Django poskytuje vestavěné nástroje pro autentizaci a autorizaci uživatelů.

## Struktura projektu Django

- **Settings.py:** Soubor obsahující nastavení vaší aplikace.
- **Urls.py:** Soubor, který obsahuje definice URL adres.
- **Views.py:** Soubor, kde jsou definovány funkce pohledů.
- **Models.py:** Soubor, kde jsou definovány modely databáze.
- **Templates:** Složka obsahující HTML šablony vaší aplikace.

## Instalace Django

Pro instalaci Django můžete použít pip, balíčkovací systém pro Python:

```python
pip install django
```

## Vytvoření projektu Django

Pro vytvoření nového projektu Django použijte příkaz `django-admin`:

```python
django-admin startproject nazev_projektu
```

## Spuštění vývojového serveru

Po vytvoření projektu můžete spustit vývojový server pomocí příkazu:

```python
python manage.py runserver
```

## Další kroky

Po vytvoření projektu můžete začít definovat URL adresy, vytvářet pohledy a modely a vytvářet šablony pro vaši aplikaci.
