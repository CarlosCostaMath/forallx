# forallx — Introdução à lógica formal

Este repositório contém uma tradução e adaptação brasileira de *forall x: An Introduction to Formal Logic*, de P.D. Magnus, baseada na edição mantida pelo [Open Logic Project](https://github.com/OpenLogicProject/forallx).

**Tradutor e adaptador:** Carlos André Duarte Costa.

A tradução está em revisão editorial. Sugestões e correções são bem-vindas por meio das [issues](https://github.com/CarlosCostaMath/forallx/issues) e dos *pull requests*.

## Arquivos principais

- [Fonte principal em LaTeX](forallx.tex)
- [PDF da última versão publicada](https://github.com/CarlosCostaMath/forallx/releases/latest/download/forallx.pdf)
- [Releases e versões anteriores](https://github.com/CarlosCostaMath/forallx/releases)
- [Execuções dos workflows](https://github.com/CarlosCostaMath/forallx/actions)

O PDF oficial é publicado automaticamente em uma Release quando uma tag de versão, como `v0.1.0`, é criada. O link acima sempre aponta para a Release marcada pelo GitHub como mais recente. O arquivo `forallx.pdf` é produzido durante a compilação e não é mantido como arquivo versionado na raiz do repositório.

## Compilação local

Com uma instalação do TeX Live que inclua XeLaTeX e `latexmk`, execute na raiz do repositório:

```sh
latexmk -xelatex -interaction=nonstopmode -halt-on-error forallx.tex
```

O comando gera `forallx.pdf` e os arquivos auxiliares da compilação. Para limpar esses arquivos, use:

```sh
latexmk -C forallx.tex
```

## Publicação de uma versão

Depois de revisar e mesclar as alterações na `master`, crie uma tag começando por `v`:

```sh
git tag v0.1.0
git push origin v0.1.0
```

O workflow `Publish PDF Release` será executado automaticamente. Se a compilação passar, o GitHub criará a Release, anexará o arquivo `forallx.pdf` e gerará as notas da versão.

## Créditos e licença

A obra original é de P.D. Magnus e foi disponibilizada sob a [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/). Esta tradução e adaptação deve manter a atribuição ao autor original e ao tradutor.

A edição brasileira não é uma publicação oficial do Open Logic Project; ela é uma obra derivada distribuída sob os termos da licença aplicável.
