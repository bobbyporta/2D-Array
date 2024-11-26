import java.util.Scanner;

public class Array2D {
    public static void main(String[] args) {
        
        Scanner scan = new Scanner(System.in);

        int rows;
        System.out.print("Enter the number of rows    : ");
        rows = scan.nextInt();
        
        int columns;
        System.out.print("Enter the number of columns : ");
        columns = scan.nextInt();

        
        int[][] total = new int[rows][columns];
        
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < columns; j++) {
                total[i][j] = i * j;
            }
        }

       
        System.out.println("Multiplication Table:");
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < columns; j++) {
                System.out.print(total[i][j] + "\t"); 
            }
            System.out.println(" "); 
        }
    }
}
