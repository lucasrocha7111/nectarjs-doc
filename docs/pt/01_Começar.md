# Instalação

É necessário possuir `NodeJS` para instalar o `NectarJS` : `https://nodejs.org/en/download/`.

Uma vez feito, instale o NectarJS : `npm install -g nectarjs`

Verifique se o NectarJS está instalado com o comando : `nectar --help`

# Configuração

É preciso inserir o seu id e o seu security key. O código é encriptado via AES durante a compilação.

Para configurar o seu id, use `--setid myid`

Para configurar a sua key, use `--setkey mykey`

# Compilação básica

A forma mais simples de usar o NectarJS :

```
nectar arquivo.js
```

O nome do arquivo de saída será escolhido automaticamente de acordo com o alvo. Você pode especificar outra saída com `-o something.out`

Pode selecionar o alvo para a compilação com `--target [THE TARGET]`

O argumento `--single` inicia a compilação do arquivo com o argumento. Se precisar de um arquivo com `require('')` na sua pasta atual, é preciso remover o `--single` e assim alterar para o modo projeto.

O NectarJS pode rodar diretamente a sua aplicação após a compilação se você especificar o `--run`. O programa será executado somente se o `--target` combinar com o seu sistema.

Para mais informações sobre a saída da compilação, use `--verbose`

Para ajuda, use `--help`
