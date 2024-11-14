<h1 align="center">Hi 👋, I'm Rashid</h1>
<h3 align="center">Flutter Engineer</h3>


  
### ⚙️ Tech stack  
  
+ [![Dart](https://img.shields.io/badge/-Dart-05122A?style=flat&logo=dart&logoColor=blue)](https://dart.dev/)  
+ [![Flutter](https://img.shields.io/badge/-Flutter-05122A?style=flat&logo=flutter&logoColor=blue)](http://flutter.dev/)  
+ [![Test](https://img.shields.io/badge/-Test-05122A?style=flat&logo=dart)](https://dart.dev/guides/testing)    
+ [![Go](https://img.shields.io/badge/-Go-05122A?style=flat&logo=go)](https://go.dev/)  
+ [![Docker](https://img.shields.io/badge/-Docker-05122A?style=flat&logo=docker)](https://www.docker.com/)  



```yml
name: waka Readme

on:
  # for manual workflow trigger
  workflow_dispatch:
  schedule:
    # runs at 12 AM UTC (5:30 AM IST)
    - cron: "0 0 * * *"

jobs:
  update-readme:
    name: WakaReadme DevMetrics
    runs-on: ubuntu-latest
    steps:
        # this action name
      - uses: athul/waka-readme@master # do NOT replace with anything else
        with:
          GH_TOKEN: ${{ secrets.GH_TOKEN }} # optional if on profile readme
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }} # required
          ### meta
          API_BASE_URL: https://wakatime.com/api # optional
          REPOSITORY:https://github.com/Durotann # optional
          ### content
          SHOW_TITLE: true # optional
          SECTION_NAME: waka # optional
          BLOCKS: -> # optional
          CODE_LANG: Flutter # optional
          TIME_RANGE: all_time # optional
          LANG_COUNT: 10 # optional
          SHOW_TIME: true # optional
          SHOW_TOTAL: true # optional
          SHOW_MASKED_TIME: false # optional
          STOP_AT_OTHER: true # optional
          IGNORED_LANGUAGES: YAML JSON TOML # optional
          
```