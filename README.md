# Aprendendo Programação em C
#### Um jeito diferente de aprender programação.

## Atividade Planejada de Fixação

>	(Desafio)Complete o código abaixo elaborando as questões das opções de menu apresentadas na função questoes(). Implemente o uso de um laço de repetição (loop) até que o estudante digite 11 (Sair). Cada questão tem sua propria função. A elaboração da questão fica a seu critério para cada assunto listado no menu de questões. Ao final, execute o código e veja se o programa roda perfeitamente. (1,5 - Um ponto e meio na nota 3).
```C
// Online C compiler to run C program online
#include <stdio.h>

void cabecalho(){
    printf("\nMinistério da Educação");
    printf("\nUniversidade Federal do Piauí");
    printf("\nDepartamento de Tecnologia");
    printf("\nCurso de Engenharia Civil");
}

int questoes(){
    int questao;
    printf("\n[1] - Tecnologia");
    printf("\n[2] - Lógica");
    printf("\n[3] - Estrutura básica de C");
    printf("\n[4] - Variaveis");
    printf("\n[5] - Tipo de dados e condicionais");
    printf("\n[6] - Laços de repetição");
    printf("\n[7] - Funções sem parâmetros");
    printf("\n[8] - Funções com parâmetros");
    printf("\n[9] - Vetores");
    printf("\n[10] - Registros");
    printf("\n[11] - Sair");
    printf("\nQual questão você deseja fazer.: ");
    scanf("%d",&questao);
    return questao;
}

void questao01(){
    int x;
    fflush(stdin);
    printf("\n\nO que significa na sua opinião 'informática'?");
    printf("\n[1] - Tecnologias de processamento em meio digital");
    printf("\n[2] - Informação automática");
    printf("\n\nEscolha.: ");
    scanf("%d",&x);
    if (x == 1){
        printf("\nmenos um ponto.");
    }else{
        printf("\nacertou. Um ponto");
    }
}

void questao02(){
  int a;
  fflush(stdin);
  printf("\n\nNo que diz respeito ao uso de condições compostas, quando queremos que as duas condições sejam necessariamente atingidas, usamos OU:");
  printf("\n[1] - certo");
  printf("\n[2] - errado");
  printf("\nEscolha.:");
  scanf("%d",&a);
  if(a ==2){
      printf("\nAcertou. Um ponto");
  }else{
      printf("\nErrou. Menos um ponto");
  }
  
}

void questao03(){
    int b;
    fflush(stdin);
    printf("\n\n Para que serve o comando printf:");
    printf("\n[1] - Encerrar o programa");
    printf("\n[2] - escrever na tela");
    printf("\n[3] - ler strings");
    printf("\n\nEscolha.:");
    scanf("%d",&b);
    if(b==2){
        printf("\nAcertou. Um ponto");
    }else{
        printf("\nErrou. Menos um ponto");
    }
}
    
void questao04(){
    int c;
    fflush(stdin);
    printf("\n\nAssinale a alternativa correspondente a entrada para strings:");
    printf("\n[1] - gets");
    printf("\n[2] - scanf");
    printf("\n[3] - printf");
    printf("\n\nEscolha.:");
    scanf("%d",&c);
    if(c==1){
        printf("\nAcertou. Um ponto");
    }else{
        printf("\nErrou. Menos um ponto");
    }
    
}
void questao05(){
    int d;
    fflush(stdin);
    printf("\n\nQual o simbolo é usado para representar a condição de diferente:");
    printf("\n[1] - ==");
    printf("\n[2] - !=");
    printf("\n\nEscolha.:");
    scanf("%d",&d);
    if(d==2){
        printf("\nAertou. Um ponto");
    }else{
        printf("\nErrou. Menos um ponto");
    }
    
}

void questao06(){
    int e;
    fflush(stdin);
    printf("\n\nQual dos seguintes laços de repetição conta com incremento automático do contador");
    printf("\n[1] - for");
    printf("\n[2] - while");
    printf("\n[3] - do...while");
    printf("\n\nEscolha.:");
    scanf("%d",&e);
    if(e==1){
        printf("\nAcertou. Um ponto");
    }else{
        printf("\nErrou. Menos um ponto");
    }
    
}

void questao07(){
    int f;
    fflush(stdin);
    printf("\n\n int main é a forma correta de declarar uma função sem parametros em C");
    printf("\n[1] - Certo");
    printf("\n[2] - Errado");
    printf("\n\nEscolha.:");
    scanf("%d",&f);
    if(f==2){
        printf("\nAcertou. Um ponto");
    }else{
        printf("\nErrou. Menos um ponto");
    }
    
}

void questao08(){
    int g;
    fflush(stdin);
    printf("\n\n void soma(int a,int b){return a+b;} é a forma correta de definir uma função dois parametros inteiros, de forma que ela retorne a soma desses valores?");
    printf("\n[1] - Certo");
    printf("\n[2] - Errado");
    printf("\n\nEscolha.:");
    scanf("%d",&g);
    if(g==2){
        printf("\nAcertou. UM ponto");
    }else{
        printf("\nErrou. Menos um ponto");
    }
    
    
}

void questao09(){
    int h;
    fflush(stdin);
    printf("\n\nTodo vetor em C começa a indexar por qual posição?");
    printf("\n[1] - 0");
    printf("\n[2] - 1");
    printf("\n\nEscolha.:");
    scanf("%d",&h);
    if(h==1){
        printf("\nAcertou. um ponto");
    }else{
        printf("\nErrou. menos um ponto");
    }
    
    
}
void questao10(){
    int i;
    fflush(stdin);
    printf("\n\nComo é chamado o registro em linguagem C?");
    printf("\n[1] - STRUCT");
    printf("\n[2] - scanf");
    printf("\n\nEscolha.:");
    scanf("%d",&i);
    if(i==1){
        printf("\nAcertou. um ponto");
    }else{
        printf("\nErrou. Menos um ponto");
    }
    
}
int main() {
    int opc;
    cabecalho();
    printf("\n----------------------------------------------------------------------");
    opc = questoes();
    while(opc!=11){
        printf("\n\nQual questão voce deseja fazer.:");
        scanf("%d",&opc);
    switch(opc){
        case 1: {
            questao01();break;
        }
        case 2: {
            questao02();break;
        }
        case 3:{
            questao03();break;
        }
        case 4:{
            questao04();break;
        }
        case 5:{
            questao05();break;
        }
        case 6:{
            questao06();break;
        }
        case 7:{
            questao07();break;
        }
        case 8:{
            questao08();break;
        }
        case 9:{
            questao09();break;
        }
        case 10:{
            questao10();break;
        }
    }
    }
    return 0;
}
```
```C
// Online C compiler to run C program online
#include <stdio.h>

void cabecalho(){
    printf("\nMinistério da Educação");
    printf("\nUniversidade Federal do Piauí");
    printf("\nDepartamento de Tecnologia");
    printf("\nCurso de Engenharia Civil");
}

int questoes(){
    int questao;
    printf("\n[1] - Tecnologia");
    printf("\n[2] - Lógica");
    printf("\n[3] - Estrutura básica de C");
    printf("\n[4] - Variaveis");
    printf("\n[5] - Tipo de dados e condicionais");
    printf("\n[6] - Laços de repetição");
    printf("\n[7] - Funções sem parâmetros");
    printf("\n[8] - Funções com parâmetros");
    printf("\n[9] - Vetores");
    printf("\n[10] - Registros");
    printf("\n[11] - Sair");
    printf("\nQual questão você deseja fazer.: ");
    scanf("%d",&questao);
    return questao;
}

void questao01(){
    int x;
    fflush(stdin);
    printf("\n\nO que significa na sua opinião 'informática'?");
    printf("\n[1] - Tecnologias de processamento em meio digital");
    printf("\n[2] - Informação automática");
    printf("\n\nEscolha.: ");
    scanf("%d",&x);
    if (x == 1){
        printf("\nmenos um ponto.");
    }else{
        printf("\nacertou. Um ponto");
    }
}

void questao02(){
    
}

void questao03(){
    
}

void questao04(){
    
}
void questao05(){
    
}

void questao06(){
    
}

void questao07(){
    
}

void questao08(){
    
}

void questao09(){
    
}
void questao10(){
    
}
int main() {
    int opc;
    cabecalho();
    printf("\n----------------------------------------------------------------------");
    opc = questoes();
    switch(opc){
        case 1: {
            questao01();break;
        }
        case 2: {
            questao02();break;
        }
        case 3:{
            questao03();break;
        }
        case 4:{
            questao04();break;
        }
        case 5:{
            questao05();break;
        }
        case 6:{
            questao06();break;
        }
        case 7:{
            questao07();break;
        }
        case 8:{
            questao08();break;
        }
        case 9:{
            questao09();break;
        }
        case 10:{
            questao10();break;
        }
    }
    return 0;
}
```


