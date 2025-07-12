# Erik Lebedinski

## Контакты
 - Email: lebedinski.erik@gmail.com
 - Discord: @nineepl
 - Phone number: +48 2137 2137
 - Github: [NineEPL](https://github.com/NineEPL)

## О себе
Меня зовут Эрик. Увлекаюсь игрой на гитаре/бас гитаре. В свободное время решаю алгоритмические задачи на C++. 

## Навыки
 - Blender 3D
 - Python
 - C++

## Примеры кода
```cpp
#include<iostream>
#include<vector>
#include<algorithm>
using namespace std;
int main(){
    ios_base::sync_with_stdio(0); cin.tie(0);
    long long n;
    cin >> n;
    vector<unsigned long long> vec;

    vector<long long> arr(n,0);
    for(long long i = 0; i < n; i++){
        long long c;
        cin >> c;
        vec.push_back(c);
    }
    for(long long i = 0; i < n; i++){

        for(long long j = i+1; j < n; j++){
            long long sum = 0;
            long long gcd_val = __gcd(vec[i],vec[j]);

            while(gcd_val > 0){
                sum += gcd_val%10;
                gcd_val /=10;
            }
            //cout << vec[i]<<" "<<vec[j] << " " <<gcd << " "<<sum<< endl;
            if( sum  %2 == 0){
                arr[i]++;
                arr[j]++;
            }
        }
        //cout << arr[i] << " ";
    }
     for(long long i = 0; i < n; i++){
        cout << arr[i] << " ";
    }
    return 0;
}
```

## Опыт работы
Участвовал в создании сайта [INFORMEJTYCY](https://informejtycy.pl/) в рамках польской олимпиады [Zwolieni z Teorii](https://zwolnienizteorii.pl/).
Полностью создал сайт [MercyRig](https://erikepl.w.staszic.waw.pl/) в рамках школьного проекта.

## Образование
 - XIV LO ogólnokształcące im. Stanisława Staszica w Warszawie
 - RS School, курс Stage 0

## Английский
 - B1/B2