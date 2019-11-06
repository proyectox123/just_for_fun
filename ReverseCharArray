public class ReverseCharArray {

    public static void main(String[] args){
        char[] test1 = reverseCharArray(new char[]{});
        char[] test2 = reverseCharArray(new char[]{'a'});
        char[] test3 = reverseCharArray(new char[]{'h', 'e', 'l', 'l', 'o'});
        char[] test4 = reverseCharArray(new char[]{'w', 'o', 'r', 'l', 'd', '!'});
        char[] test5 = reverseCharArray(new char[]{'f', 'a', 'c', 'e', 'b', 'o', 'o', 'k'});

        System.out.println(test1);
        System.out.println(test2);
        System.out.println(test3);
        System.out.println(test4);
        System.out.println(test5);
    }

    private static char[] reverseCharArray(char[] array){
        if(array.length <= 1) return array;

        return reverseCharArrayHelper(array, 0, array.length - 1);
    }

    private static char[] reverseCharArrayHelper(char[] array, int leftIndex, int rightIndex){
        if(leftIndex < rightIndex){
            char temp = array[leftIndex];
            array[leftIndex] = array[rightIndex];
            array[rightIndex] = temp;

            return reverseCharArrayHelper(array, ++leftIndex, --rightIndex);
        }

        return array;
    }
}