## Vetor de registros

```C
#include <stdio.h>
#include<stdlib.h>

//Definindo a estrutura e criando o nosso cardápio
struct Cardapio{
    char tipoTapioca[30];
    int qtdBolo;
    char tipoCafe[20];
};
//Programa principal
int main() {
    //criando nosso vetor 'rest' do tipo estrutura de cardápio.
    struct Cardapio rest[2];
    //lendo os pedidos e preenchendo nosso registro.
    for (int i=0; i<2;i++){
        printf("\nTipo tapioca.: ");
        scanf("%s",rest[i].tipoTapioca);
        printf("\nQtd Bolo.: ");
        scanf("%d",&rest[i].qtdBolo);
        printf("\ntipo cafe.: ");
        scanf("%s",rest[i].tipoCafe);
    }
//Imprimindo todos os pedidos feitos	
    for (int i=0; i<2; i++){
        printf("\n-------------------------------------");
        printf("\ntapioca => %s",rest[i].tipoTapioca);
        printf("\nbolos=> %d",rest[i].qtdBolo);
        printf("\ncafe=> %s",rest[i].tipoCafe);
    }
    return 0;
}
```
>	QT13(crucial) - Altere o código acima para preencher um vetor de registros de 10 posições, ems seguida mostre todos os pedidos feitos. Após isso, crie seu próprio código de vetor de registro. Comente cada linha do código de acordo com seu entendimento.

