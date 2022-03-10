Objetivos

1-`Explicar a diferença entre 'trhow' e 'return'`

2-`Apresentar a implementação da declaração try/catch`

## THROW

Exemplo:

`if(!string) throw "String Invalida";`

**enquanto o return retorna somente uma mensagem, o throw deixara claro que aquilo se trata de um erro e o console o tratara como tal**


## TRY .. CATCH

`O try ira verificar o codigo Caso tenha um erro o catch ira gerar um erro personalizado`

exemplo:

function tryCatchExemplo(string){
try{
    verificarPalindromo(string)
}
catch(e){
    throw e;
     <!-- // caso nao tivesse o throw o navegador mostrara um erro que vc definiu porem nao será tratado como um erro comum -->
}
}
tryCatchExemplo('');



## Finally

`O finally é uma instrução que vai ser chamada caso tenha erro ou não.`

Exemplo:
function tryCatchExemplo(string){
try{
    verificarPalindromo(string)
}
catch(e){
    throw e;
     
}
finally{
    console.log("A string enviada foi: "+string);
}
}
tryCatchExemplo('');

