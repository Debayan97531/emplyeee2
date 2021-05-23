#include<stdio.h>
struct employee {
    int empNO;
    char empName[50];
    char deptName[100];
    int age;
    int phnumber;
    int salary;
} emp[20];

int main() {
    int i;
    printf("Enter information of Employee:\n");

    // storing information
    for (i = 0; i < 20; ++i) {
        emp[i].empNO = i + 1;
        printf("\nFor employee number%d,\n", emp[i].empNO);
        printf("Enter the name of employee: ");
        scanf("%s", emp[i].empName);
        printf("Enter deptName: ");
        scanf("%s", emp[i].deptName);
        printf("enter age: ");
        scanf("%d",&emp[i].age);
        printf("enter phone number: ");
        scanf("%d",&emp[i].phnumber);
         printf("Enter salary: ");
        scanf("%d", &emp[i].salary);
    }
    printf("Displaying Information:\n\n");

    printf("Empno Name dept age phnumber salary \n");
    
    // displaying information
    for (i = 0; i < 20; ++i) {
       printf("%d",emp[i].empNO);
       printf("   %s",emp[i].empName);
       printf("   %s",emp[i].deptName);
       printf("   %d",emp[i].age);
       printf("   %d",emp[i].phnumber);
       printf("   %d",emp[i].salary);
       printf("\n");
    }
    return 0;
}
