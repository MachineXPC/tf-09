# tf-09

Fiz um Atalho, tipo aquele do Windows, que só aponta pra outro arquivo ou pasta.

- **Encapsulamento:** pra usar, você só lê o `destino` e troca com `redirecionar()`. O `__destino` e a checagem que não deixa apontar pra ele mesmo ficam escondidos lá dentro.
- **Herança:** o Atalho é um Item, então já vem com nome, pai e caminho de graça. Não precisei escrever nada disso de novo.
- **Polimorfismo:** você chama `tamanho()` ou `mostrar()` sem saber o que é. O Atalho responde 1 byte e mostra `nome -> destino`, e a Pasta e o Arquivo respondem do jeito deles.
