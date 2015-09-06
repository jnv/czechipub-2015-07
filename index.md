title: Publikujeme a blogujeme na GitHubu
author:
  name: Jan Vlnas
  twitter: janvlnas
  url: http://jan.vlnas.cz
output: index.html
controls: false
style: style.css

---

# Publikujeme a blogujeme na GitHubu
## Czechipub, 30. 7. 2015

--

### Jak se tvoří web

1. Napiš
2. Zkontroluj
3. Nahraj na server
4. Opakuj

--

### Jenže…

* Ruční nahrávání stránek je otrava
* Změny se těžko berou zpět

--

### Co je to Git?

* Verzovací nástroj
* Ukládá změny v souborech
* Usnadňuje sdílení změn s ostatními

--

### Co je to GitHub

* Služba pro spolupráci s Gitem 
* Aplikace pro práci s Gitem

--

### Co je to GitHub

<div style="text-align:center">
<img src="octocat.png" style="max-height:500px">
</div>
--

### Git není jen pro programátory

* [3D modely](https://github.com/lorennorman/octocat-3d/blob/master/stl/octocat_head.stl) (včetně [zobrazení rozdílů](https://github.com/blog/1633-3d-file-diffs))
* [mapy](https://github.com/colemanm/hurricanes/blob/master/fl_2004_hurricanes.geojson)
* [recepty](https://github.com/sinker/tacofancy)
* [vládní data a dokumenty](https://government.github.com/community/)
* psaní a publikování,
* [a více…](http://readwrite.com/2013/11/08/seven-ways-to-use-github-that-arent-coding)

--

### Termiti

* repozitář (_repository_)
* _commit_
* větev (_branch_)
* _push_ a _pull_
* _fork_

--

### Zkusme si to

1. Nainstalujte si GitHub pro desktop na [desktop.github.com](https://desktop.github.com/)
2. [Zaregistrujte si účet na GitHubu](https://github.com/join) a přihlaste se v aplikaci; nezapomeňte potvrdit svůj e-mail!
3. Vytvořte si nový repozitář, např. `pokus`
4. V něm vytvořte novou větev `gh-pages`
5. V ní vytvořte soubor `index.html` a publikujte repozitář na GitHub!

--

### Výsledek

…výsledek naleznete na adrese `<váš username>.github.io/<název repozitáře>`.

Takže pokud můj username je `uzivatel` a repozitář jsem pojmenoval `pokus`, výsledek najdu na: `uzivatel.github.io/pokus`.

--

### A co takhle vlastní blog?

<div style="text-align:center;padding-top:2em">
![](jekyll.png)
</div>

--

### Statické a dynamické stránky

Jaký je rozdíl třeba mezi Jekyllem a WordPressem?

--

## Statické stránky

<img src="dia-static.png" style="max-width:100%">

Soubor se stránkou (např. `index.html`) je uložený na disku serveru. Server jej rovnou pošle prohlížeči.

--

### Dynamické stránky

<img src="dia-dynamic.png" style="max-width:100%">

<div class="note">
Na serveru je aplikace (např. WordPress), která vygeneruje požadovanou stránku „za běhu“ s pomocí šablony a dat uložených v databázi.
</div>

--

### Generátor statických stránek

<img src="dia-gen.png" style="max-width:100%;max-height:">

<div class="note">
U sebe na počítači mám šablony a data, s pomocí generátoru (např. Jekyll) vygeneruji statické stránky a umístím na server. Server posílá statické stránky a neví o žádnem generátoru.
</div>

--

### GitHub Pages

<img src="dia-ghp.png" style="max-width:100%;max-height:">

<div class="note">
Při „pushnutí“ změn na GitHub se automaticky vygeneruje web pomocí Jekyllu, a GitHub jej začne servírovat stejně jako statické stránky které jsme si vytvořili předtím.
</div>

--

### Co Jekyll umí?

* Opakované prvky na stránce (např. navigace) můžete dát do šablony,
* automaticky generuje přehled článků a kategorie,
* články umožňuje psát v Markdownu

…a více viz [jekyllrb.com](http://jekyllrb.com/).

--

### Markdown?

…je jednoduchý značkovací jazyk který umožňuje formátovat text jednodušeji než HTML. Například:

```markdown
Tento text je **tučně** a tento _kurzivou_.
Toto je [odkaz na web Czechitas](http://www.czechitas.cz/).
```

vytvoří:

> Tento text je **tučně** a tento _kurzivou_.
> Toto je [odkaz na web Czechitas](http://www.czechitas.cz/).

<small>(Většina této prezentace je psaná v Markdownu)</small>
--

### Zkusme si to

1. „Forkněte“ si [ukázkový blog](https://github.com/jnv/czechipub-blog)
2. Upravte text v souboru `o-mne.md` nebo nějaký soubor v adresáři `_posts`
   <br><small>Soubory můžete upravit i přímo na GitHubu, když kliknete na příslušný soubor a vpravo nahoře na ikonu tužky.</small>
3. Podívejte se na výsledek na `<váš username>.github.io/czechipub-blog`!

--

Pokud nemůžete váš blog najít zkontrolujte si nastavení repozitáře (položka `Settings` s ozubeným kolem v pravém menu); v panelu GitHub Pages byste měli vidět adresu vašeho blogu.

![](gh-settings.png)

--

### Zdroje a odkazy

* [Try Git](https://try.github.io/) vás provede podrobně používáním Gitu na příkazové řádce.
* [GitBook](https://www.gitbook.com/) zjednodušuje psaní a publikaci knížek s pomocí Gitu.
* [Markdown Tutorial](http://markdowntutorial.com/) vás provede psaním v Markdownu.
* [Jekyll](http://jekyllrb.com/)
* [GitHub Pages](https://pages.github.com/)
