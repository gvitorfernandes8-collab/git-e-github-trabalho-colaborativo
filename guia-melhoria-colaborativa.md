# Guia prático: melhoria de um projeto com branch e pull request

**Público-alvo:** integrantes que já conhecem os conceitos básicos de Git e GitHub.  
**Objetivo:** executar uma melhoria pequena e rastreável em um repositório compartilhado, usando a interface do GitHub no navegador.

Este guia complementa a [cartilha principal](cartilha.md) e o [roteiro da prática colaborativa](pratica-colaborativa.md). Os passos descrevem o fluxo; os resultados só devem ser registrados depois de serem executados pelas pessoas do grupo.

## 1. Antes de começar

Leia a tarefa e defina:

- **Problema:** o que precisa ser corrigido ou melhorado?
- **Escopo:** quais arquivos realmente precisam mudar?
- **Resultado esperado:** como outra pessoa poderá conferir que a melhoria ficou correta?
- **Revisor:** quem fará a leitura independente do pull request?

Antes de editar, abra a branch de destino (neste projeto, `main`) e confira se está visualizando a versão mais recente. Evite iniciar uma melhoria baseada em uma cópia antiga do arquivo.

## 2. Criar uma branch para a melhoria

Uma branch separa o trabalho em andamento da versão principal. Para criá-la pelo navegador:

1. Abra a página inicial do repositório.
2. Clique no seletor de branches, que normalmente mostra `main`.
3. Digite um nome curto que indique o objetivo, por exemplo `melhoria-guia`.
4. Escolha a opção para criar a branch a partir de `main`.
5. Confira o nome exibido no seletor antes de editar qualquer arquivo.

**Regra importante:** confirme a branch selecionada antes de salvar. Se a edição for feita em `main` por engano, pare e converse com o grupo antes de continuar.

## 3. Fazer a alteração e registrar o commit

1. Na branch de melhoria, abra o arquivo que será alterado.
2. Use o lápis (**Edit this file**) para editar ou **Add file** para criar um novo arquivo.
3. Faça uma mudança pequena, objetiva e relacionada ao problema definido.
4. Leia o texto novamente e confira links, títulos, listas e exemplos.
5. Na área **Commit changes**, escreva uma mensagem que descreva o que foi feito.
6. Confirme o commit na branch de melhoria e abra o histórico para verificar o registro.

Exemplos de mensagens claras:

- `docs: adiciona guia de revisão de pull request`
- `docs: esclarece etapas de criação de branch`
- `fix: corrige link da documentação`

Uma mensagem útil responde: **qual foi a mudança?** Evite textos vagos como `alterações`, `teste` ou `atualização`.

## 4. Abrir um pull request (PR)

O pull request propõe incorporar as alterações da branch de trabalho à branch principal. Ele não realiza o merge automaticamente.

1. Abra a aba **Pull requests**.
2. Clique em **New pull request**.
3. Selecione `main` como **base** (destino) e `melhoria-guia` como **compare** (origem).
4. Confira se os arquivos exibidos são exatamente os que deveriam mudar.
5. Use um título específico, por exemplo: **docs: aprimora o guia de colaboração**.
6. Na descrição, explique o contexto, as mudanças e como conferi-las.
7. Clique em **Create pull request**.

Modelo de descrição:

```markdown
## Objetivo
Explicar qual dificuldade ou necessidade motivou a melhoria.

## Alterações
- Descrever os arquivos e as seções modificadas.
- Resumir o benefício para quem está aprendendo.

## Conferência
- [ ] Li o conteúdo atualizado.
- [ ] Conferi títulos, links e exemplos.
- [ ] Comparei os arquivos em "Files changed".
- [ ] Não incluí dados pessoais, senhas ou tokens.
```

Antes de pedir revisão, abra **Files changed** e leia a comparação do início ao fim. O PR deve conter apenas mudanças relacionadas ao objetivo informado.

## 5. Fazer uma revisão útil

A revisão deve ser feita por outra pessoa, usando a própria conta GitHub. O autor da mudança não deve registrar uma aprovação em nome do revisor.

Quem revisa pode:

- verificar se a mudança atende ao objetivo descrito;
- conferir clareza, ortografia, links e consistência com o restante do material;
- apontar problemas em linhas específicas;
- comentar dúvidas ou sugerir ajustes;
- aprovar quando estiver satisfeito ou solicitar alterações quando encontrar problemas.

No GitHub, a revisão pode terminar como **Approve**, **Comment** ou **Request changes**. Um comentário não significa aprovação, e uma aprovação não substitui as regras de proteção ou verificações que o repositório eventualmente exigir.

### Como responder aos comentários

