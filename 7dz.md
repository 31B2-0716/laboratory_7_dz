# Домашнее задание №7
#include <stdio.h>
#include <locale.h>
int task1() {
	int year, n;
	printf("Контрольный пример: 2015 год - это год Овцы (Козы) по восточному календарю.\n");
	printf("Введите номер года: ");
	scanf("%d", &year);
	n = (year % 12 + 12) % 12;
	printf("%d год - это год ", year);
	switch (n) {
	case 0:
		printf("Обезьяны");
		break;
	case 1:
		printf("Петуха");
		break;
	case 2:
		printf("Собаки");
		break;
	case 3:
		printf("Свиньи");
		break;
	case 4:
		printf("Крысы");
		break;
	case 5:
		printf("Быка (Коровы)");
		break;
	case 6:
		printf("Тигра");
		break;
	case 7:
		printf("Кролика (Зайца)");
		break;
	case 8:
		printf("Дракона");
		break;
	case 9:
		printf("Змеи");
		break;
	case 10:
		printf("Лошади");
		break;
	case 11:
		printf("Овцы (Козы)");
		break;
	default:
		printf("неизвестного животного");
		break;
	}
	printf(" по восточному календарю.\n");
	return 0;
}
int main() {
	setlocale(LC_ALL, ".UTF-8");
	task1();
}
