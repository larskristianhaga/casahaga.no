### Siden bruker [Hugo](https://gohugo.io/) som rammeverk for å enkelt lage nye sider, og temaet [PaperMod](https://github.com/adityatelange/hugo-PaperMod/) for styling.

For å kjøre lokalt:

```bash
hugo serve
```

Får du en 404 på forsiden, sørg for at PaperMod temaet er lastet ned ved å kjøre:

```git
git submodule update --init --recursive
```

For deployment push til `main` branch så vil GitHub Actions ta over resten av jobben.

**Oppdatere tema:**

Kjør:

```git
git submodule update --remote --merge
```

Pass på å ikke commit noe under `themes/PaperMod/*` da det tilhører ett annet repo. Istedet kan man heller overstyre
styling og slikt fra temaet.
