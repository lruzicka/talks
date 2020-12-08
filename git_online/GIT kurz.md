# GIT kurz

## Nastavení GITu

### Založení účtu na github.com

1. Jděte na `github.com`.

2. Vyplňte malý formulář vpravo nahoře.

3. Založte si účet kliknutím na zelené tlačítko **Sign up for GitHub**.

### Založení nového repozitáře

1. Klikněte na **ikonu profilu** vpravo nahoře.

2. Vyberte položku **Your repositories**.

3. Klikněte na tlačítko **New** vpravo pod ikonou profilu.

4. Zvolte jméno repozitáře.

5. Napište krátký popis repozitáře, ve kterém naznačíte, o co v repu jde.

6. Zvolte **public** nebo **private** pro veřejný či soukromý repozitář.

7. Zaškrtněte volbu **Add a README file**.

8. Zvažte přidání souboru **.gitignore**. Po zaškrtnutí vyberte odpovídající šablonu z nabídky.

9. Zvažte přidání souboru s **licencí**. Vyberte licenci z nabídky.

10. Klikněte na tlačítko **Create repository**.

### Nastavení webových stránek github.io

1. Jděte na stránku repozitáře.

2. Klikněte na tlačítko **Settings** v navigační liště vpravo.

3. Scrollujte dolů až na oddělení **GitHub Pages**.

4. Zvolte si, z jaké větve se bude brát obsah pro webové stránky.

5. Vyberte si adresář `/docs`, ze kterého se bude brát obsah pro stránky.

6. Klikněte na tlačítko **Save**.

7. Znovu běžte na tentýž oddíl, vidíte už adresu, na které se budou stránky hostovat.

8. Vyberte si téma pro stránky.

9. Vytvořil se Vám soubor `index.md`, který bude hlavním zdrojovým textem.

10. Navrhovaný obsah smažte a napište do něj následující řádek:
    
    `## Stránky Jméno Příjmení`

11. Stiskněte **Commit changes** a tím si uložíte obsah souboru.

12. Po chvíli se podívejte na adresu Vašich stránek, zda změnu vidíte.

## Ukázka learngitbranching.js.org

1. `git status`

2. `git log`

3. `git commit`

4. `git checkout -b`

5. `git merge`

6. Vysvětlit, co to je **merge commit**.

7. `git rebase`

8. Vysvětlit, co to je **rebase** a ukázat čistou historii.

9. Ukázat práci s více větvemi a jak správně slučovat.

## Vysvětlit úpravy historie

### git commit --amend

1. Proč použít?

2. Jaké to má následky vůči serveru?

3. Jak to vyřešit? `git push --force`

4. Vysvětlit, proč to dělat pouze na vlastní větvi.

### git rebase --interactive

1. Proč použít a jaké možnosti máme?

2. **pick** použije commit, tak jak je

3. **reword** použije commit, ale lze přepsat commit message

4. **edit** použije commit, ale během procesu zastaví, aby se dal commit ještě upravit

5. **squash**, použije commit a sloučí jej s předcházejícím commitem do jednoho

6. **fixup**, stejně jako squash, ale zahodí jeho commit message

7. **break** přeruší rebase na tomto místě (musí se pokračovat příkazem `git rebase --continue`)

8. **drop** zahodí commit

9. Jaké to má následky vůči serveru?

10. Vysvětlit, proč to dělat jenom na vlastní větvi.

## Odkládání stranou

1. Vysvětlit proč někdy je potřeba odložit práci stranou - je potřeba pullnout, ale už jsou změny na lokále.

2. `git stash`

3. `git stash list`

4. `git stash drop`

5. `git stash clear` (celou *stash*)

## Vytváření patchů

1. Vysvětlit, co je to **patch** a proč jej použít.

2. Patch můžu dělat mezi dvěmi různými větvemi. Tou stávající a tou, kterou uvedu v samotném příkazu. Patch na stejné větvi se mi nepodaří udělat.

3. `git format-patch <větev> -o <adresář>`

4. `git format-patch -1 <commit-sha> -o <adresář>` - udělá patch pouze z jednoho commitu.

5. `git am <soubor-s-patchem>`


