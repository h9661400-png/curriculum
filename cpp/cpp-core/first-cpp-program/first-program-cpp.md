---
author: Stefan-Stojanovic

type: normal

category: must-know
practiceQuestion:
  formats:
    - fill-in-the-gap
  context: standalone
revisionQuestion:
  formats:
    - fill-in-the-gap
  context: standalone
---

# Let's Create Our First Program!

---

## Content

Ready for some code?

It's time to create our first program! 

`"Hello, World!"` is a simple program that prints the text `"Hello, World!"` to the screen. 

In **C++**, you can print text to the screen using the `std::cout` function. Here is an example:
```cpp
#include <iostream>

int main() {
    std::cout << "Hello, World!";
    return 0;
}

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
}```

Let's save that to a script file with the `.cpp` extension.

---

## Practice

C++ code is stored in ??? files

- `.cpp`
- `.c++`
- `.cplus`
- `.csharp`

---

## Revision

C++ code is stored in ??? files

- `.cpp`
- `.c++`
- `.cplus`
- `.csharp`
