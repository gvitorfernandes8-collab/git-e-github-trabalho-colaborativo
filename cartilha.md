# Cartilha digital: primeiros passos com Git e GitHub

**Público-alvo:** pessoas iniciantes.  
**Objetivo:** criar um repositório, organizar arquivos, registrar alterações e colaborar pelo navegador.  
**Conhecimentos necessários:** navegação na internet e edição básica de texto. Não é necessário instalar programas nem usar o terminal.

**Autores:** Vitor Gomes Fernandes, Gustavo Kenji Noguchi e Bianca Souza Ferreira.

## 1. O que vamos aprender?

Ao final, você deverá conseguir explicar Git e GitHub, criar um repositório público ou privado, escrever um README em Markdown, enviar arquivos, registrar commits, consultar o histórico, convidar colaboradores e trabalhar com branch, pull request e merge.

## 2. Conceitos fundamentais

### Git e GitHub

**Git** é um sistema distribuído de controle de versão: registra alterações em arquivos e permite consultar versões anteriores. **GitHub** é uma plataforma on-line que hospeda repositórios Git e oferece recursos para compartilhar projetos, revisar contribuições e colaborar. Em resumo: Git controla as versões; GitHub oferece um espaço on-line para hospedar e colaborar.

### Repositório

Um **repositório** (ou *repo*) reúne os arquivos de um projeto e o histórico de alterações. Pode conter textos, imagens, documentos, códigos e pastas.

### Público ou privado?

- **Público:** qualquer pessoa pode visualizar o conteúdo.
- **Privado:** somente o proprietário e as pessoas autorizadas podem acessar.

Antes de publicar, verifique se não há senhas, tokens, códigos de autenticação, documentos pessoais ou dados de terceiros. Neste trabalho, o repositório está público: revisem tudo antes de enviar novos arquivos.

### README e Markdown

O arquivo **README.md** apresenta o projeto e costuma ser exibido na página inicial do repositório. A extensão `.md` indica uso de **Markdown**, uma forma simples de formatar texto.

| Objetivo | Sintaxe Markdown |
|---|---|
| Título | `# Título` |
| Subtítulo | `## Subtítulo` |
| Negrito | `**texto**` |
| Itálico | `*texto*` |
| Lista | `- item` |
| Link | `[texto](https://exemplo.com)` |
| Código em linha | `` `código` `` |

Exemplo:

```markdown
# Meu projeto de estudos

Este repositório reúne minhas anotações.

## Objetivos
- Aprender Git e GitHub.
- Praticar colaboração.
```

### Commit e histórico

Um **commit** é um registro de uma alteração no repositório, identificado por uma mensagem e associado a um autor e momento. Prefira mensagens claras, como `Adiciona explicação sobre README`. O **histórico** reúne os commits e permite conferir a evolução do projeto.

### Branch, pull request e merge

- **Branch:** linha de trabalho independente da principal. Permite experimentar mudanças sem alterar imediatamente a versão principal.
- **Pull request (PR):** proposta para incorporar as mudanças de uma branch em outra. Permite comparar arquivos, conversar e revisar antes da integração.
- **Merge:** integração das alterações propostas na branch de destino, depois da revisão e das verificações necessárias.

## 3. Primeiros passos pelo navegador

### Criar ou acessar uma conta

