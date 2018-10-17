# myBadProgram
#include <iostream>
#include <cmath>

using namespace std;

int main() {
    double x, Eps;
    double A, S = 0; //Текущее слагаемое, сумма
    int K = 0; //номер слагаемого
    double R;
    cout << "Введите x: ";
    cin >> x;
    A = x; //первый элемент при К = 0
    for(int i = 0; i <= 4; i++) {
        //if (abs(A) >= Eps) {
        S = S + A;
        K++;
        R = (K - 2) / pow((x / 3), -4);
        A = A * R;
        cout<<"Сумма: " << S << endl;
        cout << "Колличество учтенных слагаемых: "<< K << endl;
        //}
    }
}
