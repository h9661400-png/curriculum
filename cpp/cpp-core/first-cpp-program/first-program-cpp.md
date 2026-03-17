#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

int main() {
    srand(time(0));
    int secretNumber = rand() % 100 + 1;
    int guess;
    int attempts = 0;

    cout << "=== GAME DOAN SO ===" << endl;
    cout << "Toi da chon mot so tu 1 den 100." << endl;

    do {
        cout << "Nhap so ban doan: ";
        cin >> guess;
        attempts++;

        if (guess > secretNumber) {
            cout << "So qua lon!\n";
        }
        else if (guess < secretNumber) {
            cout << "So qua nho!\n";
        }
        else {
            cout << "Chuc mung! Ban doan dung sau "
                 << attempts << " lan.\n";
        }

    } while (guess != secretNumber);

    return 0;
}
