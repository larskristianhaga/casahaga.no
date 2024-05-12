### Siden bruker [Hugo](https://gohugo.io/) som rammeverk for å enkelt lage nye sider, og temaet [PaperMod](https://github.com/adityatelange/hugo-PaperMod/) for styling.

For å kjøre lokalt - ```hugo serve```

Får du en 404 på forsiden, sørg for at PaperMod temaet er lastet ned ved å kjøre `git submodule update --init --recursive`.

For deployment push til `main` branch så vil GitHub Actions ta over resten av jobben.

Google Analytics er også installert i headeren på siden for å tracke antall brukere og de mest populære sidene, dashboard kan sees
her - [analytics.google.com](https://analytics.google.com/analytics/web/#/p406743236/reports/intelligenthome).

**Oppdatere tema:**

Kjør `git submodule update --remote --merge` for å oppdatere PaperMod temaet.

Pass på å ikke commit noe under `themes/PaperMod/*` da det tilhører ett annet repo. Istedet kan man heller overstyre styling og slikt fra temaet.
