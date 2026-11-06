#include <stdio.h>
#include <locale.h>
#include <math.h>

/* Пример №1: sin(sqrt(x+1)) - sin(sqrt(x-1)) */
double expression_1(double x) {
    if (x < 1.0) {
        printf("Ошибка в Примере 1: x должен быть >= 1 (отрицательный корень)\n");
        return 0.0;
    }
    return sin(sqrt(x + 1.0)) - sin(sqrt(x - 1.0));
}

/* Пример №2: 2^(-x) - cos(x) + sin(2*x*y) */
double expression_2(double x, double y) {
    return pow(2.0, -x) - cos(x) + sin(2.0 * x * y);
}

/* Пример №3: 1/R1 + 1/R2 */
double expression_3(double r1, double r2) {
    if (r1 == 0.0 || r2 == 0.0) {
        printf("Ошибка в Примере 3: R1 и R2 не должны быть равны 0 (деление на ноль)\n");
        return 0.0;
    }
    return (1.0 / r1) + (1.0 / r2);
}

/* Пример №4: ((x + 1) / (x - 1))^3 + 18 * x * y^2 */
double expression_4(double x, double y) {
    if (x == 1.0) {
        printf("Ошибка в Примере 4: x не должен быть равен 1 (деление на ноль)\n");
        return 0.0;
    }
    double fraction = (x + 1.0) / (x - 1.0);
    return pow(fraction, 3.0) + (18.0 * x * y * y);
}

/* Пример №5: (1 + 1/(x^2))^4 - 12 * x^2 * y */
double expression_5(double x, double y) {
    if (x == 0.0) {
        printf("Ошибка в Примере 5: x не должен быть равен 0 (деление на ноль)\n");
        return 0.0;
    }
    double inner_bracket = 1.0 + (1.0 / (x * x));
    return pow(inner_bracket, 4.0) - (12.0 * x * x * y);
}

int main() {
    setlocale(LC_ALL, "Ukrainian");

    double x, y, r1, r2;
    printf("=== Финальная консольная программа вычисления 5 выражений ===\n\n");
    
    /* Ввод данных для Примеров 1, 2, 4 и 5 */
    printf("--- Ввод для Примеров 1, 2, 4 и 5 ---\n");
    printf("Введите значение x: ");
    if (scanf("%lf", &x) != 1) return 1;
    printf("Введите значение y: ");
    if (scanf("%lf", &y) != 1) return 1;

    /* Ввод данных для Примера 3 */
    printf("\n--- Ввод для Примера 3 ---\n");
    printf("Введите значение R1: ");
    if (scanf("%lf", &r1) != 1) return 1;
    printf("Введите значение R2: ");
    if (scanf("%lf", &r2) != 1) return 1;

    printf("\n=== Результаты расчетов ===\n");
    printf("Выражение 1: %f\n", expression_1(x));
    printf("Выражение 2: %f\n", expression_2(x, y));
    printf("Выражение 3: %f\n", expression_3(r1, r2));
    printf("Выражение 4: %f\n", expression_4(x, y));
    printf("Выражение 5: %f\n", expression_5(x, y));

    return 0;
}

