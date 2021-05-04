# task_3.1

public class Main {

    public static void main(String[] args) {

        int numbers[][] = {
                {1,   2,  3},
                {-1, -2, -3},
                {3,   5,  3},
                {5,   5, 10},
        };
        for (int i = 0; i < 4; i++) {
            int minimum = min(numbers [i][0], numbers [i][1], numbers [i][2]);
                System.out.println("Минимальное значение в строке " + (i+1) + " : " + minimum);
        }
    }

    static int min (int a, int b, int c) {
        int array[] = {a, b, c};
        int min = 2147483647;
        for (int i = 0; i < array.length; i++) {
            if (array[i] < min) {
                min = array[i];
            }
        }
        return min;
    }
}
