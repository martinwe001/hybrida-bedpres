# Git Workshop

Dette repoet inneholder tre velkjente sanger, hver lagret i sin txt-fil. Dere skal nå sammarbeide to og to for å fullføre sangene i utvikler-fashion :)

Gå sammen to og to og start på oppgavene under. Gjør gjerne oppgavene sammen, selv om de refereres til hver av dere.

## Oppgave 1

**Person 1:**

- Sjekk at du er logget inn i GitHub og trykk på `fork` øverst i høyre hjørne.
- På siden som kommer opp, skriv inn et navn for repoet, for eksempel `hybrida-bedpres`
- Trykk på `Create fork`

Nå har person 1 laget en kopi/fork av repoet i sin GitHub. Neste steg er at Person 1 gir sin kjære samarbeidspartner tilgang til repoet. Dette gjøres ved å:

- Gå til `Settings` i menyen i repoet på GitHub
- Trykk på `Collaborators`
- Under `Manage Access`, trykk på `Add People`
- Skriv inn brukernavnet på Person 2 og trykk `Add to this repository`

Nå er alt klart for at dere kan bruke Git til effektivt samarbeid.

## Oppgave 2

**Både Person 1 og Person 2:**

- Åpne terminalen på hver deres maskin og naviger til Desktop.
- Clone repoet lokalt på hver deres maksin ved å kjøre følgende kommando i terminalen (bytt ut <person_1_username> med GitHub-brukernavnet til Person 1 og <repo_name> med navnet på repoet dere velgte i Oppgave 1):

```
git clone https://github.com/<person_1_username>/<repo_name>.git
```

## Oppgave 3

Når flere samarbeider på et prosjekt med Git er det vanlig å lage hver sin `branch` hvor man gjør endringer på en kopi av koden. Dette som en trygghet på at man kan gjøre feil uten at det påvirker andre på prosjektet.

Dere skal nå lage hver deres branch og fullføre sangtekstene nu klinger og ja vi elsker. For å sjekke hvilke branches som finnes kjør følgende kommando i terminalen:

```
git branch
```

Skriv `q` for å gå ut at branch-visningen.

**Person 2:**

Person 2 skal endre nu_klinger.txt, men først må det lages en ny branch hvor endringene kan gjøres. Lag en ny branch kalt `nu_klinger` ved å kjøre følgende kommando i terminalen:

```
git branch nu_klinger
```

Bytt til den nye branchen ved å kjøre følgende kommando i terminalen:

```
git switch nu_klinger
```

Nå kan Person 2 åpne filen nu_klinger.txt og lime inn refrenget (vist under) i bunn av filen.

> Studenter i den gamle stad, ta vare på byens ry! (klapp x2)
> Husk på at jenter, øl og dram var kjempenes meny.
> Og faller I alle mann alle, skal det gjalle fra alle mot sky.
> La'kke byen få ro, men la den få merke den er en studenterby.
> Og øl og dram, og øl og dram, og øl og dram, og øl og dram.

Lagre filen og lukk den.

Nå er vi klare til å sende denne endringen til GitHub!
Kjør følgende kommando i terminalen:

```
git add nu_klinger.txt
```

```
git commit -m "la inn refrenget på nu klinger"
```

```
git push --set-upstream origin nu_klinger
```

Flott, endringene er pushet til branchen `nu_klinger`! La oss merge `nu_klinger` med `master`.
Bytt tilbake til master-branchen ved å kjøre følgende kommando i terminalen:

```
git switch master
```

Merge inn nu_linker-branchen ved å kjøre følgende kommando i terminalen:

```
git merge nu_klinger
```
