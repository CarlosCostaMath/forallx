# forallx — Introdução à lógica formal

Este repositório contém uma tradução e adaptação brasileira de *forall x: An Introduction to Formal Logic*, de P.D. Magnus, baseada na edição mantida pelo [Open Logic Project](https://github.com/OpenLogicProject/forallx).

**Tradutor e adaptador:** Carlos André Duarte Costa.

A tradução está em revisão editorial. Sugestões e correções são bem-vindas por meio das [issues](https://github.com/CarlosCostaMath/forallx/issues) e dos *pull requests*.

## Arquivos principais

- [Fonte principal em LaTeX](forallx.tex)
- [PDF versionado (instantâneo)](forallx.pdf)
- [Execuções do workflow de compilação](https://github.com/CarlosCostaMath/forallx/actions)

O PDF versionado é um instantâneo do repositório e pode não corresponder ao commit mais recente. Para obter o PDF compilado a partir de um commit específico, abra a execução aprovada do workflow e baixe o artefato `forallx-pdf-<commit>`.

## Compilação local

Com uma instalação do TeX Live que inclua XeLaTeX e `latexmk`, execute na raiz do repositório:

```sh
latexmk -xelatex -interaction=nonstopmode -halt-on-error forallx.tex
```

O comando gera `forallx.pdf` e os arquivos auxiliares da compilação. Para limpar esses arquivos, use:

```sh
latexmk -C forallx.tex
```

## Créditos e licença

A obra original é de P.D. Magnus e foi disponibilizada sob a [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/). Esta tradução e adaptação deve manter a atribuição ao autor original e ao tradutor.

A edição brasileira não é uma publicação oficial do Open Logic Project; ela é uma obra derivada distribuída sob os termos da licença aplicável.
