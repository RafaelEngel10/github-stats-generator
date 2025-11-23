Uses only public API for common data (followers, repos, stars, forks, languages).

If GITHUB_TOKEN already defined (ex: secrets.GITHUB_TOKEN from Actions), it is used to increase rate limits.

To include privated statistics (ex.: count_private=true from github-readme-stats), need Personal Access Token with repo scope and add it as a secrets.PERSONAL_GH_TOKEN, also need to adjust workflow to export GITHUB_TOKEN: ${{ secrets.PERSONAL_GH_TOKEN }}.