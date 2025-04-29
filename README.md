# Explorando evolução de código

Neste exercício, iremos explorar a evolução de código em sistemas reais.

Iremos utilizar a ferramenta [GitEvo](https://github.com/andrehora/gitevo).
Essa ferramenta analisa a evolução de código em repositórios Git nas seguintes linguagens: Python, JavaScript, TypeScript e Java.

Você deve submeter via Moodle apenas o link do seu `fork`, conforme descrito abaixo.

# Passo 1: Selecionar repositório a ser analisado

Selecione um repositório relevante na linguagem de sua preferência (Python, JavaScript, TypeScript ou Java).
Você pode encontrar projetos interessantes nos links abaixo:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

# Passo 2: Instalar e rodar a ferramenta GitEvo

Instale a ferramenta [GitEvo](https://github.com/andrehora/gitevo) com o comando:

```
pip install gitevo
```

Rode a ferramenta no repositório selecionado através do seguinte comando (dependendo da linguagem do projeto que escolheu):

```shell
# Python
$ gitevo -r python <git_url>

# JavaScript
$ gitevo -r js <git_url>

# TypeScript
$ gitevo -r ts <git_url>

# Java
$ gitevo -r java <git_url>
```

Onde `<git_url>` é URL do repositório a ser analisado.
Por exemplo, para analisar o projeto Flask escrito em Python:

```
$ gitevo -r python https://github.com/pallets/flask
```

# Passo 3: Explorar os gráficos de evolução de código (`index.html`)

Ao rodar a ferramenta [GitEvo](https://github.com/andrehora/gitevo), o arquivo `index.html` é gerado com diversos gráficos de evolução de código.

Abra o arquivo `index.html` e observe com atenção os gráficos gerados.

# Passo 4: Explicar um gráfico de evolução de código

Selecione um dos gráficos de evolução e explique-o com suas palavras.
Por exemplo, você pode:

- Detalhar a evolução ao longo do tempo, 
- Detalhar se as curvas estão de acordo com boas práticas,
- Explicar grandes alterações nas curvas,
- Explorar a documentação do repositório em busca de explicações para grandes alterações
- Etc.

Seja criativo!

# Exercício

Para responder este exercício, primeiramente, você deve fazer um `fork` deste repositório.
No Moodle, você deve submeter apenas a URL do seu `fork`.

Em seguida, adicione o arquivo gerado `index.html` no seu fork.

Por fim, responda as questões abaixo no seu `fork`: 

1. Repositório selecionado: [Sherlock](https://github.com/sherlock-project/sherlock)

2. Gráfico selecionado: Production and test files
  
3. Explicação:

O gráfico intitulado "Production and test files" apresenta a evolução da quantidade de arquivos de produção e de teste ao longo dos anos de 2020 a 2025. No eixo horizontal (X) são indicados os anos, enquanto o eixo vertical (Y) mostra o número de arquivos. As linhas azul e rosa representam, respectivamente, os arquivos de produção e de teste.

Observa-se que, em 2020, o projeto contava com seis arquivos de produção e nenhum arquivo de teste. Em 2021, houve um crescimento no número de arquivos de produção, que alcançou dez, enquanto os arquivos de teste permaneceram ausentes. Nos anos de 2022 a 2024, o número de arquivos de produção manteve-se constante em dez unidades. Em 2023, surgem os primeiros registros de arquivos de teste, ainda de forma incipiente, com apenas um arquivo. Esta quantidade se manteve estável também em 2024.

Em 2025, é possível perceber duas mudanças significativas: uma redução no número de arquivos de produção, de dez para oito, e um expressivo aumento no número de arquivos de teste, que passou de um para seis. Este comportamento sugere um esforço de melhoria na qualidade do projeto, com uma atenção mais clara para a criação de testes, prática considerada fundamental em processos de desenvolvimento de software.

Do ponto de vista das boas práticas, a ausência de testes até 2022 representa um risco elevado para a manutenção e evolução segura do projeto. Entretanto, a partir de 2023, a inclusão progressiva de testes demonstra uma mudança positiva na abordagem da equipe de desenvolvimento. O crescimento expressivo da quantidade de arquivos de teste em 2025 é um forte indicativo de amadurecimento no processo de desenvolvimento, mostrando maior preocupação com a qualidade e a confiabilidade do código.

A queda no número de arquivos de produção em 2025 pode ser interpretada como resultado de ações de refatoração, remoção de código obsoleto ou reorganização arquitetural, práticas que, se bem conduzidas, contribuem para a sustentabilidade e a eficiência do projeto. Para compreender em detalhes as razões dessa diminuição, seria necessário consultar os registros de commits ou a documentação do repositório.

Em síntese, a análise do gráfico revela uma trajetória de evolução do projeto no que diz respeito à adoção de práticas mais robustas de desenvolvimento, com a inclusão de testes e racionalização da base de código, o que tende a fortalecer a qualidade e a manutenibilidade do sistema a longo prazo.



