#include <stdio.h>
#include <stdlib.h>
#include <time.h>
#include <conio.h>

#define N 10

int gera_valores(int x[]);
int somar_pares(int x[],int q);
void imprimir_vetor(int x[]);
int par(int x);

int main(){

    int v_1[N],
        v_2[N],
        v_3[N],
        v_4[N],
        v_5[N];
    int i , soma;

    srand(time(NULL));
	printf("\nPrimeiro vetor:\n\n");
	gera_valores(v_1);
	imprimir_vetor(v_1);

  	printf("\nSegundo vetor:\n\n");
	gera_valores(v_2);
	imprimir_vetor(v_2);

   	printf("\nTerceiro vetor:\n\n");
	gera_valores(v_3);
	imprimir_vetor(v_3);

    	printf("\nQuarto vetor:\n\n");
	gera_valores(v_4);
	imprimir_vetor(v_4);

    	printf("\nQuinto vetor:\n\n");
	gera_valores(v_5);
	imprimir_vetor(v_5);

	printf("\nSoma dos vetores pares:\n\n");
	printf("Soma vetor 1: %d\n\n", somar_pares(v_1,N));
	printf("Soma vetor 2: %d\n\n", somar_pares(v_2,N));
	printf("Soma vetor 3: %d\n\n", somar_pares(v_3,N));
	printf("Soma vetor 4: %d\n\n", somar_pares(v_4,N));
	printf("Soma vetor 5: %d\n\n", somar_pares(v_5,N));


    soma=0;
    soma=somar_pares(v_1,N);
    if(soma<somar_pares(v_2,N)){
        soma=somar_pares(v_2,N);
    }else{
        if(soma<somar_pares(v_3,N)){
            soma=somar_pares(v_3,N);
        }else{
            if(soma<somar_pares(v_3,N)){
                soma=somar_pares(v_3,N);
            }else{
                if(soma<somar_pares(v_4,N)){
                    soma=somar_pares(v_4,N);
                }else{
                    if(soma<somar_pares(v_5,N)){
                        soma=somar_pares(v_5,N);
                     }
                 }
             }
        }
    }

	printf("\nMaior vetor: %d\n",soma);

    return 0;
}

int gera_valores(int x[]){
    int i;
   	 for(i=0;i<N;i++){
        	x[i] = rand()%10;
    }
}
int somar_pares(int x[],int q){
    if(q==0){
        return par(x[0]);
    }else{
        return par(x[q-1]) + par(somar_pares(x,q-1));
    }
}
void imprimir_vetor(int x[]){
	int i;
		for(i=0;i<N;i++){
			printf("[%d]=%d\n", i, x[i]);
	}
}
int par(int x){
    if(x%2==0){
        return x;
    }else{
        return 0;
    }
}




