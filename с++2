#include <iostream>

// Константа для максимального размера стека
const int MAX_SIZE = 100;

class Stack {
private:
    int arr[MAX_SIZE]; // массив для хранения элементов стека
    int top;           // индекс вершины стека

public:
    // Конструктор: инициализируем вершину стека как -1 (стек пуст)
    Stack() {
        top = -1;
    }

    // Метод для добавления элемента в стек
    void push(int value) {
        if (top >= MAX_SIZE - 1) {
            std::cout << "Stack Overflow! Cannot push " << value << std::endl;
            return;
        }
        arr[++top] = value; // Увеличиваем top и добавляем элемент
        std::cout << "Pushed: " << value << std::endl;
    }

    // Метод для удаления и возврата верхнего элемента
    int pop() {
        if (top < 0) {
            std::cout << "Stack Underflow! Stack is empty." << std::endl;
            return -1; // Возвращаем значение, сигнализирующее об ошибке
        }
        int value = arr[top--]; // Берем элемент и уменьшаем top
        std::cout << "Popped: " << value << std::endl;
        return value;
    }

    // Метод для просмотра верхнего элемента без его удаления
    int peek() {
        if (top < 0) {
            std::cout << "Stack is empty." << std::endl;
            return -1;
        }
        return arr[top];
    }

    // Метод для проверки, пуст ли стек
    bool isEmpty() {
        return (top < 0);
    }
};

int main() {
    Stack myStack;

    std::cout << "Is stack empty? " << (myStack.isEmpty() ? "Yes" : "No") << std::endl;

    myStack.push(10);
    myStack.push(20);
    myStack.push(30);

    std::cout << "Top element is: " << myStack.peek() << std::endl;
    std::cout << "Is stack empty? " << (myStack.isEmpty() ? "Yes" : "No") << std::endl;

    myStack.pop();
    myStack.pop();
    myStack.pop();
    myStack.pop(); // Попытка удалить из пустого стека

    return 0;
}