# Registros em C - Uma forma legal de criar uma "ficha" sobre alguma coisa.
### Nos exemplos a seguir vamos ver códigos com Structs em C que representa um registro, ou seja, tipos diferentes de dados em uma mesma estrutura.
#### Observe o código abaixo auto-explicativo e faça as questões seguintes.

```C
#include <stdio.h>
#include <conio.h>
int main(void)
{
  /*Criando a struct */
  struct ficha_de_aluno
  {
    char nome[100];
    char disciplina[100];
    float nota_prova1;
    float nota_prova2;
  };
  
  /*Criando a variável aluno que será do
  tipo struct ficha_de_aluno */
  struct ficha_de_aluno aluno; //perceba que ficha_de_aluno é como se fosse um tipo. A vairável aluno está sendo criada com esse tipo.
  
  printf("\n---------- Cadastro de aluno -----------\n\n\n");
  
  printf("Nome do aluno ......: ");
  fflush(stdin);
  
  /*usaremos o comando fgets() para ler strings, no caso o nome
  do aluno e a disciplina.
  fgets(variavel, tamanho da string, entrada)
  como estamos lendo do teclado a entrada é stdin (entrada padrão),
  porém em outro caso, a entrada tambem poderia ser um arquivo */
  
  fgets(aluno.nome, 40, stdin);
  
  printf("Disciplina ......: ");
  fflush(stdin);
  fgets(aluno.disciplina, 40, stdin);
  
  printf("Informe a 1a. nota ..: ");
  
  scanf("%f", &aluno.nota_prova1);
  
  printf("Informe a 2a. nota ..: ");
  scanf("%f", &aluno.nota_prova2);
  
  printf("\n\n --------- Mostrando os dados da struct ---------\n\n");
  printf("Nome ...........: %s", aluno.nome);
  printf("Disciplina .....: %s", aluno.disciplina);
  printf("Nota da Prova 1 ...: %.2f\n" , aluno.nota_prova1);
  printf("Nota da Prova 2 ...: %.2f\n" , aluno.nota_prova2);
  
  getch();
  return(0);
}
```
>	QT11(0,25) - Crie estruturas novas e correlacione com sua realidade. Use estruturas de repetição e estruturas switch. Ao final, as fichas com os cadastros deverão ser apresentadas.
```C
#include <stdio.h>

#define MAX_ALUNOS 100

struct Aluno {
    char nome[50];
    int periodos;
    char curso[50];
};

void lerDadosAluno(struct Aluno *aluno) {
    printf("Digite o nome: ");
    scanf(" %[^\n]s", aluno->nome);

    printf("Digite o número de períodos cursados: ");
    scanf("%d", &(aluno->periodos));

    printf("Digite o curso: ");
    scanf(" %[^\n]s", aluno->curso);
}

void imprimirDadosAluno(struct Aluno aluno) {
    printf("Nome: %s\n", aluno.nome);
    printf("Períodos cursados: %d\n", aluno.periodos);
    printf("Curso: %s\n", aluno.curso);
}

int main() {
    struct Aluno alunos[MAX_ALUNOS];
    int numAlunos = 0;
    int opcao;

    printf("Selecione uma opção:\n");
    printf("1 - Inserir novo aluno\n");
    printf("0 - Encerrar programa\n");

    do {
        printf("\nOpção: ");
        scanf("%d", &opcao);

        switch (opcao) {
            case 1:
                if (numAlunos < MAX_ALUNOS) {
                    printf("\nAluno %d:\n", numAlunos + 1);
                    lerDadosAluno(&alunos[numAlunos]);
                    numAlunos++;
                } else {
                    printf("Limite máximo de alunos atingido.\n");
                }
                break;

            case 0:
                printf("Encerrando o programa...\n");
                break;

            default:
                printf("Opção inválida. Tente novamente.\n");
                break;
        }
    } while (opcao != 0);

    printf("\nDados dos alunos:\n");
    for (int i = 0; i < numAlunos; i++) {
        printf("\nAluno %d:\n", i + 1);
        imprimirDadosAluno(alunos[i]);
    }

    return 0;
}
```
>	QT12(0,25) - Crie estruturas em C para organizar alguma necessidade sua e realize o cadastro dos registros. Utilize estruturas de loop para realizar mais de um registro. Ao final, apresente todos os cadastros realizados. Justifique todo o seu código.
```C
#include <stdio.h>

#define MAX_MAT 10 // Define o número máximo de matérias

// Definição da estrutura para armazenar os dados de cada matéria
struct Materia {
    char nome[50];
    int aulasSemana;
    int horasEstudoExtra;
};

int main() {
    int numMaterias;

    printf("Digite o número de matérias no período: ");
    scanf("%d", &numMaterias);

    // Verifica se o número de matérias não excede o limite máximo
    if (numMaterias > MAX_MAT) {
        printf("Número de matérias excede o limite máximo.\n");
        return 1;
    }

    struct Materia materias[MAX_MAT]; // Cria um array de estruturas para armazenar os registros

    // Realiza o cadastro dos registros
    for (int i = 0; i < numMaterias; i++) {
        printf("\nMatéria %d:\n", i+1);
        printf("Digite o nome da matéria: ");
        scanf(" %[^\n]s", materias[i].nome); // Lê o nome da matéria, ignorando possíveis espaços em branco no início
        printf("Digite a quantidade de aulas por semana: ");
        scanf("%d", &materias[i].aulasSemana);
        printf("Digite a quantidade de horas de estudo extra classe: ");
        scanf("%d", &materias[i].horasEstudoExtra);
    }

    // Exibe os registros cadastrados
    printf("\nRegistros cadastrados:\n");
    for (int i = 0; i < numMaterias; i++) {
        printf("\nMatéria %d:\n", i+1);
        printf("Nome: %s\n", materias[i].nome);
        printf("Aulas por semana: %d\n", materias[i].aulasSemana);
        printf("Horas de estudo extra classe: %d\n", materias[i].horasEstudoExtra);
    }

    return 0;
}
Nesse programa eu busquei colocar em um único lugar dados que estão relacionados e que são fundamentais para a minha
vida acadêmica. Assim, criei um código que pudece dizer a quantidade de matérias que vou cursar em um dado período,
a quantidades de aulas que terei por semana em cada matéria e quantas horas terei para estudar nos tempos livres para
cada matéria.
```