1. O autor lê cada observação e decide como corrigi-la.
2. Se necessário, faz novas alterações na **mesma branch** do PR.
3. Registra outro commit com uma mensagem específica.
4. Responde ao comentário explicando o ajuste ou a razão técnica para não alterá-lo.
5. O revisor confere novamente a versão atualizada.

Mantenha a conversa respeitosa e objetiva. Não resolva uma conversa de revisão antes de a questão estar realmente atendida.

## 6. Entender e resolver conflitos

Um conflito pode ocorrer quando duas mudanças incompatíveis atingem o mesmo trecho de um arquivo. O GitHub pode bloquear o merge até que ele seja resolvido.

Para conflitos simples apresentados pela interface:

1. Leia quais arquivos e trechos estão em conflito.
2. Compare as duas versões e identifique o conteúdo que deve permanecer.
3. Preserve as contribuições válidas de cada pessoa; não escolha uma versão sem conferir.
4. Use **Resolve conflicts** somente quando compreender o resultado.
5. Confira o arquivo completo depois da resolução e confirme a resolução.
6. Revise novamente a comparação do PR.

Se o conflito for complexo, envolver muitos arquivos ou não estiver claro qual conteúdo é correto, não force a resolução pelo navegador. Peça ajuda ao grupo e resolvam com cuidado antes de prosseguir.

## 7. Fazer merge e conferir o resultado

O merge deve acontecer somente depois da revisão combinada e das verificações exigidas pelo repositório.

1. Confira se os comentários importantes foram respondidos.
2. Verifique se não há conflitos ou verificações obrigatórias pendentes.
3. Leia novamente a aba **Files changed**.
4. Uma pessoa autorizada seleciona **Merge pull request** e confirma a operação.
5. Volte para `main` e abra os arquivos modificados.
6. Confirme que a alteração aprovada está na versão principal.
7. Se o grupo não precisar mais da branch, ela poderá ser excluída depois do merge; o histórico do PR continuará disponível.

As opções de merge podem variar conforme a configuração do projeto. Escolha a opção adotada pelo grupo e pela atividade.

## 8. Problemas comuns

| Situação | O que conferir |
|---|---|
| Não consigo editar ou enviar mudanças | Confirme se entrou na conta correta e se tem permissão de colaboração. |
| O PR aparece sem alterações | Confira se houve commit na branch de origem e se base/compare foram selecionadas corretamente. |
| O PR mostra arquivos inesperados | Revise a branch de origem e a comparação com `main` antes de pedir aprovação. |
| O GitHub bloqueia o merge | Leia os avisos: podem existir conflitos, revisões ou verificações pendentes. |
| A alteração não aparece em `main` | Confirme se o PR foi realmente mesclado e se está visualizando a branch `main`. |
| Duas pessoas editaram o mesmo trecho | Compare as versões e combine qual conteúdo deve permanecer; não sobrescreva sem revisar. |

## 9. Evidências para a atividade

Depois de executar o fluxo, guardem capturas reais que demonstrem:

- [ ] a branch de melhoria criada;
- [ ] o commit visível no histórico, com autor e mensagem;
- [ ] o pull request aberto, com `main` como destino;
- [ ] os arquivos e as alterações na comparação;
- [ ] a revisão feita pela pessoa responsável, com o resultado real;
- [ ] o merge concluído e a alteração visível em `main`.

Registrem os links do commit e do PR no arquivo [pratica-colaborativa.md](pratica-colaborativa.md). Não preencham campos com resultados esperados nem usem capturas montadas como se fossem evidências reais. Ocultem e-mails, notificações privadas e outras informações sensíveis.

## 10. Checklist final

- [ ] A branch foi criada a partir da versão atual de `main`.
- [ ] As alterações correspondem ao objetivo e estão na branch correta.
- [ ] A mensagem do commit descreve o trabalho.
- [ ] O PR compara a branch de melhoria com `main`.
- [ ] A descrição explica o contexto e a conferência realizada.
- [ ] Outra pessoa revisou usando sua própria conta.
- [ ] Os comentários foram tratados e as verificações necessárias foram concluídas.
- [ ] O merge foi feito por uma pessoa autorizada.
- [ ] A alteração foi conferida em `main`.
- [ ] Os links e as evidências reais foram registrados.

## Referências oficiais

- [GitHub Docs — Sobre branches](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches)
- [GitHub Docs — Criar um pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
- [GitHub Docs — Revisar alterações em pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests)
- [GitHub Docs — Sobre conflitos de merge](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/about-merge-conflicts)
- [GitHub Docs — Fazer merge de um pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/merging-a-pull-request)

**Observação:** as telas e os nomes dos botões podem mudar. Quando houver diferença, sigam os avisos apresentados pelo GitHub e confirmem o procedimento na documentação oficial.
