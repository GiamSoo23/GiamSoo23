<h1 align="left">Hi, I'm Gregory Ramírez Fuentes 👋</h1>

**CS student @ USF** — building HCI/AR research tools, full-stack side projects, and hackathon community. Looking to break into software engineering internships (CPT-eligible).

### Currently
- 🔬 Research Assistant @ USF's **EnCoDe Lab**, working on the *Pizza Project* — AR-based educational tools for child-computer interaction
- 🏆 VP of Technology, **SHPE Tech Team** — organizing Hack-A-Bull & HackJam
- 📚 Grinding NeetCode 150 + prepping for Fall 2026 hackathon season (Hackabull, HackUSF, SharkByte, ShellHacks, SwampHacks, BloomHacks)
- 💼 Open to SWE internships and full-stack / founding-engineer roles at early-stage startups

### Tech Stack

**Languages**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat&logo=c&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat&logo=arduino&logoColor=white)

**Tools & Platforms**

![WordPress](https://img.shields.io/badge/WordPress-21759B?style=flat&logo=wordpress&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat&logo=figma&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

### Contribution Skyline

on:
  schedule:
    - cron: "0 18 * * *"   # 03:00 JST / matches upstream default schedule
  workflow_dispatch:        # lets you trigger it manually from the Actions tab

permissions:
  contents: write

jobs:
  build:
    runs-on: ubuntu-latest
    name: generate-github-profile-3d-contrib
    steps:
      - uses: actions/checkout@v5

      - name: Generate 3D contribution graph
        uses: yoshi389111/github-profile-3d-contrib@latest
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          USERNAME: giamsoo23

      - name: Commit & Push
        run: |
          git config user.name github-actions
          git config user.email github-actions@github.com
          git add -A .
          if git commit -m "generated"; then
            git push
          fi

### Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/gregoryramirezf)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:ramiro2112gr@gmail.com)