# Funções em C

>	Declare funções. Uma com opção de menu para o R.U, Biblioteca Central, Teatro ou H.U e mostre-os na tela. Outra que mostre apenas uma saudação do dia após leitura do nome da pessoa. (QT9 - 0,25)
```C
#include <stdio.h>
#include <stdlib.h>

void mostrarMenu() {
    printf("Selecione uma opcao:\n");
    printf("1. R.U\n");
    printf("2. Biblioteca Central\n");
    printf("3. Teatro\n");
    printf("4. H.U\n");
    printf("Escolha uma opcao (1-4): ");
    
    int opcao;
    scanf("%d", &opcao);
    
    switch(opcao) {
        case 1:
            printf("Voce selecionou R.U\n");
            break;
        case 2:
            printf("Voce selecionou Biblioteca Central\n");
            break;
        case 3:
            printf("Voce selecionou Teatro\n");
            break;
        case 4:
            printf("Voce selecionou H.U\n");
            break;
        default:
            printf("Opcao invalida\n");
    }
}

void mostrarSaudacao() {
    char nome[100];
    printf("Digite seu nome: ");
    scanf("%s", nome);
    
    printf("Bom dia, %s!\n", nome);
}

int main() {
    mostrarMenu();
    mostrarSaudacao();
    
    return 0;
}
```

