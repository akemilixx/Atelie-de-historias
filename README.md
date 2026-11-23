# Ateliê de histórias

Site pessoal (GitHub Pages) para ideias, escritos e exercícios.
**Este repositório só tem o código.** Nenhum dado pessoal fica aqui: tudo é salvo
num repositório **privado** separado e só abre com um token seu.

## Configuração (uma vez)

1. **Repositório dos dados:** crie um repositório **privado** chamado `atelie-dados`
   (pode ser vazio).
2. **Token:** em GitHub → Settings → Developer settings → Personal access tokens →
   *Fine-grained tokens* → *Generate new token*:
   - Repository access: **Only select repositories** → `atelie-dados`
   - Permissions → Repository permissions → **Contents: Read and write**
   - Escolha a validade que preferir.
3. **GitHub Pages:** neste repositório, Settings → Pages → *Deploy from a branch* →
   escolha a branch e a pasta `/ (root)`.
4. Abra o site, informe usuário, `atelie-dados` e o token. Pronto.

## Privacidade

- Quem abrir o site sem o token vê só a tela de entrada.
- O site recusa repositórios públicos para os dados.
- O token fica salvo apenas no navegador do aparelho; “Exportar → Sair deste aparelho” apaga.
- Os dados ficam em `data/*.json` no repositório privado (com histórico de versões).
