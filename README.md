# Balta.io
Init the class

Padrão de Estilo para Mensagens Git
Definição de um padrão de estilo para escrita das mensagens do git commit.

Mensagens de commit
Na primeira linha resuma o commit em no máximo 72 caracteres (O commit pelo PyCharm já ajuda nisso);
Use SEMPRE o modo imperativo ("Adiciona feature" e não "Adicionando feature" ou "Adicionada feature");
Inicie as frases com letras maiúsculas;
Não termine a linha de resumo com ponto final (.);
Use uma linha em branco para separar a linha de resumo do corpo da mensagem;
Considere descrever com detalhes no corpo do commit (limitadas a 72 caracteres por linha);
No corpo explique "o que" e "por que" e não o "como";
Considere usar um emoji no início da mensagem de commit
Emoji	Code	Commit Type
🎉	:tada:	initial commit
🎨	:art:	quando melhorar a estrutura/formato do código
🐎	:racehorse:	quando melhorar a performance
📝	:memo:	quando escrever alguma documentação
🐛	:bug:	quando corrigir um bug
🔥	:fire:	quando remover códigos ou arquivos
💚	:green_heart:	quando corrigir uma build no CI
✅	:white_check_mark:	quando adicionar testes
🔒	:lock:	quando melhorar a segurança
⬆️	:arrow_up:	quando der upgrade em dependências
⬇️	:arrow_down:	quando der downgrade em dependências
💩	:poop:	deprecated
🚧	:construction:	em construção
🚀	:rocket:	nova feature
🙈	:see_no_evil:	gambiarra
🎁	:gift:	nova versão
Exemplo
git commit -m ":memo: Adiciona instruções sobre commits
>
> Foi criado o arquivo README.md com as instruções de
> como fazer um bom commit"
Exemplo de texto
Resumo das alterações com verbos no imprativo, 72 caracteres ou menos

Explique o problema que esse commit está resolvendo. Concentre-se em por que você
está fazendo essa alteração em vez de como (o código explica isso).
Existem efeitos colaterais ou outras conseqüências não intuitivas deste
mudança? Aqui é o lugar para explicá-los.

Outros parágrafos vêm após linhas em branco

 - Você pode usar bullets também;
 
 - Normalmente, um hífen ou asterisco é usado como marcador, precedido
   por um único espaço, com linhas em branco no meio

Se você usa um issue tracker, coloque referências a eles na parte inferior assim:

fix: #123 
Veja também: #456, #789
Por que uma boa mensagem importa?
Alguns motivos:
Caso um bug seja introduzido, uma boa mensagem de commit facilita a identificação de onde/quando isso aconteceu;
Se você reverter um commit, a mensagem será Revert "mensagem original", deixando claro o que está sendo revertido;
Boas mensagens se tornam útias ao exibir listas de commits através de comandos como git blame, git log, git shortlog, etc.
Referências
https://chris.beams.io/posts/git-commit/