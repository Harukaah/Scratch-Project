git add README.md

สมาชิกกลุ่ม\
    - ไผ่\
    - Fuse\
    - ภูผา\
    - next
    #include <stdio.h>
#include <stdlib.h>

// ฟังก์ชันเปรียบเทียบสำหรับการเรียงลำดับ
int compare(const void *a, const void *b) {
    return (*(int*)a - *(int*)b);
}

int main() {
    int array[] = {5, 2, 8, 1, 3};
    int length = sizeof(array) / sizeof(array[0]);

    printf("อาร์เรย์ก่อนเรียงลำดับ: ");
    for (int i = 0; i < length; i++) {
        printf("%d ", array[i]);
    }

    qsort(array, length, sizeof(int), compare);

    printf("\nอาร์เรย์หลังเรียงลำดับ: ");
    for (int i = 0; i < length; i++) {
        printf("%d ", array[i]);
    }

    return 0;
}
    