>	Declare funções para: Totalizar a quantidade de árvores em cada setor(CCHL, CCE, CT, CCN, DIE, CCS) da ufpi através de entrada de dados pelo teclado. Ao final mostrar o total de árvores na UFPI. (Q10 - 25).
```C
#include <stdio.h>

// Função para totalizar a quantidade de árvores em um setor específico
int totalizarArvoresSetor(char setor[]) {
    int quantidadeArvores;
    printf("Informe a quantidade de árvores no setor %s: ", setor);
    scanf("%d", &quantidadeArvores);
    return quantidadeArvores;
}

int main() {
    int totalUFPI = 0;

    // Totalizar árvores no setor CCHL
    int arvoresCCHL = totalizarArvoresSetor("CCHL");
    totalUFPI += arvoresCCHL;

    // Totalizar árvores no setor CCE
    int arvoresCCE = totalizarArvoresSetor("CCE");
    totalUFPI += arvoresCCE;

    // Totalizar árvores no setor CT
    int arvoresCT = totalizarArvoresSetor("CT");
    totalUFPI += arvoresCT;

    // Totalizar árvores no setor CCN
    int arvoresCCN = totalizarArvoresSetor("CCN");
    totalUFPI += arvoresCCN;

    // Totalizar árvores no setor DIE
    int arvoresDIE = totalizarArvoresSetor("DIE");
    totalUFPI += arvoresDIE;

    // Totalizar árvores no setor CCS
    int arvoresCCS = totalizarArvoresSetor("CCS");
    totalUFPI += arvoresCCS;

    // Mostrar o total de árvores na UFPI
    printf("\nTotal de arvores na UFPI: %d\n", totalUFPI);

    return 0;
}
```
# Vetores em C
Declarar e preencher um vetor em C nos possibilita muitas utilizações. Observe a estrutura básica de um vetor em C.
Observe o código abaixo.
```C
#include <stdio.h>

int main()
{
    int meuVetor[3];
    
    meuVetor[0] = 32;
    meuVetor[1] = 10;
    meuVetor[2] = 5;
    
    printf("O valor dos vetores é: %d\n",meuVetor[0]);
    printf("O valor dos vetores é: %d\n",meuVetor[1]);
    printf("O valor dos vetores é: %d\n",meuVetor[2]);
    
    return 0;
}
```
>	QT04 (0,25 pontos) - Altere o código acima para 10 posições de vetor atribuindo 10 valores inteiros manuais e imprimindo todos eles na tela.
```C
#include <stdio.h>

int main()
{
    int meuVetor[10];
    
    meuVetor[0] = 32;
    meuVetor[1] = 10;
    meuVetor[2] = 5;
    meuVetor[3] = 14;
    meuVetor[4] = 22;
    meuVetor[5] = 27;
    meuVetor[6] = 11;
    meuVetor[7] = 3;
    meuVetor[8] = 19;
    meuVetor[9] = 7;
    
    printf("O valor do vetor na posição 0 é: %d\n", meuVetor[0]);
    printf("O valor do vetor na posição 1 é: %d\n", meuVetor[1]);
    printf("O valor do vetor na posição 2 é: %d\n", meuVetor[2]);
    printf("O valor do vetor na posição 3 é: %d\n", meuVetor[3]);
    printf("O valor do vetor na posição 4 é: %d\n", meuVetor[4]);
    printf("O valor do vetor na posição 5 é: %d\n", meuVetor[5]);
    printf("O valor do vetor na posição 6 é: %d\n", meuVetor[6]);
    printf("O valor do vetor na posição 7 é: %d\n", meuVetor[7]);
    printf("O valor do vetor na posição 8 é: %d\n", meuVetor[8]);
    printf("O valor do vetor na posição 9 é: %d\n", meuVetor[9]);
    
    return 0;
}
```


Para cada valor a partir da posição zero do vetor, temos um elemento. Cada posição é representada pelo símbolo de colchetes. Sempre iniciará da posição zero. Dessa forma, se o vetor de elementos tem 3 posições corresponderá às posições 0,1,2 (três elementos). A mesma ideia se aplica a qualquer quantidade de elementos.
Quando essa quantidade é bem grande, usamos laços de repetição. Observe o código abaixo.

```C
#include <stdio.h>
// Cada posição i do vetor é um valor multiplicado por 2. Usamos um for para preencher e outro for para mostrar.
int main()
{
    int meuVetor[10];
    
    for (int i=0; i<10; i++){
        meuVetor[i] = i*2;
    }
    for (int i=0; i<10; i++){
        printf("Posição %d e valor => %d \n",i,meuVetor[i]);
    }
    return 0;
}

```
>	QT05 (0,25 pontos) - Altere o código acima para que seja lido diretamente do teclado um valor inteiro, ao invés de atribuído. Mostre todos os valores lidos ao final.
```C
#include<stdio.h>
int main()
{
     int meuVetor[10];
     int numero;
     
     for(int i=0; i<10; i++){
     	printf("Digite um valor inteiro: ");
     	scanf("%d",&numero);
     	meuVetor[i]=numero*2;
     }
     for(int i=0; i<10; i++){
     	printf("Posição %d e valor => %d \n",i,meuVetor[i]);
     }
}
```


