Questões Objetivas
1. B
2. B
3. D
4. D
5. B
6. B

Questões Discursivas

7. 

Início

    var Idade = LerEntradaDoUsuário "Insira sua Idade aqui:"

        Se: Idade < 16 anos 
         Então: mostrar:  Você não pode votar!
        
        Se não: Idade < 18
         Então: mostrar: Seu voto é facultativo!
        
        Todas as idades restantes:
         Então: mostrar: Seu voto é obrigatório!
        
Fim

8. 

Início

    classe FormaGeometrica
        Atributos: cor
        Construtor: cor
        atributoCor = Cor
        

    classe retangulo extende FormaGeometrica:
        Atributos: cor, largura e comprimento
        Importa de FormaGeometrica: AtributoCor
        this.largura = largura
        this.comprimento = comprimento
    
        Metodo cacularAreaRetangulo. Atrbutos: largura, comprimento
            Atributo: arearetangulo = AtributoLargura x AtributoComprimento
            retorna areaRetangulo
        
    
    classe circulo extende FormaGeometrica
        Atributos: raio e cor
        construtor: cor e raio
        Herdando de FormaGeometrica o AtributoCor
        this.raio = raio
        
        Método calcularAreaCirculo: Atributos: raio
            areaCirculo = raio^2*3.14
            retorna areaCirculo

Fim

9. 

Início

    trajetoTotal = 5000 metros
    tempoMáximo = 10 minutos = 600 segundos 
    aceleração = 2 m/s
    velocidadeMáxima = 20 m/s
    velocidadeInicial = 5 m/s
    velocidade = 0

    Método acelerar:
        Enquanto: velocidade < velocidadeMáxima
            velocidade = velocidadeInicial + aceleração*tempo

    Método calcularTempoTotalDeViagem:

        trajetoTotal/velocidade = tempoDeViagem

        5000 m/20 m/s = 250 segundos = 4 minutos e 10 segundos 

Fim

10. 

Início

    Função TransporMatriz(matriz)

        #Para facilitar a multiplicação de matrizes, vou transfromar colunas em linhas, subtituindo as antigas listas

        #Primeiro, se verifica se a matriz é 3x3

        Se tamanho(matriz) = 3 E tamanho(matriz[0]) = 3 E Matriz = 
        
        [ [matriz[0][0], matriz[0][1], matriz[0][2]],  
        
        [matriz[1][0], matriz[1][1], matriz[1][2]], 
        
        [matriz[2][0], matriz[2][1], matriz[2][2]] ]  


            Então:

            Matriz = 
            
            [ [ matriz[0][0], matriz[1][0], matriz[2][0] ],  
            
            [ matriz[0][1], matriz[1][1], matriz[2][1] ], 
            
            [ matriz[0][2], matriz[1][2], matriz[2][2] ] ]  


    Função CriarNovaMatriz(matriz01, matriz02)

        Para i de 0 até 2
            
            Faça: 
            
            NovaMatriz = 
        
        [ [matriz[0][0], matriz[0][1], matriz[0][2]],  
        
        [matriz[1][0], matriz[1][1], matriz[1][2]], 
        
        [matriz[2][0], matriz[2][1], matriz[2][2]] ]  

            NovaMatriz[i][0] = matriz01[i][0]*matriz02[0][0] + matriz01[i][1]*matriz02[0][1] + matriz01[i][2]*matriz02[0][2]
            NovaMatriz[i][1] = matriz01[i][0]*matriz02[1][0] + matriz01[i][1]*matriz02[1][1] + matriz01[i][2]*matriz02[1][2]
            NovaMatriz[i][2] = matriz01[i][0]*matriz02[2][0] + matriz01[i][1]*matriz02[2][1] + matriz01[i][2]*matriz02[2][2]

            Imprima: NovaMatriz


    Função MultiplicaçãoDeMatrizes(matriz01, matriz02):

        # Verifica se a primeira matrize têm o mesmo número de colunas e que o número de linhas da segunda

        Se tamanho(matriz01) ≠ tamanho(matriz02[0]) então:
            Retornar "As matrizes não podem ser multiplicadas."

        Senão:

        Chamar Função TransporMatriz(matriz01)

        Chamar Função CriarNovaMatriz(matriz01,matriz02)

    matrizA = [[1,4,3], [2,3,1], [3,7,9]];
    matrizB = [[3,2,1], [5,4,8], [2,5,1]];

    MultiplicaçãoDeMatrizes(matrizA, MatrizB)

Fim