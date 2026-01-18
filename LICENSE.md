#include<stdio.h>
int main()
{
 	int x, N, m, i = 0, flag = 0;
 	scanf_s("%d %d", &x, &N);

 	do {
 		scanf_s("%d", &m);
 		i++;
 		if (m < x) {
 			printf("Too small\n");
 		}
 		if (m > x) {
 			printf("Too big\n");
 		}
 		if (m == x) {
 			flag = 1;
 			switch (i) {
 			case 1:printf("Bingo!\n");
 			case 2:printf("Lucky You!\n");
 			case 3:printf("Lucky You!\n");
 			default:printf("Good Guess!\n");
 
 			}
 		}
 		if (i > N) { printf("Game Over"); }
 	} while (m>0);
 	if (flag == 0) {
 		printf("Game Over");
 	}
 	return 0;
}
#include<stdio.h>
int main()
{
 	int x, N, m, i = 0;
 	scanf("%d %d", &x, &N);
 	int flag = 0;

 	do {
 		scanf("%d", &m);
 		i++;
 		if (i <= N && flag == 0) {
 			if (m > x) {
 				printf("Too big\n");
 			}
 			if (m < x&&m>0) {
 				printf("Too small\n");
 			}
 			if (m == x) {
 				flag = 1;
 				switch (i) {
 				case 1:printf("Bingo!\n"); break;
 				case 2:printf("Lucky You!\n"); break;
 				case 3:printf("Lucky You!\n"); break;
 				default:printf("Good Guess!\n"); break;
 				}
 			}
 		}if (i > N && flag == 0) {
 			flag = 2;
 			printf("Game Over\n");
 		}
 	} while (m >= 0);
 	if (flag == 0) {
 		printf("Game Over\n");
 	}
 	return 0;
}
注意这个循环怎么用！！！！！
