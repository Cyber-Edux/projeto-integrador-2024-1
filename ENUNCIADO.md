# Projeto Integrador

**Cyber Edux, Cuiabá-MT**

**Curso de Capacitação em Python (2023-2024)**

#### Resumo

Este repositório é o *template* do projeto integrador do curso de capacitação em Python oferecido pela Cyber Edux de setembro de 2023 a março de 2024. O projeto consiste em um *web-app* de gestão acadêmica desenvolvido em Python com o framework Django. O presente documento descreve os requisitos básicos do projeto e o sistema de avaliação, além de dar sugestões de recursos adicionais que podem ser implementados pelo aluno.

## 1. Introdução

Um projeto integrador é uma atividade desenvolvida para "forçar" o estudante a tentar aplicar o conhecimento que foi adquirido ao longo de um curso na resolução de problemas reais. Este tipo de atividade é fundamental em especial na área de desenvolvimento de *software* - uma área em que,  para alcançar o sucesso, o aluno deve praticar intensivamente e estudar de forma **contínua** do início ao fim de sua carreira. Tendo isso em vista, ministramos a presente atividade - cuja avaliação será o principal determinante da nota final do aluno - como um meio para que os alunos do curso de capacitação em Python da Cyber Edux exercitem algumas das habilidades mais importantes do mundo da programação: a capacidade de estruturar soluções para problemas complexos, a capacidade de reconhecer erros lógicos e causas de *bugs*, o autodidatismo, entre outras. O escopo proposto para o projeto é **gestão acadêmica**. A princípio, os alunos do curso devem desenvolver um sistema simples de gestão acadêmica para instituições com sistema de créditos - um "CRUD" de entidades acadêmicas, como estudantes, professores, cursos, disciplinas, salas, etc. A partir desta base, os alunos podem (se quiserem) explorar problemas mais complexos dentro do escopo proposto, como detecção de alocações conflitantes de horários e estatísticas de desempenho de estudantes. Iniciativas de desenvolver além dos requisitos básicos do projeto serão recompensadas nas avaliações.

Este documento está organizado da seguinte forma: 
* A seção de **requisitos básicos** contém os requisitos que o projeto proposto, em sua forma mais básica, deve cumprir.
* A seção de **método de avaliação** contém os critérios de avaliação e o sistema de pontuação que será utilizado para atribuir notas aos projetos.

## 2. Requisitos básicos

