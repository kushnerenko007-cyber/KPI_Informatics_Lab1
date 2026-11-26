# Лабораторна робота № 1 (Частина 1)
**Дисципліна:** Інформатика. Основи програмування та алгоритми  
**Тема:** Типи даних та потоки введення-виведення  
**Навчальний заклад:** КПІ ім. Ігоря Сікорського  
**Факультет:** Радіотехнічний факультет (РТФ)  
**Група:** ЗП-11  
**Студент:** Кушнеренко Олександр Володимирович  

---

## 1. Мета роботи
Опанувати базові навички роботи з середовищем розробки Code::Blocks, вивчити базові типи даних мови C (`unsigned int`, `float`, `int`, `double`), розібратися з потоками введення-виведення (`printf`, `scanf`), оголошенням символьних констант за допомогою `#define` та явним зведенням типів.

---

## 2. Завдання
1. Оголосити константні символьні рядки (`#define`) з інформацією про ВНЗ, факультет, групу та студента.
2. Реалізувати введення з клавіатури номеру семестру, вступного балу, 5 оцінок за предмети та віку.
3. Розрахувати середній бал для 5 предметів з явним перетворенням типів до `double`.
4. Реалізувати очищення екрана консолі за допомогою `system("cls")`.
5. Оформити виведення з розділювальними рядками зі 15 символів `*` та `=`.
6. Налаштувати форматоване виведення: вступний бал — з 1 знаком після коми (`%.1f`), середній бал — з 2 знаками (`%.2f`).

---

## 3. Вихідний код програми (`main.c`)

```c
#include <stdio.h>
#include <stdlib.h>

// Symbol constants
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

    // Calculate average grade with explicit cast
    averageGrade = (double)(grade1 + grade2 + grade3 + grade4 + grade5) / 5.0;

    // Clear console
    system("cls");

    // Output results
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

---

## 4. Результати виконання <img width="1112" height="626" alt="image" src="https://github.com/user-attachments/assets/3c9470fa-2ad4-4403-ba9a-cb8b541042a6" />
## 5. Висновки
Під час виконання лабораторної роботи №1
 (Частина 1) було здобуто практичні навички
 роботи у IDE Code::Blocks, засвоєно роботу зі
 специфікаторами формату функції printf(), потоком введення scanf(),
а також опрацьовано правильність обчислення дійсних значень за допомогою явного зведення типів (double).