Em algumas situações temos que impor condições para obter dados de tudo o que foi lido e armazenado em uma lista de vetores. Vejamos um exemplo no código abaixo:
```C
#include <stdio.h>

int main()
{
    int meuVetor[10]; 	//vetor de 10 elementos
    int numero;		//variável inteira
    int pos = 0;	//variável inteira e inicializada com zero
    int neg = 0;	// outra inteira e inicializada com zero	

//Essa estrtura for preenche o vetor
    for (int i=0; i<10; i++){
        printf("Digite um valor para o vetor: ");
        scanf("%d",&numero);
        meuVetor[i] = numero;
    }
//Essa verifica uma condição e totaliza os valores.
    for (int i=0; i<10; i++){
        if(meuVetor[i] > 0){
            pos = pos + 1;
        }else neg = neg + 1;
    }
//Ao final do código, mostra os valores totalizados.
    printf("Quantidade de numeros positivos: %d \n",pos);
    printf("Quantidade de numeros negativos: %d \n",neg);
    return 0;
}
```
>	QT06 (0,5 - pontos) - Crie um código onde sejam lidos 20 votos. Os votos serão armazenados em um vetor inteiro de elementos. Cada número do voto corresponde a um time de futebol que será mostrado em um menu com 4 opções sendo elas: Flamengo, Vasco, São Paulo, Corinthians. Totalize os votos ao final e mostre na tela.
```C
#include <stdio.h>

int main()
{
    int votos[20]; // Vetor para armazenar os votos
    int flamengo = 0, vasco = 0, saoPaulo = 0, corinthians = 0; // Variáveis para totalizar os votos

    printf("Digite os votos (1-Flamengo, 2-Vasco, 3-São Paulo, 4-Corinthians):\n");

    // Ler os votos
    for (int i = 0; i < 20; i++) {
        printf("Voto %d: ", i+1);
        scanf("%d", &votos[i]);

        // Verificar o voto e atualizar a contagem
        switch (votos[i]) {
            case 1:
                flamengo++;
                break;
            case 2:
                vasco++;
                break;
            case 3:
                saoPaulo++;
                break;
            case 4:
                corinthians++;
                break;
            default:
                printf("Voto inválido. Tente novamente.\n");
                i--; // Decrementar o contador para repetir a leitura do voto inválido
        }
    }

    // Exibir a contagem dos votos
    printf("Total de votos:\n");
    printf("Flamengo: %d\n", flamengo);
    printf("Vasco: %d\n", vasco);
    printf("São Paulo: %d\n", saoPaulo);
    printf("Corinthians: %d\n", corinthians);

    return 0;
}
```

>	QT07 (0,5 - pontos) - Refaça a mesma questão anterior utilizando o While e acrescentando uma condição de parada chamada "Totalizar" representada pelo número 99 no menu.
```C
#include <stdio.h>

int main()
{
    int votos[20]; // Vetor para armazenar os votos
    int flamengo = 0, vasco = 0, saoPaulo = 0, corinthians = 0; // Variáveis para totalizar os votos
    int voto = 0; // Variável para ler o voto

    printf("Digite os votos (1-Flamengo, 2-Vasco, 3-São Paulo, 4-Corinthians):\n");

    // Ler os votos
    int i = 0;
    while (i < 20) {
        printf("Voto %d: ", i+1);
        scanf("%d", &voto);

        // Verificar o voto e atualizar a contagem
        if (voto == 99) {
            break; // Condição de parada "Totalizar" (99)
        } else if (voto >= 1 && voto <= 4) {
            switch (voto) {
                case 1:
                    flamengo++;
                    break;
                case 2:
                    vasco++;
                    break;
                case 3:
                    saoPaulo++;
                    break;
                case 4:
                    corinthians++;
                    break;
            }
            i++; // Incrementar o contador apenas se o voto for válido
        } else {
            printf("Voto inválido. Tente novamente.\n");
        }
    }

    // Exibir a contagem dos votos
    printf("Total de votos:\n");
    printf("Flamengo: %d\n", flamengo);
    printf("Vasco: %d\n", vasco);
    printf("São Paulo: %d\n", saoPaulo);
    printf("Corinthians: %d\n", corinthians);

    return 0;
}
```


