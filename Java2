import java.util.ArrayList;

public class SplitArray {

    public static void main(String[] args) {
        // Исходный массив (аналог списка из Python)
        char[] originalArray = {'a', '1', 'b', '2', 'c', '3'};

        // Списки для хранения результатов (аналог list в Python)
        ArrayList<Character> letters = new ArrayList<>(); // для букв
        ArrayList<Character> digits = new ArrayList<>();  // для цифр

        // Проходим по исходному массиву и распределяем элементы
        for (int i = 0; i < originalArray.length; i++) {
            if (i % 2 == 0) { // Если индекс четный (0, 2, 4...) - это буквы
                letters.add(originalArray[i]);
            } else {          // Если индекс нечетный (1, 3, 5...) - это цифры
                digits.add(originalArray[i]);
            }
        }

        // Выводим результат
        System.out.println("Array with letters (even indices): " + letters);
        System.out.println("Array with digits (odd indices): " + digits);
    }
}
