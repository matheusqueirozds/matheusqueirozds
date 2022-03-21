<div align="center">
 
 # Desenvolvedor Front-end e UI Designer
 
</div>

## 🤓 SOBRE MIM
🔍 Atualmente estudo **`HTML`**, **`CSS`**, **`JavaScript`** e **`UI Design`**

⚡ Sou cristão, nerd declarado e amante de ficção científica. Meus filmes favoritos são a *Triologia De Volta Para o Futuro* e a *Triologia do Homem-aranha (Sam Raimi)*

📈 Metas para 2022 
  * Criar no mínimo 6 projetos: 
  
    * [x]  🤖 Site Responsivo Android - [*Acesse aqui*](https://github.com/matheusqueirozds/site-responsivo-android)
    * [x]  🎵 Desafio Cordel - [*Acesse aqui*](https://github.com/matheusqueirozds/desafio-cordel)
    * [x]  ☀ Bio - [*Acesse aqui*](https://github.com/matheusqueirozds/bio) 
    * [ ]  📜 Portfólio (em construção) - [*Acesse aqui*](https://github.com/matheusqueirozds/portfolio)
    * [ ]  🧹 Vassourax - [*Acesse aqui*](#)
    * [ ]  ⛪ Site para Igreja - [*Acesse aqui*](#)
  
  * Aprender algum framework

<div align="center">
 
[![Portfólio](https://img.shields.io/badge/Portfólio-%23000000.svg?style=for-the-badge&logoColor=#FF7139)](https://matheusqueirozds.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/matheusqueirozds)
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?style=for-the-badge&logo=Instagram&logoColor=white)](https://www.instagram.com/matheusqueirozds.dev)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:matheusqueirozds@gmail.com)

 </div>

---
## 🛠 TECNOLOGIAS E FERRAMENTAS

<div align="center">
 
### 🔠 Programação
![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
 
</div> 

#

<div align="center">
 
### 🖌 Design
![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white)
![Adobe Illustrator](https://img.shields.io/badge/adobe%20illustrator-%23FF9A00.svg?style=for-the-badge&logo=adobe%20illustrator&logoColor=white)
![Adobe Photoshop](https://img.shields.io/badge/adobe%20photoshop-%2331A8FF.svg?style=for-the-badge&logo=adobe%20photoshop&logoColor=white)
![Adobe Premiere Pro](https://img.shields.io/badge/Adobe%20Premiere%20Pro-9999FF.svg?style=for-the-badge&logo=Adobe%20Premiere%20Pro&logoColor=white)
 
</div> 

---
## 📚 CURSOS 

<div align="center">
 
### Em andamento
  
Curso | Instituição | Carga horária | Conclusão
-|:-:|:-:|-
  Web Full Stack | Labenu | 12 meses | 04/2023
 
#

### Concluídos
  Curso | Instituição | Carga horária | Certificado
  -|:-:|:--:|-
  UI Design para iniciantes | Origamid | 34 horas | [Acesse aqui](https://drive.google.com/file/d/1_IqY6FIqnL0g_2QMijRrFPlhlfQ6f5sK/view?usp=sharing)
  Web Design Completo | Origamid | 44 horas | [Acesse aqui](https://drive.google.com/file/d/1Q6OlmB-mWhcixGuN5z1kjGwnzLgoKBeY/view?usp=sharing)
  Computação Gráfica | Saga | 36 meses | [Acesse aqui](https://drive.google.com/file/d/1fcDaHT4RIssUp5yRAr_3mIbEna9qKPTD/view?usp=sharing)

</div>

---

## 📊 ESTATÍSTICAS
  <a href="https://github.com/matheusqueirozds">
  <img height="160rem" src="https://github-readme-stats.vercel.app/api/top-langs/?username=matheusqueirozds&layout=compact&langs_count=7&theme=dark"/>

  <a href="https://github.com/matheusqueirozds">
  <img height="160rem" src="https://github-readme-stats.vercel.app/api?username=matheusqueirozds&show_icons=true&theme=dark&include_all_commits=true&count_private=true"/>
   
   
   <!-- <span style="height ">
![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=matheusqueirozds&show_icons=true&theme=tokyonight)
</span> -->

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=matheusqueirozds&show_icons=true&theme=tokyonight)
[![matheusqueirozds](https://github-readme-stats.vercel.app/api/top-langs/?username=matheusqueirozds&hide=html&layout=compact=true&theme=tokyonight)](https://github.com/matheusqueirozds/)

# GitHub Action for generating a contribution graph with a snake eating your contributions.

name: Generate Snake

# Controls when the action will run. This action runs every 6 hours.

on:
  schedule:
      # every 6 hours
    - cron: "0 */6 * * *"

# This command allows us to run the Action automatically from the Actions tab.
  workflow_dispatch:

# The sequence of runs in this workflow:
jobs:
  # This workflow contains a single job called "build"
  build:
    # The type of runner that the job will run on
    runs-on: ubuntu-latest

    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:

    # Checks repo under $GITHUB_WORKSHOP, so your job can access it
      - uses: actions/checkout@v2

    # Generates the snake  
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: matheusqueirozds
          # these next 2 lines generate the files on a branch called "output". This keeps the main branch from cluttering up.
          gif_out_path: dist/github-contribution-grid-snake.gif
          svg_out_path: dist/github-contribution-grid-snake.svg

     # show the status of the build. Makes it easier for debugging (if there's any issues).
      - run: git status

      # Push the changes
      - name: Push changes
        uses: ad-m/github-push-action@master
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          branch: master
          force: true

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          # the output branch we mentioned above
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} 


