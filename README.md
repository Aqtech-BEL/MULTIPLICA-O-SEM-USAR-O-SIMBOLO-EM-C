
Escreva um program em C que leia dois números inteiros positivos e calcule a 
multiplicação do primeiro pelo segundo.

    #include <stdio.h>
    
    int main() {
        int num1, num2, resultado = 0, i;

    do{
        printf("Digite o primeiro número inteiro positivo: ");
        scanf("%d", &num1);
        printf("Digite o segundo número inteiro positivo: ");
        scanf("%d", &num2);

    }while (num1 <= 0 || num2 <= 0);
        
    
    for (int i = 0; i < num2; i++) {
        resultado += num1; // Soma o num1, num2 vezes
    }

    
    printf("Resultado de %d multiplicado por %d é: %d\n", num1, num2, resultado);

    return 0;
    }

  USANDO O SIMBOLO

    #include <stdio.h>

    int main(){
    
    int num1 , num2, i, mult;
    
    
    do{
        printf("Digite um número positivo: ");
        scanf("%d", &num1);
        
        while(num1 < 0){
            printf("Digite um número positivo: ");
            scanf("%d", &num1);
        }
        
        if(num1 > 0){
            printf("Digite um segundo número positivo: ");
            scanf("%d", &num2);
            
            while(num2 < 0){
                printf("Digite um segundo número positivo: ");
                scanf("%d", &num2);
            }
            
        }
        
    }while(num1 < 0 || num2 < 0);
    
    
    printf("O resultado da multiplicação: %d * %d = %d.", num1, num2, num1 * num2);
    

    return 0;
    }
