# Алгоритмы, базовая теория 
## Задание №1 
> Составить алгоритм: если введенное число больше 7, то вывести “Привет”
>> Решение
```Java import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Введите число: ");
        int num = scanner.nextInt();
        if (num > 7) {
            System.out.println("Привет");
        }
    }
}
```


## Задание №2
> Составить алгоритм: если введенное имя совпадает с Вячеслав, то вывести “Привет, Вячеслав”, если нет, то вывести "Нет такого имени"
>> Решение
```Java import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Введите имя:");

        String name = scanner.nextLine();

        if (name.equals("Вячеслав")) {
            System.out.println("Привет, Вячеслав");
        } else {
            System.out.println("Нет такого имени");
        }

        scanner.close();
    }
}
```


## Задание №3 
> Составить алгоритм: на входе есть числовой массив, необходимо вывести элементы массива кратные 3
> > Решение
```Java import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int[] array = {1, 3, 5, 6, 9, 10, 12};
        printMultiplesOfThree(array);
    }
    
    public static void printMultiplesOfThree(int[] arr) {
        for (int num : arr) {
            if (num % 3 == 0) {
                System.out.println(num);
            }
        }
    }
}
```


## Задание №4
> Дана скобочная последовательность: [((())()(())]]
- Можно ли считать эту последовательность правильной?
- Если ответ на предыдущий вопрос “нет”, то что необходимо в ней изменить, чтоб она стала правильной?
> Решение
>> Данная скобочная последовательность "[((())()(())]]" не правильная. Так как в последовательности две закрывающие квадратные скобки и одна квадратная открывающая; и не для каждой пары скобок есть своя открывающая и закрывающая скобка.
Правильная последовательность выглядит так [((())()(()))]