>	QT08 (0,5 - pontos) - Crie um vetor de 20 posições para ler números correspondente ao estilo musical da turma (1 - Sertanejo, 2 - Internacional, 3 - Pop, 4 - Coreano, 5 - Forró, 6 - Funk, 7 - Gospel, 8 - Rock, 9 - Eletrônica, 10 - Classica). Totalize os votos por estilo e mostre ao final. Utilize o Do..while.
```C
#include <stdio.h>

int main() {
    int votos[20]; // vetor para armazenar os votos
    int contagem[10] = {0}; // vetor para contar os votos por estilo musical
    int i, estilo;

    printf("Digite o número correspondente ao estilo musical da turma:\n");
    printf("1 - Sertanejo\n2 - Internacional\n3 - Pop\n4 - Coreano\n5 - Forró\n");
    printf("6 - Funk\n7 - Gospel\n8 - Rock\n9 - Eletrônica\n10 - Clássica\n");

    i = 0;
    do {
        printf("Voto %d: ", i + 1);
        scanf("%d", &estilo);

        if (estilo >= 1 && estilo <= 10) {
            votos[i] = estilo;
            contagem[estilo - 1]++; // incrementa a contagem do estilo correspondente
            i++;
        } else {
            printf("Estilo inválido. Digite novamente.\n");
        }
    } while (i < 20);

    printf("\nResultados da votação:\n");
    printf("-----------------------\n");

    for (i = 0; i < 10; i++) {
        switch (i + 1) {
            case 1:
                printf("Sertanejo: %d votos\n", contagem[i]);
                break;
            case 2:
                printf("Internacional: %d votos\n", contagem[i]);
                break;
            case 3:
                printf("Pop: %d votos\n", contagem[i]);
                break;
            case 4:
                printf("Coreano: %d votos\n", contagem[i]);
                break;
            case 5:
                printf("Forró: %d votos\n", contagem[i]);
                break;
            case 6:
                printf("Funk: %d votos\n", contagem[i]);
                break;
            case 7:
                printf("Gospel: %d votos\n", contagem[i]);
                break;
            case 8:
                printf("Rock: %d votos\n", contagem[i]);
                break;
            case 9:
                printf("Eletrônica: %d votos\n", contagem[i]);
                break;
            case 10:
                printf("Clássica: %d votos\n", contagem[i]);
                break;
            default:
                break;
        }
    }

    return 0;
}
```

## Revisando estrutura básica

##### Aqui você irá ver de novo e praticar a estrutura básica.

