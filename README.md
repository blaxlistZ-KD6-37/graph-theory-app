# Locating Task
1. **Open** `main.tex`
2. **Check** the document for the **roles**.
    - Ex `main.tex` : 
    ```{.tex}
        % Woodrow
        \import{./2_Introduction}{1_Rationale_Fajardo.tex}
    ```
3. **Locate** and open that file. You will see something that looks like this:
    - Ex `2_Traversability_Visitacion.tex` :
    ```{.tex}
        \providecommand{\graphTheoryPreambleLoaded}{}
        \ifx\graphTheoryPreambleLoaded
        \documentclass{article}
        \usepackage{./1_Preamble/graph_theory_preamble}

        \begin{document}
            \fi
            
            \subsection*{Traversability}
            \addcontentsline{toc}{subsection}{Traversability}
            
            \subsubsection*{Eulerian}
            \addcontentsline{toc}{subsubsection}{Eulerian}
            
            \subsubsection*{Hamiltonian}
            \addcontentsline{toc}{subsubsection}{Hamiltonian}
            
            \ifx\graphTheoryPreambleLoaded
        \end{document}
        \fi
    ```

# Handling Errors due to SVG
1. Install **InkScape** through their [website](https://inkscape.org/release/inkscape-1.4.2/windows/64-bit/msi/?redirected=1).
2. Enable `-shell-escape` through your IDE.
    - If IDE is `TexStudio`:
        1. Navigate to **Options**.
        2. Click on **Configure TeXStudio**.
        3. Click on **Commands**
        4. If compiler uses **PdfLaTex**, then change the command to be 
        `pdflatex.exe -synctex=1 -interaction=nonstopmode -shell-escape %.tex`

# Other Notes
- You can either ***add***, ***delete***, and/or ***modify*** your given task to your own liking.

- **Images** or any figure that were not created within a \(\LaTeX\) package(s) must be stored at `0img` folder!

- **Download** by pressing the **Code** button and clicking **Download as Zip**.

- I can only help you with **TeXStudio** problems since I do not use other IDEs.