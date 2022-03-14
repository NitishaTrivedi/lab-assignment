package Assignment_2;

// ASSIGNMENT 2 QUESTION 2

//Book Store App Class
public class BookStoreApp {
	public static void main(String[] args) {
		BookStore bs=new BookStore();

		System.out.println("Before selling:");
		bs.display();

		System.out.println("After selling:");
		bs.sell("Book2",5);
		bs.display();

		System.out.println("After Ordering:");
		bs.order("12345",45);
		bs.display();
	}

}

