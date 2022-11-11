# Method-Exercise
public class ArrayExercise {
    public static void main(String[] args) {
        int[] a = {7, 3, 103, 9, 23,-1, 80};

        System.out.println(nonZero(a));

    }

    static int nonZero(int[] values) {
        int result = 0;

        for (int i = 0; i < values.length; i++) {

            if (values[i] > 0) {
                result = 1;
                // Condition of highest even number greater than highest odd number and even number and highest odd number must be less than 50
                String conditionTwo = (highestEvenNumbers(values) > highestOddNumbers(values)) && (highestEvenNumbers(values) <50) && (highestEvenNumbers(values) < 50) ? "1" :"0";


            } else {
                result = 0;


            }


        }
        return result;

    }

    public static int highestEvenNumbers(int[] values) {

        int highestEven = values[0];
        for (int i = 0; i < values.length; i++) {
            if (values[i] % 2 == 00 && values[i] > highestEven)
                highestEven = values[i];

        }
        return highestEven;


    }

    public static int highestOddNumbers(int[] values) {
        int highestOdd = values[0];

        for (int i = 0; i < values.length; i++) {
            if ((values[i] % 2 != 0) && (values[i] > highestOdd)) {
                highestOdd = values[i];
            }


        }
        System.out.println(highestOdd);
        return highestOdd;
    }
}

