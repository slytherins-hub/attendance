# Prezenční listina

### Úkol 1
* Naklonuj si obsah tohoto repozitáře.
  ```
  https://github.com/slytherins-hub/attendance.git
  ```
* Přepni se do naklonované složky a zkontroluj historii repozitáře (např. pomocí `gitk --all` nebo `git log --oneline`).
* V pracovním adresáři repozitáře vytvoř prázdný textový soubor a ulož ho pod svým jménem `jmeno_prijmeni.txt`. Nepoužívej diaktritiku.
* Vytvoř novou revizi:
  ```
    git add jmeno_prijmeni.txt
    git commit
  ```
* Na GitHubu na stránce repozitáře klikni vpravo nahoře na tlačítko <kbd>Fork</kbd>. Vytvoří se kopie tohoto repozitáře na tvém účtu:
  `https://github.com/tvuj-ucet/attendance`
* V příkazové řádce přidej do Gitu zkratku k tvému vzdálenému repozitáři:
  ```
  git remote add muj_fork https://github.com/tvuj-ucet/prezencka
  ```
* Pošli změny na tvúj vzdálený repozitář:
  ```
  git push muj_fork main
  ```
* Na stránce tvého repozitáře se nahoře objeví možnost <kbd>Contribute</kbd> a po rozkliknutí <kbd>Open pull request</kbd>.
  Otevřete tedy nový pull request, zkontrolujte popisek změny a potvrďte ho <kbd>Create pull request</kbd>.
* V případě, že autor repozitáře změny přijme, provede jejich začlenění do původního repozitáře.
  Stáhni si aktuální verzi repozitáře:
  ```
  git pull origin main
  ```
* Ověř stav repozitáře a zkontroluj jeho historii:
  ```
  git status
  gitk --all
  git log --oneline
  ```


### Úkol 2
V souboru, který jsi přidal/a do repozitáře, doplň, jakou máš dnes náladu.

* V repozitáři vytvoř novou větev:
  ```
  git branch nazev_vetve
  ```
* Přepni se do nově vytvořené větve:
  ```
  git switch nazev_vetve
  ```
* V souboru se svým jménem proveď potřebné změny.
* Vytvoř novou revizi.
* Pošli změny do svého vzdáleného repozitáře:
  ```
  git push vase_jmeno nazev_vetve
  ```
* Na GitHubu vytvoř pull request.
* Po začlenění tvých změn:
    * Přepni se zpět na hlavní větev:

      ```
      git switch main
      ```
    * Stáhni aktuální verzi repozitáře:

      ```
      git pull origin main
      ```
    * Smaž větev, na které jsou začleněné změny:

      ```
      git branch -d nazev_vetve
      ```
