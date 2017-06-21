#include <stdio.h>
int main(void){
int K[4][4],i, j, kat, kit, linha, coluna;

    for(i=0; i<4; i++){
        for(j=0; j<4; j++){
            scanf("%d",&K[i][j]);

        }
    }
        linha=0;
        for(i=0; i<4; i++){
        kat=0;
            for(j=0; j<4; j++){

            kat+= K[i][j];
        }
        if(kat==0)
            linha++;
    }
        coluna=0;
        for(j=0; j<4; j++){
        kat=0;
            for(i=0; i<4; i++){

            kat+=K[i][j];

        }
        if(kat==0)
        coluna++;
    }

        printf("Linhas nulas = %d\n", linha);
        printf("Colunas nulas = %d\n", coluna);
return 0;
}
