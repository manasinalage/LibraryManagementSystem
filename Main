package Elevatelab;

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
    	
    	int choice;
        Library l= new Library();
        l.addBook(new Book("Java Basics", "James Gosling"));
        l.addBook(new Book("OOP in Java", "Jane Smith"));
        l.addBook(new Book("Effective Java", "Joshua Bloch"));
        l.addBook(new Book("Head First Java", "Kathy Sierra"));
        l.addBook(new Book("Java: The Complete Reference", "Herbert Schildt"));
        l.addBook(new Book("Core Java Volume I", "Cay S. Horstmann"));
        l.addBook(new Book("Clean Code", "Robert C. Martin"));

        
        Scanner sc = new Scanner(System.in);

        
        do{
        	System.out.println("---------Menu----------");
            System.out.println("\n1. View Books\n2. Issue Book\n3. Return Book\n4. Exit");
            choice = sc.nextInt();
            sc.nextLine(); 

            switch (choice) {
                case 1:
                    l.displayBooks();
                    break;
                case 2:
                    System.out.print("Enter book title to issue: ");
                    String issueTitle = sc.nextLine();
                    l.issueBook(issueTitle);
                    break;
                case 3:
                    System.out.print("Enter book title to return: ");
                    String returnTitle = sc.nextLine();
                    l.returnBook(returnTitle);
                    break;
                case 4:
                    System.out.println("Goodbye!");
                    return;
                default:
                    System.out.println("Invalid option.");
            }
        }
        while(choice!=0);
    }
}
