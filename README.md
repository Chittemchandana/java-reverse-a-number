# java-reverse-a-number
# Reverse a Number using a while loop in Java
class Main {
  public static void main(String[] args) {

    int num = 1234, reversed = 0;
    
    System.out.println("Original Number: " + num);

    // run loop until num becomes 0
    while(num != 0) {
    
      // get last digit from num
      int digit = num % 10;
      reversed = reversed * 10 + digit;

      // remove the last digit from num
      num /= 10;
    }

    System.out.println("Reversed Number: " + reversed);
  }
}

# Reverse a number using a for loop in Java
class Main {
  public static void main(String[] args) {
    
    int num = 1234567, reversed = 0;

    for(;num != 0; num /= 10) {
      int digit = num % 10;
      reversed = reversed * 10 + digit;
    }

    System.out.println("Reversed Number: " + reversed);
  }
}
