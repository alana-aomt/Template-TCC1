# Template TCC I — UFMA / Eng. da Computação

Template LaTeX (abnTeX2) para o **Trabalho de Conclusão de Curso I** do curso de Engenharia da Computação da UFMA.

## Estrutura do documento

| Arquivo | Conteúdo |
|---------|----------|
| `main.tex` | Capa, folha de rosto, resumo, sumário e configurações |
| `1-introducao.tex` | Introdução, justificativa e objetivos |
| `2-fundametacao.tex` | Fundamentação teórica |
| `2-trabalhos-relacionados.tex` | Trabalhos relacionados e posicionamento |
| `3-metodologia.tex` | Metodologia da pesquisa |
| `4-resultados.tex` | Resultados **esperados** (TCC I) |
| `5-cronograma.tex` | Cronograma para o TCC II |
| `6-conclusao.tex` | Considerações finais |
| `referencias.bib` | Referências bibliográficas (BibTeX) |

## Como usar

1. **Clone ou copie** este repositório para a pasta do seu TCC.
2. **Edite `main.tex`**: preencha título, autor(a), orientador(a) e resumo.
3. **Edite cada capítulo** (`.tex`): substitua os textos `\placeholder{...}` pelo seu conteúdo.
4. **Leia os blocos de orientação** (`Orientação:` em itálico): eles explicam o que escrever em cada seção.
5. **Adicione referências** em `referencias.bib` e cite com `\cite{chave}`.
6. **Logo da UFMA**: coloque `logoufma.png` em `figuras/logoufma.png`.
7. **Antes de entregar**: remova ou comente os comandos `\orientacao{...}` e `\placeholder{...}` do `main.tex` e dos capítulos.

## Compilação

Requisitos: TeX Live (ou MacTeX) com abnTeX2, Biber/BibTeX e fonte Arial instalada.

```bash
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

> **Nota:** use `xelatex` (não `pdflatex`) porque o template define a fonte Arial via `fontspec`.

Ou use um editor como TeXstudio, Overleaf ou VS Code com LaTeX Workshop.

## Elementos pré-textuais (SIGAA)

- **Ficha catalográfica**: após gerar no SIGAA, descomente `\includepdf{ficha_cat.pdf}` em `main.tex`.
- **Assinaturas da banca** (TCC II): descomente `\includepdf{assinaturas.pdf}` quando disponível.

## Dicas

- No TCC I **não há resultados empíricos** — use o capítulo de Resultados Esperados.
- Mantenha coerência entre problema de pesquisa, objetivos, metodologia e resultados esperados.
- Converse com seu orientador sobre seções opcionais (resumo em inglês, listas de figuras/tabelas, apêndices).
- Para o TCC II, renomeie/adapte `4-resultados.tex` para apresentar dados reais e adicione o capítulo de Discussão.

## Licença

Baseado no modelo abnTeX2 (LPPL). Adaptado como template acadêmico UFMA.
