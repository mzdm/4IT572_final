**Informace k závěrečnému projektu**:

s využitím našeho e-shopu, GitHub Actions, Docker a Ansible **sestavit pipeline**.

- [x] Pipeline bude rozdělena na dvě větve.
    - [x] Pokud otevřu pull request z nějaké branche do masteru,
        - [x] sestaví se mi eshop,
        - [x] otestuje a
        - [x] povolí mi mergnout kód do masteru.
    - [x] Pokud neprojde, bude merge blokován.
    - [x] V okamžiku merge do masteru se spustí workflow,
        - [x] které kromě kroků z předchozího scénáře ještě
        - [x] nasadí eshop pomocí Ansible na EC2.
        - [x] Po doběhnutí GHA workflow z masteru se vám tedy pokaždé vytvoří nová instance EC2, **zůstane vám tam ale i ta stará**.
        - [ ] Poslední částí toho úkolu je **automatické mazání té staré instance**. To zajistíte jako další krok ve vašem Ansible playbooku.
- [x] Při vypracování projektu chci abyste dbali na správnou práci s klíči a pem klíčem do AWS. Kdo bude mít všechny tyto věci v hardcodované a pem v repozitáři, bude za to penalizován 5body.