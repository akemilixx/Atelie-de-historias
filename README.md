# Ateliê de histórias

Site pessoal (GitHub Pages) para ideias, escritos e exercícios.
**Este repositório só tem o código.** Nenhum dado pessoal fica aqui: tudo é salvo
num repositório **privado** de quem está usando e só abre com o token dessa pessoa.

Qualquer pessoa pode usar o site com o próprio GitHub. Cada uma tem os seus dados
no seu próprio repositório privado, e ninguém vê os dados de ninguém.

## Como usar (para qualquer pessoa)

Você precisa de uma conta no GitHub. Não precisa instalar nada.

1. **Crie o repositório dos dados:** no GitHub, clique em *New repository*, escolha
   um nome (por exemplo `atelie-dados`) e marque **Private**. Pode deixar vazio.
2. **Crie um token:** GitHub → Settings → Developer settings → Personal access tokens →
   *Fine-grained tokens* → *Generate new token*:
   - Repository access: **Only select repositories** → escolha o repositório do passo 1
   - Permissions → Repository permissions → **Contents: Read and write**
   - Escolha a validade que preferir.
   - Copie o token gerado (começa com `github_pat_`). Ele só aparece uma vez.
3. **Entre no site** e preencha:
   - **Usuário do GitHub:** o seu nome de usuário
   - **Repositório privado dos dados:** o nome do repositório do passo 1
   - **Token de acesso:** o token do passo 2

Pronto. A partir daí, tudo o que você escrever é salvo automaticamente no seu
repositório privado.

### Cuidados

- **Use sempre um token fine-grained limitado a um único repositório**, como no
  passo 2. Não use token *classic*: ele dá acesso a todos os seus repositórios.
- **Computador compartilhado:** o token fica salvo no navegador. Ao terminar, use
  **Exportar → Sair deste aparelho** para apagá-lo.
- **Token expirou?** O site avisa e pede para entrar de novo. Gere um novo token
  (passo 2) e entre com ele. Os seus dados continuam no repositório.
- **Quer mais independência?** O token é digitado numa página hospedada por outra
  pessoa. Se preferir não depender dela, faça um *fork* deste repositório e publique
  a sua própria cópia (veja abaixo).

## Publicar a sua própria cópia do site

1. Faça um *fork* deste repositório (ou copie o `index.html` e o `.nojekyll`).
2. No seu repositório, Settings → Pages → *Deploy from a branch* → escolha a branch
   e a pasta `/ (root)`.
3. Abra o endereço que o GitHub Pages mostrar e siga os passos de "Como usar".

## Privacidade

- O site não tem servidor nem banco de dados: o navegador fala direto com a API do
  GitHub, usando o usuário, o repositório e o token de quem está usando.
- Quem abrir o site sem o token vê só a tela de entrada.
- O site recusa repositórios públicos para os dados.
- O token fica salvo apenas no navegador do aparelho; “Exportar → Sair deste aparelho” apaga.
- Os dados ficam em `data/*.json` no repositório privado (com histórico de versões).
