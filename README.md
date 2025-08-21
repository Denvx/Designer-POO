# Esse reposiório descreve 3 ténicas dentro de POO

# Herança

- A herança, ela serve pra reaproveitamento de codigo, codigo que voce ia ficar repetindo em varios locais de sua api.
- nela, voce consegue sobrescrever os metodos criados na classe pai e adicionar coisas novas so a ela. mas cuidado que
- ela nao serve para tudo, as vezes, forçala deixa o sistema muito confuso. nesse caso, entra outro recurso que é a composição!

# Composição / Associação

- Associação, é quando conectamos uma classe a outra, mas sem "pai e filho" (herança), é uma relação direta entre classes, tipo um vinculo.
- Ex: Uma pessoa pode esta associada a um endereço. Mas pessoa não é um endereço, mas tem um endereço. aqui entramos em 1/1, 1/N ou N/N, uma pessoa
- tem um endereços, um professor tem varios alunos ou um aluno esta em varias turmas, e uma turma tem varios alunos

- A composição é um tipo de associação forte, porque uma é formada por outra. se a principal deixar de existir, a parte tambem deixa.
- Ex: Um carro é composto por um motor. Se o carro deixar de existir, o motor daquele #carro# tambem nao faz sentido.
- Ele se diferencia da Hereança porque: Herança "É UM" e a composição "TEM UM"
- Mas se carro tem, quem cria ? o propio carro ? ai vamos para a injeção de dependencia...

# Injeção de Dependencia

- A injeção de dependencia (DI - Dependency Injection), é um jeito de passar as dependencias de uma classe "de fora pra dentro", em vez da propia classe
- cria tudo sosinha, assim, ao invez de estar acoplada fortemente (que ficar dificil de usar), voce entrega pronto o que ela precisa, e ela so usa.
- lembra da composição "Carro tem um motor"? a injeção de dependencia cria e so entrega ao carro ! Parece uma pequena diferença, mas assim voce consegue deixar seu
- sistema muito flexivel e facil de dar manutenção, fazer textes e mais.
