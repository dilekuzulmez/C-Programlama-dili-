#include <stdio.h>
#include <stdlib.h>


int main()
{
    int x,y,z,sayac;
    float ortalama,fonksiyon,toplam;
    toplam=0;
    sayac=1;

    for(x=-3;x<=3;x++){
        for(y=-3;y<=3;y++){
            if(x*x==y*y)continue;
            for(z=-3;z<=3;z++){
                fonksiyon=(-(x*x)+(2*y*z*z)-(3*x*y*z))/((x*x)-(y*y));
            printf("Olasi butun degerler:%f'dir.\n",fonksiyon);
                toplam=toplam+fonksiyon;
                sayac=sayac+1;
        }

      }
    }
    ortalama=toplam/sayac;
    printf("Toplam: %.2f'dir.\n",toplam);
    printf("Ortalama: %.2f'dir.\n",ortalama);

    return 0;
}
