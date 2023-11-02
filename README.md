Olá, Meu nome é Caio Bassalo Resque 👋

- 🔭 Atualmente estou trabalhando com tecnologias de front-end, procurando sempre aprimorar cada vez mais o meu conhecimento.
- 🌱 Hoje estou estudando React.
- 💻 No futuro pretendo aprender tecnologias de back-end, para que assim, eu possa me tornar um desenvolvedor Fullstack.
- 📫 Contate-me no email: caio.resque@gmail.com


<a href="https://github.com/caioresque"></a>
<img width="42%" src="https://github-readme-stats.vercel.app/api?username=caioresque&show_icons=true&theme=gruvbox"/>
<img width="57%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=caioresque&layout-compact&langs_count-16&theme=gruvbox"/>

<h2 align="center">🛠️&ensp; <i>Ｔｅｃｎｏｌｏｇｉａ s</i> &ensp;🛠️</h2>
<div style="text-align: center;">
<p align="center">
<img align="center" alt="Caio-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
<img align="center" alt="Caio-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
<img align="center" alt="Caio-Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
<img align="center" alt="Caio-React" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg">
<img align="center" alt="Caio-Git" height="30" width="40" src="https://skillicons.dev/icons?i=github" width="32" alt=" icon"/>
</p>
</div>



<h2 align="center"><i>Redes Sociais</i>💬</h2>
<div style="text-align: center;">
<p align="center">
<a href="https://www.linkedin.com/in/caioresque" alt="" target="_blank">
<img align="center" height="30" width="40" src="https://skillicons.dev/icons?i=linkedin"/>
</a>

<a href="https://m.facebook.com/caio.resque" alt="" target="_blank">
<img align="center" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/facebook/facebook-original.svg">
</a>

<a href="https://twitter.com/caioresque" alt="" target="_blank">
<img <img align="center" height="30" width="40" src="https://skillicons.dev/icons?i=twitter"/>
</a>

<a href="https://instagram.com/caio.resque" alt="" target="_blank">
<img align="center" height="30" width="40" src="https://skillicons.dev/icons?i=instagram"/>
</a>
</div>
</p>

name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: caioresque
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  



