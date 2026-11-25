#include <stdio.h>

struct Student {
    int roll_no;
    char name[50];
    int marks[3];
    int total;
    float percentage;
};

int main(void) {
    int n;

    printf("Enter the number of students: ");
    if (scanf("%d", &n) != 1 || n <= 0) {
        return 1;
    }

    struct Student s[n];

    for (int i = 0; i < n; i++) {
        printf("\nEnter the roll number, name and marks of 3 subjects:\n");
        scanf("%d %49s %d %d %d",
              &s[i].roll_no,
              s[i].name,
              &s[i].marks[0],
              &s[i].marks[1],
              &s[i].marks[2]);

        s[i].total = s[i].marks[0] + s[i].marks[1] + s[i].marks[2];
        s[i].percentage = s[i].total / 3.0f;
    }

    printf("\n%-10s %-12s %-12s %-12s %-12s %-8s %-10s\n",
           "Roll No", "Name", "Subject: 1", "Subject: 2", "Subject: 3", "Total", "Percentage");

    for (int i = 0; i < n; i++) {
        printf("%-10d %-12s %-12d %-12d %-12d %-8d %-10.2f\n",
               s[i].roll_no,
               s[i].name,
               s[i].marks[0],
               s[i].marks[1],
               s[i].marks[2],
               s[i].total,
               s[i].percentage);
    }

    return 0;
}
