# thesis-template

Minimal but nicely styled thesis template.

The PDF is compiled on commits and is available at [https://github.com/mdmould/thesis-template/blob/build/main.pdf](https://github.com/mdmould/thesis-template/blob/build/main.pdf). This is the file `./main.pdf` in the `build` branch. Change the GitHub username to yours in the URL.

Make sure GitHub actions have write permissions. To do this, go to `Settings` / `Actions` / `General` / `Workflow permissions` and check the box `Read and write permissions`.

You should edit `frontmatter/info.tex` and the other frontmatter pages in `frontmatter/`, which you can choose to make appear or not in `main.tex`.

Chapter and appendix templates are located in `chapters/`. Add `.tex` files for each chapter and appendix and add them to `chapters/`, making sure to `\include{chapters/filename}` in `main.tex`.

Add your figures in `figures/`, with a folder for each chapter if you like.

Add all your references to `main.bib`.

Files in `style/` should not be edited unless you want to edit the thesis style more deeply.

There are two colour macros pre-defined that you can use to highlight text while editing: `\todo{...}` (blue) and `\red{...}` (red).

Compile the PDF locally with `compile.sh` and remove the excess build files with `clean.sh`, which will keep the final `main.pdf`.
