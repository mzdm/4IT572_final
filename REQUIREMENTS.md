**Informace k závěrečnému projektu**:

s využitím našeho e-shopu, GitHub Actions, Docker a Ansible **sestavit pipeline**.

- [ ] Pipeline bude rozdělena na dvě větve.
    - [ ] Pokud otevřu pull request z nějaké branche do masteru,
        - [ ] sestaví se mi eshop,
        - [ ] otestuje a
        - [ ] povolí mi mergnout kód do masteru.
    - [ ] Pokud neprojde, bude merge blokován.
    - [ ] V okamžiku merge do masteru se spustí workflow,
        - [ ] které kromě kroků z předchozího scénáře ještě
        - [ ] nasadí eshop pomocí Ansible na EC2.
        - [ ] Po doběhnutí GHA workflow z masteru se vám tedy pokaždé vytvoří nová instance EC2, **zůstane vám tam ale i ta stará**.
        - [ ] Poslední částí toho úkolu je **automatické mazání té staré instance**. To zajistíte jako další krok ve vašem Ansible playbooku.
- [ ] Při vypracování projektu chci abyste dbali na správnou práci s klíči a pem klíčem do AWS. Kdo bude mít všechny tyto věci v hardcodované a pem v repozitáři, bude za to penalizován 5body.