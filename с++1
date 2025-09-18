#include <iostream>
#include <vector>

int main() {
    // Исходный массив (аналог списка из Python)
    char originalArray[] = {'a', '1', 'b', '2', 'c', '3'};
    int length = sizeof(originalArray) / sizeof(originalArray[0]); // Вычисляем длину массива

    // Вектора для хранения результатов (более современный аналог списка в C++)
    std::vector<char> letters; // для букв
    std::vector<char> digits;  // для цифр

    // Проходим по исходному массиву и распределяем элементы
    for (int i = 0; i < length; ++i) {
        if (i % 2 == 0) { // Если индекс четный (0, 2, 4...) - это буквы
            letters.push_back(originalArray[i]);
        } else {          // Если индекс нечетный (1, 3, 5...) - это цифры
            digits.push_back(originalArray[i]);
        }
    }

    // Выводим результат
    std::cout << "Array with letters (even indices): ";
    for (char c : letters) {
        std::cout << c << " ";
    }
    std::cout << std::endl;

    std::cout << "Array with digits (odd indices): ";
    for (char c : digits) {
        std::cout << c << " ";
    }
    std::cout << std::endl;

    return 0;
}