O mínimo que se espera que o aluno desenvolva é um pequeno CRUD de entidades acadêmicas como professor, disciplina, sala, curso, etc. CRUD, acrônimo de Create-Read-Update-Delete, é um termo frequentemente usado na área de desenvolvimento que denota um sistema desenvolvido para fazer não muito mais do que operações básicas de leitura e escrita de banco de dados. Como é uma aplicação *web*, devem haver páginas HTML com formulários, tabelas de consulta, e alguma estilização com CSS. O uso de um framework CSS (como o [Bootstrap](https://getbootstrap.com.br/)) é fortemente encorajado, embora não seja mandatório. O aluno é livre para definir a regra de negócio do sistema que irá desenvolver, porém o escopo deve ser gestão acadêmica.

Além de implementar o projeto, o aluno deve elaborar uma pequena documentação em *markdown* nos arquivos [README.md](README.md), [DOCUMENTACAO.md](DOCUMENTACAO.md) e [MANUAL.md](MANUAL.md).

## 4. Método de avaliação

### Critérios de avaliação

* **Seção A** - critérios de acordância com o escopo da atividade. 
* **Seção B** - esta seção contempla os critérios técnicos mais básicos possíveis. Caso o aluno apresente um projeto que, mesmo que não satisfaça os requisitos básicos da atividade, faça uso de uma parte dos conceitos aprendidos no curso, as notas desta seção garantem que a nota final deste aluno não seja zero.
* **Seção C** - os critérios desta seção são referentes aos requisitos básicos da atividade.
* **Seção D** - critérios de **qualidade de *software***, como usabilidade e tolerância a erros do usuário, entram nessa seção.
* **Seção E** - esta seção contempla as qualidades do projeto que extrapolam os requisitos básicos.

#### Seção A

| Componente da nota | Critério |
|:-:|:-:|
|$A_1$|Acordância com o escopo *gestão acadêmica*|
|$A_2$|Acordância com o tipo de projeto proposto: sistema *web*|

#### Seção B

| Componente da nota | Critério |
|:-:|:-:|
|$B_1$|Uso da linguagem Python|
|$B_2$|Código limpo e organizado|
|$B_3$|Uso de coleções de dados (lista, tupla, dicionário e conjunto)|
|$B_4$|Uso de recursos de manipulação de arquivos|
|$B_5$|Conexão com um banco de dados|
|$B_6$|Uso de alguma biblioteca gráfica que não seja um *framework web*, como Streamlit, Tkinter ou Qt|

| Nota no componente da seção A | Descrição |
|:-:|:-:|
| 0 | Critério não satisfeito |
| 1 | Critério satisfeito |

**Cálculo da nota final da seção B:**
$$B_\text{final} = \frac{B_1 + B_2 + B_3 + \min(B_4 + 2B_5, 2) + 3B_6}{8}$$

#### Seção C

| Componente da nota | Critério |
|:-:|:-:|
|$C_1$|Uso de um *framework web*, como Django ou Flask|
|$C_2$|Páginas HTML|
|$C_3$|Entrada e saída de dados nas páginas|
|$C_4$|Estilização com CSS|

| Nota no componente da seção C | Descrição |
|:-:|:-:|
| 0 | Critério não satisfeito |
| 1 | Critério satisfeito |

**Cálculo da nota final da seção C:**
$$C_\text{final} = \frac{4C_1 + C_2 + C_3 + C_4 + C_5}{8}$$

Observações:
* se o componente $C_1$ tiver nota 0, as seções C, D e E são zeradas.
* se o componente $C_2$ tiver nota 0, não há como atribuir nota 1 para os componentes $C_3$ e $C_4$.
#### Seção D

| Componente da nota | Critério |
|:-:|:-:|
|$D_1$|Tolerância às entradas erradas e mal uso|
|$D_2$|Robustez (quanto menos *bugs* o *software* tiver, mais robusto ele é)|
|$D_3$|Qualidade estética das páginas|
|$D_4$|Usabilidade (o quão intuitiva é a interface)|

| Nota no componente da seção D | Descrição |
|:-:|:-:|
| 0 | Não há material para avaliar |
| 1 | Baixa qualidade |
| 2 | Qualidade satisfatória |
| 3 | Boa qualidade |


**Cálculo da nota final da seção D:**
$$D_\text{final} = \frac{D_1 + D_2 + D_3 + D_4}{12}$$

#### Seção E

| Componente da nota | Critério | Descrição |
|:-:|:-:|:-:|
|$E_1$ | Páginas responsivas | Páginas responsivas são aquelas que podem ser usadas com facilidade em qualquer dispositivo (smartphone, tablet ou PC), pois se ajustam ao tamanho da tela. |
|$E_2$ | Uso de tecnologias extras | O uso de tecnologias não exigidas nos requisitos básicos, como um *framework* CSS, JavaScript e consumo de APIs, é recompensado neste critério.  |
|$E_3$ | Relevância e complexidade do problema resolvido | Há uma ampla gama de problemas computacionais que podem ser resolvidos no âmbito da gestão acadêmica, como problemas de logística (alocação de recursos), problemas de análise de dados e automatização de processos morosos. Caso o aluno cumpra todos os requisitos básicos e desenvolva uma solução para um problema real, sua iniciativa é recompensada com esta nota, que é dada de acordo com a relevância e a complexidade do problema escolhido. |
|$E_4$ | Relevância da solução desenvolvida | Qualquer problema computacional pode ter múltiplas soluções possíveis, e uma dessas soluções pode ser melhor do que as outras. A nota $E_4$ é definida de acordo com o quão bem o projeto do aluno resolve o problema que ele escolheu. |
