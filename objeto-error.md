Objetivo

`Explicar como manipular o objeto error`

## OBJETO ERROR

[CODIGO:]

new Error(message,filename,linenumber)

//todos os parametros são opcionais
[Exemplo]:
const MeuErro = new Error('Mensagem Invalida');

throw MeuErro;


`O erro pode ter um nome tambem`

[Exemplo]:
const MeuErro = new Error('Mensagem Invalida');
MeuErro.name = 'InvalidMessage';
throw MeuErro;


