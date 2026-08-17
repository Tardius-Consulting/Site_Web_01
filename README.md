# Site_Web_01
Esse documento contem informações básicas para contribuições e desenvolvimento nesse projeto.

## Desenvolvimento
Para desenvolver nesse projeto você pode usar o comando 'git clone https://github.com/Tardius-Consulting/Site_Web_01.git' para copiar o repositório dirato para a pasta que você deseja desenvolver, ou então pode optar por baixar o repositório na pagina inicial como um arquivo zip e extraindo para a pasta de destino.

## Contribuição
Para enviar seu código para o repositório você deve primeiro usar o comando "git pull" para verificar se não existe nenhuma atualização, depois fazer o commit das modificações que você realizou em uma banch diferente da main, você pode verificar a branch que você está com o comando 'git branch' e pode criar uma nova branch com o comando 'git cheackout -b novaBranch', estando em uma nova branch você pode fazer o commit com o comando 'git commit -m "<tipo>(<escopo>): <descrição curta>"', após o commit você usar o comando 'git push -u origin novaBranch' para enviar as atualizações para o repositório.

Para garantir que você consiga enviar as contribuições você deve estar logado com sua conta do github no vscode ou incluir um tocken de acesso da sua conta do github no git para garantir a sua identidade.

Abaixo estão alguns exemplos de tipos e escopos para commits.

### 🎨 Tipos de Commits

* **`feat`**: Criação ou adição de um novo elemento visual ou página (ex: `feat(home): adiciona seção de contato`).
* **`fix`**: Correção de bugs visuais ou de funcionamento (ex: `fix(navbar): corrige alinhamento do menu no mobile`).
* **`style`**: Ajustes de estilo, cores, fontes ou espaçamentos que não mudam a estrutura (ex: `style(global): altera cor padrão do fundo`).
* **`docs`**: Atualizações na documentação ou no README (ex: `docs: adiciona instruções de como abrir o projeto`).
* **`refactor`**: Melhorias no código HTML, CSS ou JS que não alteram o visual nem corrigem erros (ex: `refactor(script): limpa código repetido do carrosel`).
* **`chore`**: Organização de arquivos, imagens ou limpeza do projeto (ex: `chore(assets): adiciona imagens da equipe`).

---

### 📂 Escopos Sugeridos para o Projeto

Para sabermos exatamente onde a alteração foi feita, use um destes escopos entre parênteses:

* `(page i)`: Página expecífica que a alteração afeta
* `(componente i)`: Componente expecífico alterado, mas que afeta várias páginas como rodapé, menus, etc.
* `(global)`: Arquivos globais (como `style.css` principal ou reset)

