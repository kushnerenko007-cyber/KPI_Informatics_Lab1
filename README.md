# Звіт з лаболаторної роботи № 1 (Частина 1)
**Дисципліна:** Інформатика. Основи програмування та алгоритми  
**Тема:** Типи даних та потоки введення-виведення  
**Навчальний заклад:** КПІ ім. Ігоря Сікорського  
**Факультет:** Радіотехнічний факультет (РТФ)  
**Група:** ЗП-11  
**Студент:** Кушнеренко Олександр Володимирович  

---

## 1. Мета роботи
Опанувати базові навички роботи з середовищем розробки Code::Blocks, вивчити базові типи даних мови C.
---

## 2. Завдання
Зібрати особисті данні студента, обчислити середній бал.

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
```
## 4. Результати виконання
Під час запуску програми в консольному вікні було послідовно введено номер семестру, вступний бал, оцінки з 5 предметів та вік студента.

Після очищення екрана за допомогою `system("cls")` програма вивела відформатовану підсумкову інформацію:
- Шапку з назвою ВНЗ, факультету та групи з розділювачами `*` та `=`.
- Персональні дані студента.
- Вступний бал із 1 знаком після коми (`%.1f`).
- Обчислений середній бал із 2 знаками після коми (`%.2f`).

*(Сюди ви зможете завантажити або вставити скріншот роботи програми)*  
`![Результати роботи програми](<img width="1105" height="626" alt="image" src="https://github.com/user-attachments/assets/a990998b-fe9a-41de-ab86-5da3dd58c0f0" />
)`

'''

## 5. Висновки
Під час виконання Лабораторної роботи №1 (Частина 1) було:
1. Опановано роботу в інтегрованому середовищі розробки Code::Blocks.
2. Вивчено та застосовано на практиці базові типи даних мови C (`unsigned int`, `float`, `int`, `double`).
3. Засвоєно роботу з потоками введення-виведення `printf()` та `scanf()`, специфікаторами формату та escape-послідовностями.
4. Реалізовано обчислення середнього арифметичного значень із застосуванням явного зведення типів `(double)`.
5. Створено та оформлено репозиторій на GitHub із вихідним кодом і звітом про виконану роботу.
