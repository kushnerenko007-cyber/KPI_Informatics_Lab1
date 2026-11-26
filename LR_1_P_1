#include <stdio.h>
#include <stdlib.h>

// Symbol constants (Latin / Translit)
#define Name "Oleksandr"
#define LastName "Kushnerenko"
#define GroupName "ZP-11"
#define Faculty "RTF"
#define University "KPI im. Ihorya Sikorskoho"

int main()
{
    // Variable declarations
    unsigned int semestr;
    float admissionScore;
    int grade1, grade2, grade3, grade4, grade5;
    double averageGrade;
    unsigned int age;

    // Keyboard input
    printf("%s %s, vykonayte nastupni diyi.\n", Name, LastName);
    printf("Vvedit nomer semestru: ");
    scanf("%u", &semestr);
    
    printf("Vvedit sviy vstupniy bal: ");
    scanf("%f", &admissionScore);
    
    printf("Vvedit otsinku za predmet No1: ");
    scanf("%d", &grade1);
    
    printf("Vvedit otsinku za predmet No2: ");
    scanf("%d", &grade2);
    
    printf("Vvedit otsinku za predmet No3: ");
    scanf("%d", &grade3);
    
    printf("Vvedit otsinku za predmet No4: ");
    scanf("%d", &grade4);
    
    printf("Vvedit otsinku za predmet No5: ");
    scanf("%d", &grade5);
    
    printf("Vvedit sviy vik: ");
    scanf("%u", &age);

    // Calculate average grade with explicit double cast
    averageGrade = (double)(grade1 + grade2 + grade3 + grade4 + grade5) / 5.0;

    // Clear console screen
    system("cls");

    // Output with formatting and delimiters
    printf("***************\n");
    printf("===============\n");
    printf("%s\n", University);
    printf("Fakul'tet: %s\n", Faculty);
    printf("Hrupa: %s\n", GroupName);
    printf("------------------------------\n");
    printf("Student: %s %s\n", Name, LastName);
    printf("Vik: %u\n", age);
    printf("Semestr: %u\n", semestr);
    printf("------------------------------\n");
    printf("Vstupniy bal: %.1f\n", admissionScore);
    printf("Seredniy bal: %.2f\n", averageGrade);
    printf("\n");

    return 0;
}
