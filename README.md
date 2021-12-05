# README

## To read

## HTML, PDF and DOCX

open the file

## Markdown

### Best way

1. Open GreenIT_LesPetitGestes.md in Visual Studio Code
2. Install package `Markdown All In One`
3. Press `ctrl`+`shift`+`p` and run `Markdown: open preview`

### Other way

- open GreenIT_LesPetitGestes.md in markdown editor on your device.
- open GreenIT_LesPetitGestes.md in [stackedit](https://stackedit.io/app#).

## How can I contribute?

1. Fork and clone the repository:
   1. On GitHub interface:
      1. Click **Fork** ![Fork](https://docs.github.com/assets/images/help/repository/fork_button.jpg)
      2. GitHub will take you to your copy (your fork) of the greenItSpeakUp repository.
      3. On GitHub, navigate to your fork of the greenItSpeakUp repository.
      4. Above the list of files, click Code ![Code](https://docs.github.com/assets/images/help/repository/code-button.png)
      5. To clone the repository using HTTPS, under "Clone with HTTPS", click on paste icon. To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click Use SSH, then click on paste icon. To clone a repository using GitHub CLI, click Use GitHub CLI, then click on paste icon. ![Clone](https://docs.github.com/assets/images/help/repository/https-url-clone.png)
      6. Open Git Bash.
      7. Change the current working directory to the location where you want the cloned directory.
      8. run `git clone https://github.com/YOUR-USERNAME/greenItSpeakUp`
   2. In command line:
      1. *Prerequisit* install [GitHub CLI](https://cli.github.com/)
      2. Open Git Bash.
      7. Change the current working directory to the location where you want the cloned directory.
      3. run `gh repo fork https://github.com/artvantichelen/greenItSpeakUp.git --clone`
2. Install dependances:
   1. Install [Pandoc](https://pandoc.org/installing.html)
   2. Install [MiKTeX](https://miktex.org/download)
3. Changes:
   1. Modify only the file **GreenIT_LesPetitsGestes.md**
   2. Export to pdf:
      1. run in terminal `pandoc GreenIT_LesPetitsGestes.md -o GreenIT_LesPetitsGestes.pdf`
   3. Export to html:
      1. run in terminal `pandoc --toc --standalone --mathjax --metadata title="Green IT : Les petits gestes" -f markdown -t html GreenIT_LesPetitsGestes.md -o GreenIT_LesPetitsGestes.html`
   4. Export to docx:
      1. run in terminal `pandoc -f markdown -t latex -o GreenIT_LesPetitsGestes.tex GreenIT_LesPetitsGestes.md && pandoc -f latex -t docx --data-dir=docs/rendering/ -o GreenIT_LesPetitsGestes.docx GreenIT_LesPetitsGestes.tex`
4. Push on your repo:
   1. run `git add .`
   2. run `git commit -m "a short description of the change"`
   3. run `git push`
5. Making a pull request:
   1. Navigate to your fork `https://www.github.com/<your_username>/greenItSpeakUp`. You'll see a banner indicating that your branch is one commit ahead of `octocat:main`
   2. Click **Contribute** and then **Open a pull request**