#include <stdio.h>
#include <stdlib.h>

int main()
{
    int ay,yil;
    printf("Lutfen bir ay giriniz: \n");
    scanf("%d",&ay);

    printf("Lutfen bir yil giriniz: \n");
    scanf("%d",&yil);

    while(ay<1){
        printf("Daha buyuk bir ay giriniz: \n");
        scanf("%d",&ay);
    }

    while (ay>12){
        printf("Daha kucuk bir ay giriniz: \n");
        scanf("%d",&ay);
    }

    if(ay==2){
        if(0==yil%4)
            printf("Ay 29 gundur ve Artik yildir.");
        if(0!=yil%4)
            printf("Ay 28 gundur.");
    printf("Mevsim Kistir.");
    }
    if(ay>2 && ay<=5){
        if(0==ay%2)
            printf("Ay 30 gundur.");
        if(0!=ay%2)
            printf("Ay 31 gundur.");
    printf("Mevsim Ilkbahardir.");
    }
    if(ay>5 && ay<=8){
        if(ay==6)
            printf("Ay 30 gundur.");
        if(ay>6)
            printf("Ay 31 gundur.");
    printf("Mevsim Yazdir.");
    }
    if(ay>8 && ay <=11){
        if(0==ay%2)
            printf("Ay 31 gundur.");
        if(0!=ay%2)
            printf("Ay 30 gundur.");
    printf("Mevsim Sonbahardir.");
    }
    if(ay==1){
        printf("Ay 31 gundur.");
    printf("Mevsim Kistir.");
    }
    if(ay==12){
        printf("Ay 31 gundur.");
    printf("Mevsim Kistir.");
    }
    return 0;
}
