# c-program-using-structure-.

#include <stdio.h>

// Creating a structure to store student information
struct Student {
    char name[50];
    int age;
    char phone[15];
    float marks;
};

int main() {
    struct Student s;

    printf("Enter Student Details:\n");

    printf("Enter Name: ");
    scanf("%49s", s.name);   // reads a single word name

    printf("Enter Age: ");
    scanf("%d", &s.age);

    printf("Enter Phone Number: ");
    scanf("%14s", s.phone);

    printf("Enter Marks: ");
    scanf("%f", &s.marks);

    // Displaying the stored details
    printf("\n===============================\n");
    printf("       STUDENT DETAILS\n");
    printf("===============================\n");
    printf("Name          : %s\n", s.name);
    printf("Age           : %d\n", s.age);
    printf("Phone Number  : %s\n", s.phone);
    printf("Marks         : %.2f\n", s.marks);
    printf("===============================\n");

    return 0;
}
