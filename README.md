### Hi there, I'm a Student My Name is Emirhan 
<img align="right" alt="GIF" src="https://raw.githubusercontent.com/abhisheknaiidu/abhisheknaiidu/master/code.gif" width="500" height="320" />
<!--
**emirhandalgiran/emirhandalgiran** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile. -->

This is the place where I opensource stuff and break things

- 🔭 I’m currently working on something really cool
- 🌱 I’m currently learning everything
- 👯 I’m looking to collaborate on more open source projects.
- 💬 Ask me anything [here](https://www.instagram.com/emirhan.dalgiran/) related to <b>Android application Development, Windows Forms, C#, Javascript, Unity.</b>

### Connect with me:

[<img align="left" alt="lefearr | GitHub" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/github.svg" />][github]
[<img align="left" alt="lefearr | Instagram" width="22px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/instagram.svg" />][instagram]


<br />

### Languages and Tools:
<img align="left" alt="JavaScript" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/javascript/javascript.png" />
<img align="left" alt="Android" width="26px" src="https://img.favpng.com/13/23/14/c-foreach-loop-while-loop-conditional-png-favpng-LKs4HkfcdgR64TbSHhtHVD7DK.jpg" />
<img align="left" alt="Visual Studio" width="26px" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/59/Visual_Studio_Icon_2019.svg/1200px-Visual_Studio_Icon_2019.svg.png" />
<img align="left" alt="Visual Studio Code" width="26px" src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Visual_Studio_Code_1.35_icon.svg/2048px-Visual_Studio_Code_1.35_icon.svg.png" />
<img align="left" alt="PostgreSQL" width="26px" src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/Postgresql_elephant.svg/745px-Postgresql_elephant.svg.png" />
<img align="left" alt="MSSQL" width="26px" src="https://1.bp.blogspot.com/-PKyyK4SxGfg/YP6gzi4l5pI/AAAAAAAAAWc/gvbZQmUkHfgFuMAkN5XJ3SgfEYbNcNVGwCLcBGAsYHQ/s1280/microsoft-sql-server-logo.png" />
<img align="left" alt="Unity" width="26px" src="https://brandslogos.com/wp-content/uploads/images/large/unity-logo.png" />
<img align="left" alt="GitHub" width="26px" src="https://raw.githubusercontent.com/github/explore/78df643247d429f6cc873026c0622819ad797942/topics/github/github.png" />
<br />
<br />

### 📊 GitHub Stats:
![emirhandalgiran's github stats](https://github-readme-stats.vercel.app/api?username=emirhandalgiran&show_icons=true&theme=radical&count_private=true&include_all_commits=true&hide=contribs,issues,stars)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=emirhandalgiran&layout=compact)


name: Generate Snake



  
  
  Controls when the action will run. This action runs every 6 hours.


on:

  schedule:

      # every 6 hours

    - cron: "0 */6 * * *"



  
  
  This command allows us to run the Action automatically from the Actions tab.


workflow_dispatch:



  
  
  The sequence of runs in this workflow:


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
      github_user_name: emirhandalgiran
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


[instagram]: https://www.instagram.com/emirhan.dalgiran/
[github]: https://github.com/emirhandalgiran
