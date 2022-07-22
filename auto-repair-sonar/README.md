# Plugin de reparo de violações do SonarQube na StackSpot

Esse plugin utiliza a bibilioteca [sorald](https://github.com/SpoonLabs/sorald) para realização de reparos automáticos em programas Java que violem um conjunto de regras do SonarQube. 

## Utilização

![Plugin de reparo automático na StackSpot](https://github.com/gustavopintozup/stk-dev-java/blob/main/repair-how-to.gif)

Para utilizar esse plugin, você precisa primeiro ter o o `stk` da StackSpot funcionando no seu computador.

Em seguida, você precisa importar essa stack deste repositório na sua instalação do `stk`:

```
stk import stack git@github.com:gustavopintozup/stk-dev-java.git
```

Para garantir que tanto a stack, quanto o plugin, foram importados corretamente, você pode executar os seguintes comandos:

```
stk list stack

stk list plugin
```

Após instalação da stack, basta rodar o plugin *dentro* do diretório do projeto que você deseja realizar as reparações.

```
cd <nome-do-meu-projeto>
stk apply plugin dev-java/auto-repair-sonar
```

## Dúvidas

Caso você tenha alguma dúvida ou dificuldade no uso, abra uma issue nesse repositório para que possamos auxilia-lo.