# tf-09 — Atalho na árvore de arquivos

- **Encapsulamento:** quem usa o Atalho só precisa saber que existe `atalho.destino` para ler e `redirecionar()` para trocar; o atributo `__destino` e a validação que impede apontar para si mesmo ou para uma pasta acima ficam escondidos dentro da classe.
- **Herança:** quem usa sabe que o Atalho é um Item, então tem `nome`, `pai`, `mover_para()` e `caminho()`; como isso é implementado fica todo no Item, o Atalho não repete nada.
- **Polimorfismo:** quem chama só pede `tamanho()` ou `mostrar()`, sem perguntar o tipo; por baixo, o Atalho responde 1 byte e imprime `nome -> caminho do destino`, enquanto Pasta e Arquivo respondem do jeito deles.
