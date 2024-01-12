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

A avaliação é feita por com sistema de avaliação onde há critérios e escalas pré-definidos. Os critérios de avaliação e as escalas de pontuação estão separados em seções. Para cada seção, há uma fórmula de cálculo de nota da seção, que é sempre de 0 a 1. A nota final do projeto do aluno será calculada como uma soma ponderada das notas das seções.

### Critérios de avaliação
#### Seção A
Critérios de acordância com o escopo da atividade. 

| Componente da nota | Critério |
|:-:|:-:|
|$A_1$|Acordância com o escopo *gestão acadêmica*|
|$A_2$|Acordância com o tipo de projeto proposto: sistema *web*|

| Nota no componente da seção A | Descrição |
|:-:|:-:|
| 0.85 | Critério não satisfeito |
| 1 | Critério satisfeito |

**Cálculo da nota final da seção A:**
$$A_\text{final} = \frac{A_1 + A_2}{2}$$

#### Seção B
Esta seção contempla os critérios técnicos mais básicos possíveis. Caso o aluno apresente um projeto que, mesmo que não satisfaça os requisitos básicos da atividade, faça uso de uma parte dos conceitos aprendidos no curso, as notas desta seção garantem que a nota final deste aluno não seja zero.

| Componente da nota | Critério |
|:-:|:-:|
|$B_1$|Uso da linguagem Python|
|$B_2$|Código limpo e organizado|
|$B_3$|Uso de coleções de dados (lista, tupla, dicionário e conjunto)|
|$B_4$|Uso de recursos de manipulação de arquivos|
|$B_5$|Conexão com um banco de dados|


| Nota no componente da seção B | Descrição |
|:-:|:-:|
| 0 | Critério não satisfeito |
| 1 | Critério satisfeito |

**Cálculo da nota final da seção B:**
$$B_\text{final} = \frac{B_1 + B_2 + B_3 + \min(B_4 + 2B_5, 2)}{5}$$

#### Seção C
Os critérios desta seção são referentes aos requisitos básicos da atividade.

| Componente da nota | Critério |
|:-:|:-:|
|$C_1$|Construção de uma interface gráfica (com ou sem um *framework web*), ou uma API *web*|
|$C_2$|Uso de um *framework web*, como Django ou Flask|
|$C_3$|Páginas HTML|
|$C_4$|Entrada e saída de dados nas páginas|
|$C_5$|Estilização com CSS|

| Nota no componente da seção C | Descrição |
|:-:|:-:|
| 0 | Critério não satisfeito |
| 1 | Critério satisfeito |

**Cálculo da nota final da seção C:**
$$C_\text{final} = \frac{2C_1 + 2C_2 + C_3 + C_4 + C_5 + C_6}{8}$$

Observações:
* caso o componente $C_2$ seja satisfeito, o componente $C_1$ automaticamente também é satisfeito.
* se o componente $C_1$ tiver nota 0, as seções C, D e E são zeradas.
* se o componente $C_3$ tiver nota 0, não há como atribuir nota 1 para os componentes $C_4$ e $C_5$.
  
#### Seção D
Critérios de **qualidade de *software***, como usabilidade e tolerância a erros do usuário, entram nessa seção.

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
Esta seção contempla as qualidades do projeto que extrapolam os requisitos básicos do ponto de vista técnico (técnicas e tecnologias utilizadas).

| Componente da nota | Critério | Descrição |
|:-:|:-:|:-:|
|$E_1$ | Páginas responsivas | Páginas responsivas são aquelas que podem ser usadas com facilidade em qualquer dispositivo (smartphone, tablet ou PC), pois se ajustam ao tamanho da tela. |
|$E_2$ | Uso de tecnologias extras | O uso de tecnologias não exigidas nos requisitos básicos, como um *framework* CSS, JavaScript e consumo de APIs, é recompensado neste critério.  |

| Nota no componente da seção E | Descrição |
|:-:|:-:|
| 0 | Critério não satisfeito |
| 1 | Critério parcialmente satisfeito |
| 2 | Critério satisfeito |

**Cálculo da nota final da seção E:**
$$E_\text{final} = \frac{E_1 + E_2}{2}$$

#### Seção F
Esta seção contempla as qualidades da ideia do projeto.

| Componente da nota | Critério | Descrição |
|:-:|:-:|:-:|
|$F_1$ | Relevância e complexidade do problema resolvido | Há uma ampla gama de problemas computacionais que podem ser resolvidos no âmbito da gestão acadêmica, como problemas de logística (alocação de recursos), problemas de análise de dados e automatização de processos morosos. Caso o aluno cumpra todos os requisitos básicos e desenvolva uma solução para um problema real, sua iniciativa é recompensada com esta nota, que é dada de acordo com a relevância e a complexidade do problema escolhido. |
|$F_2$ | Relevância da solução desenvolvida | Qualquer problema computacional pode ter múltiplas soluções possíveis, e uma dessas soluções pode ser melhor do que as outras. A nota $F_2$ é definida de acordo com o quão bem o projeto do aluno resolve o problema que ele escolheu. |

| Nota no componente da seção F | Descrição |
|:-:|:-:|
| 0 | Baixa relevância - problema ou solução simples e sem aplicabilidade prática ou com aplicabilidade muito limitada. |
| 1 | Relevância moderada - problema ou solução de complexidade baixa com grande aplicabilidade prática. |
| 2 | Relevância alta - problema ou solução de complexidade média com grande aplicabilidade prática. |
| 3 | Relevância muito alta - apenas para casos excepcionais, em que a complexidade do problema ou solução é alta e tem grande aplicabilidade prática. |


**Cálculo da nota final da seção F:**
$$F_\text{final} = \frac{F_1 + F_2}{2}$$

### Cálculo na nota final

$$N_\text{final} = A_\text{final}\left(4B_\text{final} + 3C_\text{final} + 2D_\text{final} + \frac{1}{2}E_\text{final} + \frac{1}{2}F_\text{final}\right)$$