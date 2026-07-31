[README.md](https://github.com/user-attachments/files/30566724/README.md)
# processos-recebiemnto# Suporte Recebimento — Central de Documentos

Site estático com os manuais, formulários e planilhas do setor de Recebimento.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (pode ser **privado** se os documentos forem internos).
2. Envie todo o conteúdo desta pasta para o repositório (`index.html`, a pasta `files/`, e este `README.md`).
3. No repositório, vá em **Settings → Pages**.
4. Em **Source**, selecione a branch `main` e a pasta `/root`, depois clique em **Save**.
5. Em alguns minutos o GitHub gera um link do tipo `https://seu-usuario.github.io/nome-do-repositorio/`.

⚠️ **Atenção:** se o repositório for privado, o GitHub Pages só funciona nesse modo em planos pagos (GitHub Pro/Team/Enterprise). No plano gratuito, Pages exige repositório público. Se os documentos forem sensíveis, considere hospedar em vez disso no SharePoint, Google Sites, ou um plano pago do GitHub.

## Como adicionar ou trocar um arquivo

1. Coloque o novo arquivo dentro da subpasta correta em `files/` (ex: `files/manuais/`).
2. Abra o `index.html` e copie um bloco `<a class="card">...</a>` já existente na mesma seção.
3. Ajuste:
   - `href="files/.../nome-do-arquivo.ext"` → caminho do novo arquivo
   - `data-search="..."` → palavras-chave para a busca encontrar
   - `<div class="title">...</div>` → nome que aparece no site
   - `<div class="meta">...</div>` → tamanho do arquivo (opcional)
   - o `tag-chip` (`chip-pdf`, `chip-doc`, `chip-sheet`, `chip-img`) → cor do selo conforme o tipo

## Estrutura de pastas

```
index.html
files/
  notas-fiscais-entradas/
  inventario/
  manuais/
  controle-ativos/
  holambra/
  arquivos-e-planilhas/
  organograma-compras-e-suplay/
```

Todos os nomes de arquivo foram padronizados (sem acentos, espaços ou colchetes) para evitar problemas de link quebrado no GitHub.
