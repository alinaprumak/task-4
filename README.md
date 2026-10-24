# task-4

#include <iostream>
#include <string>
using namespace std;

int main() {
    int n;
    cin >> n;

    for (int i = 1; i <= n; i++) {
        if (i > 1) cout << " ";

        if (i % 3 == 0 && i % 5 == 0)
            cout << "FizzBuzz";
        else if (i % 3 == 0)
            cout << "Fizz";
        else if (i % 5 == 0)
            cout << "Buzz";
        else
            cout << i;
    }

    cout << endl;

    string pershyi, druhyi;
    cin >> pershyi >> druhyi;

    if (pershyi == druhyi) {
        cout << "nichyia" << endl;
    }
    else if (
        (pershyi == "kamin" && druhyi == "nozhytsi") ||
        (pershyi == "nozhytsi" && druhyi == "papir") ||
        (pershyi == "papir" && druhyi == "kamin")
    ) {
        cout << "pershyi" << endl;
    }
    else {
        cout << "druhyi" << endl;
    }

    return 0;
}
