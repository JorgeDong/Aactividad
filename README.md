#include <stdio.h>
 
int main (void){
  
    char cadena[100]
    char letra;
    int i;
    int desp;

    gets(cadena);
    scanf("%d", &desp);
    
    i=0;
    while (cadena[i] != '\0'){
      letra = cadena[i];
        
        if (letra >= 'a' && letra <= 'z')
        {
            letra = letra + desp;
            if(letra > 'z'){
                letra = letra - 'z' + 'a' - 1;
            }
            cadena[i] = letra;
        }
      i++;
    }
    printf("%s", cadena);
    
    return 0;
}
