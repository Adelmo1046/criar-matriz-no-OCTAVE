# criar-matriz-no-OCTAVE
Como criar uma Matriz
Para criar uma matriz e armazená-la em uma variável de modo que se possa consultála mais tarde, basta digitar os elementos da matriz entre colchetes [ ... ], sendo os elementos de uma mesma linha da matriz separados por vírgula ou espaço e as linhas
separadas por ponto e vírgula. Por exemplo:
>> x=[2,5,8;5,6,7]
x =
2 5 8
5 6 7
>>
Ou
>> x=[2 5 8;5 6 7]
x =
2 5 8
5 6 7
>>
Caso o usuário queira criar uma matriz sem que ela seja mostrada na tela, basta
colocar apenas ’;’ no final, como por exemplo:
>> x=[2,5,8;5,6,7];
>>
Obs: Este procedimento(;) pode ser aplicado em qualquer circunstância.
Estes três casos fornecem o mesmo resultado, que é o de armazenar estes elementos
em forma de matriz (2 linhas por 3 colunas) numa variável cujo nome é ’x’.
Para gerar uma matriz com elementos igualmente espaçados, utiliza-se o seguinte
comando:
11
12 CAPÍTULO 4. MATRIZES E VETORES
>> 0:2:10
ans =
0 2 4 6 8 10
>>
O Octave possui ainda funções para geração de matrizes especiais, tais como:
• eye - matriz identidade
>> I=eye(3)
I =
1 0 0
0 1 0
0 0 1
>>
• ones - matriz cujos todos os elementos são 1
>> Uns=ones(3)
Uns =
1 1 1
1 1 1
1 1 1
>>
• zeros - matriz nula
>> Z=zeros(3)
Z =
0 0 0
0 0 0
0 0 0
>>
• rand - matriz com valores aleatórios
>> Aleat=rand(3)
Aleat =
0.00207 0.59451 0.58122
0.07802 0.25870 0.62960
0.47869 0.01718 0.48988
>>
4.2. COMO DELETAR UMA LINHA OU UMA COLUNA DE UMA MATRIZ 13
4.2 Como deletar uma linha ou uma coluna de uma Matriz
Para deletar alguma linha ou coluna de uma Matriz, deve-se utilizar o seguinte
comando:
C =
2 5 8 4
8 9 7 6
3 15 12 11
>>
>> C(3,:)=[]
C =
2 5 8 4
8 9 7 6
>> C(:,2)=[]
C =
2 8 4
8 7 6
>>
• C(3,:), deleta a linha 3 da Matriz C;
• C(:,2), deleta a coluna 2 da Matriz C resultante
