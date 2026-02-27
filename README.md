# quest-es-Girotto-C
PRIMEIRA QUEST
#include <stdio.h>

#define PI 3.14159  // Definição da constante PI

int main() {
    double raio = 0.0;
    double area = 0.0;
    double circunferencia = 0.0;

    printf("=== CALCULO DE ADESIVO CIRCULAR ===\n");
    printf("Informe o valor do raio: ");

    // Verifica se o valor digitado é válido
    if (scanf("%lf", &raio) != 1 || raio <= 0) {
        printf("Erro: valor de raio invalido.\n");
        return 1;
    }

    // Cálculos
    area = PI * raio * raio;
    circunferencia = 2 * PI * raio;

    // Resultados
    printf("\n--- RESULTADOS ---\n");
    printf("Area necessaria: %.2lf\n", area);
    printf("Comprimento da borda: %.2lf\n", circunferencia);

    return 0;
}
SEGUNDA QUEST:
#include <stdio.h>
#include <math.h>
	int main(){
		double L, perimetro, area, diagonal;
		
		printf("Digite o lado da placa quadrada:");
		scanf("%lf", &L);
	
		perimetro = 4 * L;
		area = L * L;
		diagonal = L * sqrt(2.0);
	   //sqrt é para raiz quadrada!
	   	printf("Total das bordas (perimetro): %.4f\n", perimetro);
   	    printf("Area para verniz: %.4f\n", area);
  	    printf("Diagonal (canto a canto): %.4f\n", diagonal);
		return 0;
	}
  TERCEIRA QUEST:
  #include <stdio.h>

int main(){
    double A, B;
    double C, D;

    printf("Digite a leitura do sensor A: ");
    scanf("%lf", &A);
    printf("Digite a leitura do sensor B: ");
    scanf("%lf", &B);

    C = (A - B) * (A - B);   
    D = (A * A) - (B * B);   
    printf("\nIndicador C (A - B)^2 = %.6lf\n", C);
    printf("Indicador D (A^2 - B^2) = %.6lf\n", D);

    return 0;
}
