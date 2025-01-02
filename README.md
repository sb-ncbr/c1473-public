# Podklady pro praktické příklady v předmětu C1473

Kroky popsané v tomto dokumentu je třeba provést **několik dnů** před začátkem kursu. Vyžadují reakci správců infrastruktury, která může mít jistou prodlevu,
a v den konání už se nestihne.
Bez splnění těchto předpokladů předmět **nelze absolvovat**.

## Přihláška Metacentra

Nemáte-li ještě z jiných důvodů účet v národní infrastruktuře Metacentrum, požádejte o něj vyplněním formuláře https://metavo.metacentrum.cz/cs/application/prihlaska

1. Na tomto vyberte v části "Přímé odkazy na přihlášení přes vybrané instituce" políčko MUNI.
2. Formulář vás přesměruje na stránku jednotného přihlášení MU, tam zadáte své IČO a primární heslo.
3. Po úspěšném přihlášení se dostanete na vlastní formulář přihlášky:
   - Jako důvod k využití infrastruktury uveďte praktická cvičení v předmětu C1473
   - Uživatelské jméno a heslo: pro tento předmět ho potřebovat nebudete, ale zvolte něco smysluplného pro případné budoucí využití (změnit uživatelské jméno je dost komplikované)
   - Příslušnost k instituci uveďte Přírodovědeckou fakultu MU
   - Zkontrolujte správnost předvyplňených osobních údajů
   - Žádné nepovinné položky nevypňujte :-)
4. Vyčkejte na emailové potvrzení, že přihláška byla přijata.

## Start serveru v JupyterHubu

1. Po schválení přihlášky Metacentra přejděte na https://hub.cloud.e-infra.cz/
2. Klikněte na tlačitko přihlášení pomocí e-INFRA CZ AAI
3. Z nabízených možností vyberte opět "Masaryk University" a zadejte UČO a primární heslo
4. Zobrazí se vstupní stránka JupyterHub, na ní vyberte "My Server"
5. Formulář přejde na část "Choosing Image", zvolte variantu "Custom Image" a v ní zadejte `cerit.io/hubs/minimalnb:02-01-2025-ai` a klikněte "Next"
6. V následující části "Choosing storage":
   - Při prvním přístupu vyberte "Persistent Notebook Home" -> "New", vytvoří se váš vlastní pracovní prostor.
   - Při následujícím přístpu volte "Existing" a vyberte variantu `USERNAME-home-default`.
     
   Žádné další volby nezapínejte.
8. V části "Resources" ponechte implicitní nastavení, tj. CPU limit 1, memory limit 4 a "None" pro GPU a klikněte na "Submit"
9. Během nanejvýš několika minut se server nastartuje a formulář vás na něj automaticky přesměruje.

JypyterHub dovoluje jednomu uživateli spustit více serverů a používat více různých pracovních prostorů, ale snažte se to nedělat, dokud jasně nevíte proč, riskujete tím zbytečný zmatek na vlastním písečku.

Nastartovaný server zpravidla běží několik dnů, v tom případě vás na něj tlačítko "My Server" na úvodní straně přímo navede. Jinak při návratu postup zopakujte (s volbou druhé alternativy v kroku 6). 

## Nakopírování podkladů
