[![LeetCode user maxusun](https://img.shields.io/badge/dynamic/json?style=flat-square&labelColor=black&color=%23ffa116&label=Solved&query=solvedOverTotal&url=https%3A%2F%2Fleetcode-badge.vercel.app%2Fapi%2Fusers%2Fmaxusun&logo=leetcode&logoColor=yellow)](https://leetcode-cn.com/u/maxusun/)


![info](https://github-readme-stats.vercel.app/api?username=maxusun&show_icons=true&count_private=true&hide=prs&theme=default_repocard)

name: WakaTime Readme

on:
  push:
    branches:
      - master
  schedule:
    - cron: '0 19 * * *'

jobs:
  update-readme:
    runs-on: ubuntu-latest
    steps:
      - uses: athul/waka-readme@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
