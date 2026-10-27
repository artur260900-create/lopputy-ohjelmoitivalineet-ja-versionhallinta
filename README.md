# Lopputyö: Git, VS Code ja GitHub

Kurssin lopputyö, terminaaliversio. Kaikki Git-toiminnot tehdään komentorivillä (Git Bash) ja yhteys GitHubiin on SSH.

## Projektin idea

Pieni kauppalista-sivu (HTML + JavaScript), johon voi lisätä ja poistaa ostoksia.
Projekti on tarkoituksella yksinkertainen, koska työssä harjoitellaan versionhallintaa:
haaroja, mergeä, konfliktien ratkaisua ja Gitin jatkotoimintoja.

## Käytetyt komennot

### SSH-avaimen luonti ja testaus

```bash
ssh-keygen -t ed25519 -C "artur260900@icloud.com"
ssh -T git@github.com
```

Julkinen avain (`~/.ssh/id_ed25519.pub`) lisättiin GitHubiin kohdassa Settings → SSH and GPG keys.

### Repositorion kloonaus SSH:lla

```bash
git clone git@github.com:artur260900-create/lopputy-ohjelmoitivalineet-ja-versionhallinta.git
```

### Ensimmäinen commit

```bash
git add README.md
git commit -m "Lisää README ja projektin kuvaus"
git push origin main
```

## Ongelmat ja ratkaisut

- **Repository not found kloonatessa:** kokeilin ensin väärää repositorion nimeä. GitHub muuttaa nimen
  ääkköset ja välilyönnit, joten oikea nimi piti tarkistaa GitHubista.
- **README tallentui väärään kansioon:** VS Codessa oli auki vanha harjoituskansio. Ratkaisu oli avata
  oikea kansio (File → Open Folder) ennen tiedoston luomista.

## Mitä opin

(Täydennetään työn edetessä.)
