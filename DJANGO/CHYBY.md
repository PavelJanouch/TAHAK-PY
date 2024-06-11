# Nejčastější chyby v Django a jejich řešení

## 1. ImproperlyConfigured: settings.DATABASES je neplatné

- **Popis:** Tato chyba se objeví, když je nastavení databáze neplatné nebo neexistující.
- **Řešení:** Zkontrolujte soubor settings.py a ujistěte se, že máte správně nastavené připojení k databázi, včetně názvu databáze, uživatelského jména a hesla.

## 2. TemplateDoesNotExist: Šablona neexistuje

- **Popis:** Tato chyba se objeví, když Django nenajde požadovanou šablonu pro zobrazení.
- **Řešení:** Ujistěte se, že cesta k šabloně je správně definována v pohledech a že soubory šablon jsou umístěny ve správných adresářích.

## 3. NoReverseMatch: Reverse for 'view_name' not found

- **Popis:** Tato chyba se objeví, když Django nemůže najít URL adresu pro zadaný pohled.
- **Řešení:** Zkontrolujte, zda máte správně nastavené URL routy v souboru urls.py a zda používáte názvy pohledů, které existují.

## 4. ImproperlyConfigured: settings.AUTH_USER_MODEL musí být zadané

- **Popis:** Tato chyba se objeví, když není správně nastavené vlastní uživatelské model ve vašem projektu Django.
- **Řešení:** Ujistěte se, že máte správně nastavené vlastní uživatelské model v settings.py pomocí proměnné AUTH_USER_MODEL.

## 5. ForeignKeyConstraintError: IntegrityError - klíč cizího klíče neexistuje

- **Popis:** Tato chyba se objeví, když se snažíte vytvořit záznam v tabulce s cizím klíčem, který odkazuje na neexistující záznam v jiné tabulce.
- **Řešení:** Ujistěte se, že existují záznamy v rodičovské tabulce, než vytvoříte záznamy v tabulce s cizím klíčem, nebo použijte `null=True` nebo `on_delete=models.SET_NULL` pro nastavení nulovatelnosti cizího klíče.

## 6. AttributeError: 'module' object has no attribute 'xxx'

- **Popis:** Tato chyba se objeví, když se pokoušíte přistoupit k atributu, který neexistuje v modulu.
- **Řešení:** Zkontrolujte názvy importovaných modulů a objektů a ujistěte se, že jsou správně napsány.

## 7. TypeError: 'xxx' is not iterable

- **Popis:** Tato chyba se objeví, když se pokusíte iterovat přes objekt, který není iterovatelný.
- **Řešení:** Ujistěte se, že iterujete přes správný typ objektu a že je správně inicializován.

## 8. ProgrammingError: Relation 'xxx' already exists

- **Popis:** Tato chyba se objeví, když se pokoušíte vytvořit tabulku, která již existuje v databázi.
- **Řešení:** Zkontrolujte, zda tabulka již neexistuje v databázi, a pokud ano, buď ji smažte a znovu migrujte, nebo upravte migrace tak, aby nevytvářely existující tabulky.

## 9. SuspiciousOperation: Attempted access to 'xxx' denied

- **Popis:** Tato chyba se objeví, když uživatel nemá oprávnění k přístupu k určitému zdroji.
- **Řešení:** Zkontrolujte nastavení oprávnění a ujistěte se, že uživatel má oprávnění k přístupu k danému zdroji.

## 10. Internal Server Error (500)

- **Popis:** Tato chyba se objeví, když server narazí na interní chybu, kterou nedokáže zpracovat.
- **Řešení:** Zkontrolujte logy serveru a Django pro podrobnosti o chybě a pokuste se ji identifikovat a opravit.
