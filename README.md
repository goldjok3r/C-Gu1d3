# C-Gu1d3
Guias y ejercicios de Lenguaje C.


#include <stdio.h> // imput and output
#include <unistd.h> 
#include <limits.h> //limits
#define PI 3.1416f //const - directive
// lineal comment
/* box comment */
void print_types(void) {
    // <stdio.h> // imput and output
    write(1, "c\n", 2);
    printf("Guide.gold\n");
    puts("var-const ----\n");
    
    //var
    int anno = 2020;
    int mes = 5;
    printf("Este es mes: %d del año: %d\n",mes,anno);
    
    //const
    const float pi = 3.14f;
    printf("const pi: %f\n",pi);
    // #define PI 3.1416f //const - directive
    printf("const directive PI: %f\n",PI);
    /*
    char            1   %c
    short           2   %hi %hd
    int             4   %d %i
    unsigned int    4   %u
    long            4   %ld %li
    long long       8   %lld %lli
    float           4   %f %g %e %a 
    double          8   %lf %lg %le %la
    loung double    12  %Lf %Lg %Le %La
    */
    puts("\n");
}

void print_limits(void) {
    // <limits.h> //limits
    puts("limits ----");
    printf("int --> %d - %d\n",INT_MIN, INT_MAX);
    printf("unsigned int --> 0 - %u\n",UINT_MAX);
    printf("\n");
    /*
    () []
    raiz a^x
    / \*
    - +
    */
}

void print_functions(void) {
    int a = 1;
    int b = 2;
    int c = 3;
    
    //block if
    if (a > b) {
        printf("suma %d",(a+b));
    } else {
       printf("resta %d",(b-c));
    }
    if (2 < 5 && a < b) {
        
    } else if (4 >= 3 || b <= c) {
        
    } else if (2 != 4) {
        
    } else {
        printf("Operador ternario");
        //(oper)?exp1:exp2
    }
    
}

int main() {
    // print && outputs functions
    print_types();
    // limits of var
    print_limits();
    
    //print_functions();
    return 0;
}
