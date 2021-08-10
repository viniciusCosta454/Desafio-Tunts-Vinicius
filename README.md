# Desafio-Tunts

[Repositório GitHub](https://github.com/viniciusCosta454/Desafio-Tunts-Vinicius) | [Planilha](https://docs.google.com/spreadsheets/d/1mUTHvBLelwFduV0uSVvdi7P5N2Whry7CSwh42HcJcko/edit?usp=sharing)

The application must be able to read a google sheets spreadsheet, get the necessary information, calculate and write the result on the spreadsheet.



## Regras

Calcular a situação de cada aluno baseado na média das 3 provas (P1, P2 e P3), conforme a tabela:

| Média (m)  | Situação |
| ------------- | ------------- |
| m < 50  | Reprovado por Nota  |
| 5 <= m < 7  | Exame Final  |
| m >= 7  | Aprovado  |

Caso o número de faltas ultrapasse 25% do número total de aulas o aluno terá a situação "Reprovado por Falta", independente da média.

Caso a situação seja "Exame Final" é necessário calcular a "Nota para Aprovação Final"(naf) de cada aluno de acordo com seguinte fórmula: 

5 <= (m + naf)/2

Caso a situação do aluno seja diferente de "Exame Final", preencha o campo "Nota para Aprovação Final" com 0.

Arredondar o resultado para o próximo número inteiro (aumentar) caso necessário.

Utilizar linhas de logs para acompanhamento das atividades da aplicação.

Os textos do código fonte (atributos, classes, funções, comentários e afins) devem ser escritos em inglês, salvo os identificadores e textos pré-definidos nesse desafio.

O candidato deve especificar os comandos que devem ser utilizados para execução da aplicação. Exemplo de uma aplicação node.js:

```bash
    1.npm install
    2.npm start
```

O candidato deve publicar o código fonte em um repositório git de sua preferência (exemplo: github, gitlab, bitbucket e etc).
## Especificações técnicas

### Tecnologias utilizadas

- **Back-end:** NodeJs
- **Infra:** Git

### Instruções de instalação

First of all, you will need to install [NodeJS](https://nodejs.org/en/download/).
Afterwards, clone this repository on your machine:

```bash
git clone "https://github.com/Ploosh/Desafio-Tunts.git"
```

Install project dependencies:

```bash
cd "Desafio-Tunts"
npm install
```

To use the API it is necessary to create an authentication key. [Click here](https://theoephraim.github.io/node-google-spreadsheet/#/getting-started/authentication?id=service-account) to see how to create it.

Move the key to the ```Desafio-Tunts/src``` folder and rename it to **key.json**

On the [spreadsheet](https://docs.google.com/spreadsheets/d/1BCMGbmE_qGpHVhZYIfjb3L7MSERGYZkbkL0VMqDRu8k/edit?usp=sharing) page click "Share" and add the available email in your key.json file so that it is possible to write in the spreadsheet.
### Running the project locally

Open a terminal window in the project's root folder and run the backend:

```bash
npm run start
```

Follow the process on the table page(:
