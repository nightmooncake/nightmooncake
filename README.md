name: Generate Snake

on:
  # Berjalan otomatis setiap 24 jam
  schedule:
    - cron: "0 */24 * * *"
  
  # Memungkinkan kita menjalankan workflow ini secara manual dari tab Actions
  workflow_dispatch:
    
  # Berjalan otomatis setiap kali ada push di branch main/master
  push:
    branches:
    - main
    - master

jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    timeout-minutes: 5
    
    steps:
      # Generates a snake game from a github user contributions graph, output a svg animation
      - name: generate github-contribution-grid-snake.svg
        uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg?palette=github-dark&color_snake=#FF003C&color_dots=#161b22,#45000a,#780012,#b3001b,#FF003C
            dist/ocean.svg?color_snake=#FF003C&color_dots=#161b22,#45000a,#780012,#b3001b,#FF003C

      # Push file svg yang dihasilkan ke branch output agar bisa diakses oleh README
      - name: push github-contribution-grid-snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
