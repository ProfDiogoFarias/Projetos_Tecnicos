# Guia de instalação — Biblioteca de Projetos Técnicos

## 1. Criar repositório
1. Entre em https://github.com/ e crie sua conta.
2. Clique em `+` → `New repository`.
3. Nome: `SEU-USUARIO.github.io` (substitua pelo seu usuário exato).
4. Marque `Public` e `Add a README file`; clique em `Create repository`.

## 2. Enviar os arquivos
1. Abra o repositório e clique em `Add file` → `Upload files`.
2. Abra a pasta extraída do ZIP no computador.
3. Envie os arquivos e pastas que estão dentro dela, mantendo a estrutura. `index.html` e `projetos.json` devem ficar na raiz.
4. Escreva uma mensagem como `Adicionar primeira versão do portal` e clique em `Commit changes`.

## 3. Ativar GitHub Pages
1. Abra `Settings` → `Pages`.
2. Em `Build and deployment`, selecione `Deploy from a branch`, se disponível.
3. Escolha branch `main` e pasta `/(root)`.
4. Clique em `Save` e aguarde alguns minutos.
5. Abra `https://SEU-USUARIO.github.io`.

## 4. Cadastrar um TCC
1. Abra `projetos.json` no GitHub e clique no lápis para editar.
2. Copie um objeto de projeto existente, incluindo as chaves `{ }`, e cole como novo item dentro de `projetos`.
3. Dê um ID único, título, área, situação, resumo, tecnologias e palavras-chave.
4. Clique em `Commit changes`.

Exemplo de objeto:
```json
{
  "id": "TCC-2026-001",
  "slug": "monitoramento-energia",
  "titulo": "Monitoramento de consumo elétrico",
  "area": "Eficiência energética",
  "situacao": "Em desenvolvimento",
  "resumo": "Descrição curta do objetivo técnico.",
  "tecnologias": ["Sensores", "Energia elétrica", "Dashboard"],
  "palavrasChave": ["medição", "consumo", "economia"],
  "simbolo": "ϟ",
  "cor": 3,
  "exemploFicticio": false,
  "pagina": "projetos/modelo-tcc/"
}
```
Atenção às vírgulas: não deixe uma vírgula após o último campo ou o último projeto. Os nomes de situação precisam ser exatamente `Em desenvolvimento`, `Em avaliação` ou `Concluído`.

## 5. Criar página individual
1. Crie uma pasta, por exemplo `projetos/tcc-2026-001/`.
2. Crie dentro dela `index.html`.
3. Copie o conteúdo de `projetos/modelo-tcc/index.html` e substitua os campos entre colchetes.
4. No projeto em `projetos.json`, altere `pagina` para `projetos/tcc-2026-001/`.

## 6. Se o catálogo não carregar
- Confirme que `projetos.json` está na raiz, ao lado de `index.html`.
- Confira que os nomes são exatos e que as pastas `css` e `js` estão corretas.
- Confira se o JSON é válido e aguarde a publicação terminar.
- Como o site usa `fetch`, abrir `index.html` diretamente do computador pode não carregar os dados; teste depois de publicar no Pages.

## 7. Segurança
Revise nomes, fotos, relatórios, código e diagramas antes de publicar. Não inclua informações pessoais, documentos internos, senhas, tokens ou credenciais. Confirme autorização de divulgação.
