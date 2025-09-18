import java.util.ArrayList;

// Простой класс Stack, реализованный на основе ArrayList
class ArrayListStack<T> {
    private ArrayList<T> stackList; // ArrayList будет хранить элементы стека

    // Конструктор
    public ArrayListStack() {
        stackList = new ArrayList<>();
    }

    // Метод для добавления элемента в стек
    public void push(T item) {
        stackList.add(item);
        System.out.println("Pushed: " + item);
    }

    // Метод для удаления и возврата верхнего элемента
    public T pop() {
        if (isEmpty()) {
            System.out.println("Stack Underflow! Stack is empty.");
            return null; // Возвращаем null, если стек пуст
        }
        // Удаляем и возвращаем последний элемент ArrayList'а
        T item = stackList.remove(stackList.size() - 1);
        System.out.println("Popped: " + item);
        return item;
    }

    // Метод для просмотра верхнего элемента без его удаления
    public T peek() {
        if (isEmpty()) {
            System.out.println("Stack is empty.");
            return null;
        }
        return stackList.get(stackList.size() - 1);
    }

    // Метод для проверки, пуст ли стек
    public boolean isEmpty() {
        return stackList.isEmpty();
    }

    // Метод для вывода содержимого стека (для наглядности)
    public void display() {
        if (isEmpty()) {
            System.out.println("Stack is empty.");
        } else {
            System.out.println("Stack contents: " + stackList);
        }
    }
}

public class Main {
    public static void main(String[] args) {
        // Создаем стек для целых чисел
        ArrayListStack<Integer> myStack = new ArrayListStack<>();

        System.out.println("Is stack empty? " + (myStack.isEmpty() ? "Yes" : "No"));

        myStack.push(10);
        myStack.push(20);
        myStack.push(30);

        myStack.display(); // Покажем весь стек

        System.out.println("Top element is: " + myStack.peek());
        System.out.println("Is stack empty? " + (myStack.isEmpty() ? "Yes" : "No"));

        myStack.pop();
        myStack.pop();
        myStack.pop();
        myStack.pop(); // Попытка удалить из пустого стека

        myStack.display();
    }
}