> Usando o compilador C online repassado para a turma {https://www.onlinegdb.com/online_c_compiler} reescreva o código abaixo:
```C
#include<stdio.h>
int main(){
	int a;
	a = 20;
	printf("o valor de a é: %d",a);
}
```
Na estrutura básica temos:
>	#include<stdio.h>
>	int main()
> 	{} //chaves para o escopo do código.
### Atividade QT01 (0,1 pontos) - Reescreva o código criando mais duas variáveis inteiras e mostre-as na saída padrão.
```C
#include <stdio.h>

int main()
{
    int a, b, c;
    
    a = 20;
    b = 15;
    c = 10;
    
    printf("O valor de a é: %d\n", a);
    printf("O valor de b é: %d\n", b);
    printf("O valor de c é: %d\n", c);
    
    return 0;
}
```

## Revisando estrutura condicional.

##### Aqui você irá ver de novo e praticar as condicionais de C.

> Usando o compilador C online repassado para a turma {https://www.onlinegdb.com/online_c_compiler} reescreva o código abaixo:
```C
#include <stdio.h>
int main(){
	int a;
	a = 20;
	if (a < 20){
		printf("O valor é menor que 20");
	}
}
```
Na estrutura acima temos:
>	O uso de uma estrutura condicional com o if
>	Seu escopo também inicia com chaves e termina com chaves.
### Atividade QT02 (0,1 pontos) - Reescreva o código criando mais uma estrutura if para uma frase se valores de a forem maiores que 20.
```C
#include <stdio.h>
int main(){
    int a;
    a = 20;
    
    if (a < 20) {
        printf("O valor é menor que 20\n");
    }
    else if (a > 20) {
        printf("O valor é maior que 20\n");
    }
return 0;
}
```

## Revisando estrutura condicional com if - else.

##### Aqui você irá ver de novo e praticar as condicionais de C com if - else.

> Usando o compilador C online repassado para a turma {https://www.onlinegdb.com/online_c_compiler} reescreva o código abaixo:
```C
#include <stdio.h>
int main(){
	int a;
	a = 20;
	if (a < 20){
		printf("O valor é menor que 20");
	}else{
		printf("esse é maior");
	}
}
```
Na estrutura acima temos:
>	O uso de uma estrutura condicional com o if e outra para o else
>	Seu escopo também inicia com chaves e termina com chaves também.
### Atividade QT03 (0,1 pontos) - Reescreva o código com estrutura if-else para uma frase se valores forem negativos ou positivos.
```C
#include <stdio.h>

int main() {
    int a;
    a = 20;

    if (a < 0) {
        printf("O valor é negativo.\n");
    } else if (a > 0) {
        printf("O valor é positivo.\n");
    } else {
        printf("O valor é zero.\n");
    }

    return 0;
}
```

## Revisando Laços de Repetição: for.
##### Nessa atividade iremos revisar através de código escrito em C, como podemos trabalhar com esse tipo de variável que pode armazenar dados de um único tipo.

>  Usando novamente o "for" em C.
```C
int main(){
  
  //Vamos criar um laço de repetição ou loop usando o for logo abaixo.
  //Esse laço apenas escreverá 10 números começando do zero.
  //Observe que foi criado e inicializado uma variável "i" no próprio for.
  
  for(int i=0; i<10;i++){
    print("Esse é o valor de i: %d",i);
  }
}
```
>  Tarefa 01 - Altere o código e execute-o no falcon++ para que ele imprime todos os números entre 20 e 40. Após conseguir, basta copiar as linhas de código e colar aqui e realize o commit.
```C
#include<stdio.h>
int main(){
    for(int i=20; i<41;i++){
      printf("\n Esse e o valor de i: %d",i);
    }

}
```

## Revisando Laços de Repetição: While.
#### Aqui iremos agora focar no laço de repetição While.

>  Usando o While temos uma particularidade. Diferente do for, ele não é finalizado com um valor específico. Ele é finalizado com uma condição. Observe:

```C
int main(){
  // Foi criado uma variável inteira chamada "parada" e inicializada com 0 (zero).
  int parada = 0;
  //Agora vamos impor a condição de que essa variável não pode ser maior que 20. Iremos incrementar ela de 1 a cada interação.
  while (parada <=20){    
    printf("\n O valor da parada agora: %d",parada);
    //na linha abaixo incrementamos de 1 para a próxima interação.
    parada++;
  }  
}
```
>  Tarefa 2 - Altere o código anterior para mostrar a frase "esse é o valor escolhido" quando a variável "parada" for igual a 9. Copie e cole o código aqui e realize o commit.
```C
#include<stdio.h>
int main(){
   int parada = 0;
   while(parada<=20){
      printf("\n O valor da parada agora: %d",parada);
      if(parada ==9){
         printf("\n Esse e o valor escolhido: %d",parada);
      }
      parada++;
   }

}
```

## Revisando Laços de Repetição: Do
#### Agora iremos finalizar nosso último laço de repetição. Iremos usar o do.
>  Usando o do..while temos algo bem legal: iremos colocar a condição de parada apenas no final do código. Observe:
```C
int main(){
  //Criamos a variável inteira incremento aqui para ser lida do teclado. O usuário irá digitar um valor inteiro.
  int incremento = 0;
  // Nas linhas abaixo iremos escrever todo o nosso cardápio vitual.
  do{
    printf("\n############# CARDAPIO VIRTUAL ##############");
    printf("\n[1]-Cafe");
    printf("\n[2]-Almoco");
    printf("\n[3]-Janta");
    printf("\n[99]-Sair do Menu");
    printf("\n#############################################");
    //Aqui mostramos uma frase para o usuário escolher um dos números do cardápio.
    printf("\nEscolha a um numero do cardapio: ");
    //Nesse scanf fazemos a leitura do valor que ele vai digitar.
    scanf("%d",&incremento);
  }while(incremento != 99);// com essa condição, o laço do..while só irá parar quando ele digitar 99.
}
```
>  Tarefa 3 - Altera o código para que quando seja escolhido 1, seja escrito "você escolheu cafe da manhã". Quando 2, seja escrito "você escolheu almoço". Quando 3, seja escrito "você escolheu agora jantar". Copie o código aqui e realize o commit.
 ```C
 #include<stdio.h>
  int main(){
   int incremento = 0;
   do{
       printf("\n############# CARDAPIO VIRTUAL ##############");
       printf("\n[1]-Cafe");
       printf("\n[2]-Almoço");
       printf("\n[3]-Janta");
       printf("\n[99]-Sair do Menu");
       printf("\n#############################################");
       printf("\nEscolha a um numero do cardapio: ");
       scanf("%d",&incremento);
       if(incremento ==1)
           printf("\n Voce escolheu cafe da manha");
       	
       if(incremento ==2)
	   printf("\n Voce escolheu almoço");
	      
       if(incremento ==3)
       	   printf("\n Voce escolheu agora jantar");
          
	}while(incremento !=99);
	
}
```
