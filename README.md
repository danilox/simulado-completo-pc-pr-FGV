# Simulado PC PR 2026 — Agente — FGV — Versão calibrada pelos PDFs

Versão estática para GitHub Pages.

## O que esta versão altera

- Banco de 100 questões mantido na distribuição do concurso.
- Enunciados ampliados com padrão mais próximo dos cadernos FGV enviados.
- Situações-problema em todas as disciplinas, especialmente TI, Forense, Direitos, Contabilidade e Estatística.
- Alternativas mais contextualizadas e menos óbvias.
- Comentários de professor ampliados com alerta de pegadinha FGV.
- Resposta travada: depois de marcar, o candidato não consegue trocar.
- Mapa de questões por disciplina com quadradinhos clicáveis.
- Salvamento automático no localStorage.
- Som: usa `audio/erro.mp3` se existir; caso contrário, usa som sintético + fala do navegador: “Errou. Fatality.”

## Como rodar localmente

Abra o arquivo `index.html` no navegador.

## Como publicar no GitHub Pages

1. Envie o `index.html` para a raiz do repositório.
2. Acesse Settings > Pages.
3. Selecione Deploy from branch > main > root.
4. Salve e aguarde o link ser publicado.

## Como colocar seu próprio áudio de erro

Crie a pasta `audio` na raiz do repositório e coloque o arquivo:

```text
index.html
audio/erro.mp3
```

O navegador só libera áudio depois de clique do usuário, então use o botão de teste na tela inicial.

## Como atualizar no GitHub

```bash
git rm -r .
# copie o novo index.html para a pasta do projeto
git add index.html README.md
git commit -m "Atualiza simulado PC PR 2026 calibrado pelos PDFs FGV"
git push
```


## Áudios de acerto e erro

Esta versão inclui os arquivos de áudio enviados pelo usuário:

```text
audio/acerto.ogg
audio/erro.ogg
```

Com o botão de som ativado, o simulado toca `acerto.ogg` quando o candidato acerta a questão e `erro.ogg` quando ele erra. O navegador exige uma interação do usuário antes de liberar áudio; por isso há botões de teste na tela inicial.
