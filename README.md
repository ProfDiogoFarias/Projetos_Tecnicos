# Biblioteca de Projetos Técnicos

Portal estático em português para organizar e divulgar projetos técnicos e TCCs autorizados. Funciona no GitHub Pages, sem backend, bibliotecas externas ou serviços pagos.

## Estrutura
- `index.html`: página inicial.
- `projetos.json`: catálogo.
- `css/estilo.css`: aparência responsiva.
- `js/biblioteca.js`: busca, filtros e renderização.
- `projetos/modelo-tcc/index.html`: modelo de página individual.
- `GUIA-DE-INSTALACAO.md`: instruções para iniciantes.

## Publicar
1. Crie um repositório público chamado `SEU-USUARIO.github.io`, trocando pelo seu nome de usuário.
2. Envie todos os arquivos e pastas deste pacote para a raiz do repositório.
3. Vá a **Settings → Pages**.
4. Em **Build and deployment**, selecione a publicação por branch, `main` e `/(root)`, depois salve.
5. Aguarde e abra `https://SEU-USUARIO.github.io`.

## Cadastrar projetos
Edite `projetos.json` e acrescente um objeto dentro da lista `projetos`. Use as situações `Em desenvolvimento`, `Em avaliação` ou `Concluído`. Preserve a sintaxe JSON: aspas duplas, vírgulas entre itens e sem vírgula após o último item.

Para uma página própria, copie o modelo para uma pasta como `projetos/tcc-2026-001/index.html` e atualize o campo `pagina` do projeto para `projetos/tcc-2026-001/`.

## Privacidade
Não publique dados pessoais, senhas, tokens, credenciais, documentos internos ou materiais sem autorização. Conteúdo público pode ser copiado por terceiros. O portal não tem login; apenas usuários com permissão de escrita no repositório podem editar os arquivos.
