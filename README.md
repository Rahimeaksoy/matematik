# matematik
Bu Ödev sayesinde ikinci dereceden bir denklemin koklerinin elle çözüm yapmadan bilgisayar programı yardımıyla nasıl bulabileceğini öğrendim. Diskriminant kavramının programlama mantığıyla nasıl kullanıldığını ve farklı durumlara göre delta küçük sıfır , delta eşit sıfır, delta büyük sıfır koşullu ifadelerle nasıl karar verildiğini kavradım. Ayrıca matematikte öğrendiğim teorik bilgileri algoritmik düşünceyle birleştirerek kod haline getirmenin önemini fark ettim. Fonksiyonun grafik çizimi kısmında ise türevler yardımıyla bir fonksiyonun davranışının nasıl analiz eedildiğini ve bu bilgilerin grafik yorumuna nasıl yansıdığını öğrendim.[Ödev 6.cpp](https://github.com/user-attachments/files/24782011/Odev.6.cpp)
#include <iostream>
#include <cmath>
using namespace std;

int main() {
    int n;
    double toplam = 0.0;

    cout << "n degerini giriniz: ";
    cin >> n;

    for (int k = 1; k <= n; k++) {
        toplam += (k + 1) / pow(3, k);
    }

    cout << "Serinin ilk " << n << " teriminin toplami = " << toplam << endl;

    return 0;
}

[Ödev6.cpp](https://github.com/user-attachments/files/24782160/Odev6.cpp)
#include <iostream>
#include <cmath>
using namespace std;

// Faktoriyel hesaplayan fonksiyon
long long faktoriyel(int x) {
    long long f = 1;
    for (int i = 1; i <= x; i++) {
        f *= i;
    }
    return f;
}

int main() {
    int n;
    double toplam = 0.0;

    cout << "n degerini giriniz: ";
    cin >> n;

    for (int k = 1; k <= n; k++) {
        toplam += pow(5, k) / faktoriyel(2 * k);
    }

    cout << "Serinin ilk " << n << " teriminin toplami = " << toplam << endl;

    return 0;
}