1. Acesse [github.com](https://github.com/).
2. Entre em **Sign in** ou crie uma conta em **Sign up**.
3. Use sua própria conta e confirme o e-mail se solicitado.
4. Nunca compartilhe sua senha com colegas.

### Criar um repositório

1. Entre no GitHub e abra o menu `+` no canto superior.
2. Selecione **New repository**.
3. Informe um nome sem espaços e uma descrição objetiva.
4. Escolha **Public** ou **Private**, conforme a orientação da atividade.
5. Se desejar iniciar com um README, marque **Add a README file**.
6. Clique em **Create repository**.

Um repositório privado só poderá ser avaliado por quem receber acesso. Um público pode ser visto por todos; revise o conteúdo antes de publicar.

### Criar ou enviar arquivos

1. Na página do repositório, clique em **Add file**.
2. Escolha **Create new file** para escrever no navegador ou **Upload files** para enviar arquivos existentes.
3. Informe o nome e a extensão, por exemplo `anotacoes.md`.
4. Escreva ou envie o conteúdo e confira a pré-visualização.
5. Em **Commit changes**, escreva uma mensagem que resuma a alteração.
6. Confirme em **Commit changes**.

Para criar uma pasta pelo editor, use um caminho como `images/LEIA-ME.md`.

## 4. Registrar contribuições e consultar versões

### Fazer uma contribuição

1. Abra o arquivo que deseja alterar.
2. Clique no lápis (**Edit this file**), se tiver permissão.
3. Acrescente uma explicação, exemplo ou correção relevante.
4. Confira a pré-visualização.
5. Escreva uma mensagem clara em **Commit changes**.
6. Confirme e abra novamente o arquivo para verificar a mudança.

Para o exercício, cada integrante deve contribuir com uma dica real no arquivo `pratica-colaborativa.md`, em sequência, usando sua própria conta.

### Consultar o histórico

1. Na página principal, abra a área **Commits** (histórico).
2. Confira mensagem, autor e data.
3. Abra um commit para ver os arquivos e as linhas alteradas.
4. Compare os registros com as contribuições combinadas pelo grupo.

## 5. Compartilhar o repositório

1. Abra o repositório e entre em **Settings**.
2. Acesse **Collaborators** ou a seção de acesso indicada na interface.
3. Clique em **Add people**.
4. Pesquise o nome de usuário GitHub da pessoa e envie o convite.
5. A pessoa convidada deve aceitar o convite em sua própria conta.
6. Confirme que ela aparece na lista de colaboradores.

Convide somente as pessoas necessárias. Não compartilhe credenciais. Para esta atividade, verifiquem também o acesso da professora indicada no enunciado.

## 6. Criar uma branch, abrir um pull request e fazer merge

### Criar uma branch

1. Na página do repositório, abra o seletor de branches, que normalmente mostra `main`.
2. Digite um nome, por exemplo `melhoria-guia`.
3. Selecione a opção para criar a branch a partir de `main`.
4. Confirme que a branch nova está selecionada antes de editar.

### Fazer uma alteração e abrir um PR

1. Edite um arquivo na branch nova e registre um commit.
2. Abra **Pull requests** e selecione **New pull request**.
3. Escolha `main` como base e `melhoria-guia` como compare.
4. Confira a comparação dos arquivos.
5. Dê um título e explique o motivo da mudança.
6. Clique em **Create pull request**.

### Revisar e mesclar

1. Outra pessoa do grupo abre o PR e confere as alterações.
2. Ela comenta o que está correto ou sugere melhorias.
3. O autor corrige o que for necessário.
4. Depois da revisão, uma pessoa autorizada seleciona **Merge pull request** e confirma.
5. Volte à branch `main` e confira se a mudança foi incorporada.

Não faça merge antes da revisão combinada. Se houver conflito ou opção diferente na interface, leiam as mensagens do GitHub e registrem o que ocorreu.

## 7. Desafio para praticar

Crie ou utilize um repositório de estudos, escreva um README com o objetivo e três assuntos que deseja aprender, adicione um arquivo de anotações e registre uma alteração com um commit claro. Compartilhe o repositório com um colega e confira a contribuição dele. Se possível, faça uma alteração em branch e proponha-a por pull request.

**Como conferir se concluiu:** o README está visível; o arquivo de anotações existe; o histórico mostra seu commit; o colega consegue acessar; e, se fizeram o desafio de revisão, o PR mostra a comparação e o resultado do merge.

## 8. Referências oficiais

- [GitHub Docs — Hello World: introdução prática](https://docs.github.com/en/get-started/start-your-journey/hello-world)
- [GitHub Docs — Sobre repositórios](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories)
- [GitHub Docs — Sobre o README](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [GitHub Docs — Sintaxe básica do Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [GitHub Docs — Convidar colaboradores](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/repository-access-and-collaboration/inviting-collaborators-to-a-personal-repository)
- [GitHub Docs — Editar arquivos](https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files)
- [GitHub Docs — Criar um pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- [GitHub Docs — Fazer merge de um pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/merging-a-pull-request)

**Uso responsável da IA:** a IA ajuda a organizar e explicar, mas não substitui documentação oficial nem testes. Confiram os links e testem as etapas nas próprias contas. O registro de prompts e conferência está em `registro-ia.md`.

---

**Fim da cartilha.** O aprendizado acontece quando cada integrante contribui, revisa e consegue explicar o que foi feito.
