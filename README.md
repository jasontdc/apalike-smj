# Italicise_apalike_bst
A modified `apalike.bst` LaTeX bibliography style file for submissions to Strategic Management Journal.

Changes from original apalike style:

- Includes italicised "et al.'s".
- Excludes parentheses around publication date.

Thanks to [@jrjhealey]( https://github.com/jrjhealey ) for his [Italicise_apalike_bst]( https://github.com/jrjhealey/Italicise_apalike_bst ) on which this is based.

### 'Installing'

In order to use this alternative `.bst` file, download the file itself to the *same directory* as the `.tex` document which constructs your bibliography. This must be done so that your TeX application prioritises it over the default files located among the system files.
i.e.:

    ../                         <---- Document top level folder
     |
     |-- document.tex           <---- Document file that calls \bibliographystyle{}
     |
     |-- customapalike.bst      <---- Modified file from this repository
      
In your `.tex` file, you should then have something that resembles the following:

```tex
%% Preamble
\documentclass[]{} % Doc Setup

\begin{document}
...document body...

\bibliographystyle{customapalike}
\bibliography{/path/to/mybibfile.bib}
\end{document}
```

Set the `\bibliographystyle{customapalike}` using the name of the downloaded `.bst` file. If it is in the same directory as the main `.tex` file, you shouldnt need to specify the extension or the full filepath.
