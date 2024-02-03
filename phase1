package orderEntryPhase1;

import java.util.Scanner;

public class OrderEntryPhase1 {
    // instance variables
    private String itemNumber;
    private String itemDescription;
    private double itemPrice;
    private int itemQuantity;
    private double totalTax;
    private double itemDiscount;

    private void getData() {
        // Declare Scanner object to get console data
        Scanner input = new Scanner(System.in);

        System.out.print("Enter item number: ");
        itemNumber = input.nextLine();

        System.out.print("Enter item Description: ");
        itemDescription = input.nextLine();

        System.out.print("Enter item price: $");
        itemPrice = input.nextDouble();

        System.out.print("Enter Quantity Ordered: ");
        itemQuantity = input.nextInt();

        System.out.print("Enter item tax: $");
        totalTax = input.nextDouble();

        System.out.print("Enter item discount: $");
        itemDiscount = input.nextDouble();
    }

    public String toString() {
        return ("\nOrder Details: " +
                "\nItem Number Item Description Item Price Quantity Ordered Tax Amount Discount Amount \n" +
                " " + itemNumber +
                "\t   " + itemDescription +
                "\t\t$" + itemPrice +
                "\t   " + itemQuantity +
                "\t\t  $" + totalTax +
                "\t\t  $" + itemDiscount);
    }

    public double addIntDouble(double itemPrice, double totalTax, double itemDiscount) {
        return itemPrice + totalTax + itemDiscount;
    }

    public double multiplyIntDouble(double itemPrice, int itemQuantity) {
        return itemPrice * itemQuantity;
    }

    public static void main(String[] args) {
        // Create new order
        OrderEntryPhase1 myOrder = new OrderEntryPhase1();

        // Get data for order
        myOrder.getData();

        // Display order details
        System.out.println(myOrder.toString());

        // Call the addIntDouble method
        double addResult = myOrder.addIntDouble(myOrder.itemPrice, myOrder.totalTax, myOrder.itemDiscount);
        System.out.println("itemTotal: " + addResult);

        // Call the multiplyIntDouble method
        double multiplyResult = myOrder.multiplyIntDouble(myOrder.itemPrice, myOrder.itemQuantity);
        System.out.println("itemSubtotal: " + multiplyResult);
    }
}
