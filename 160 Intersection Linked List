// Create a class named IntersectionLinkedList
public class IntersectionLinkedList {

    // Create a Node class to represent one node of the linked list
    static class Node {

        // Store the value of the node
        int data;

        // Store the reference to the next node
        Node next;

        // Constructor to create a node with a given value
        Node(int data) {

            // Store the given value inside the node
            this.data = data;
        }
    }

    // Method to find the intersection node of two linked lists
    static Node findIntersection(Node headA, Node headB) {

        // Start pointer 'a' at the beginning of List A
        Node a = headA;

        // Start pointer 'b' at the beginning of List B
        Node b = headB;

        // Continue until both pointers point to the same node
        while (a != b) {

            // If pointer 'a' reaches the end of List A
            if (a == null)

                // Move 'a' to the beginning of List B
                a = headB;

                // Otherwise
            else

                // Move 'a' to the next node
                a = a.next;

            // If pointer 'b' reaches the end of List B
            if (b == null)

                // Move 'b' to the beginning of List A
                b = headA;

                // Otherwise
            else

                // Move 'b' to the next node
                b = b.next;
        }

        // Return the node where both pointers meet
        return a;
    }

    // Main method where the program starts
    public static void main(String[] args) {

        // Create the first common node with value 30
        Node common1 = new Node(30);

        // Create the second common node with value 40
        Node common2 = new Node(40);

        // Create the third common node with value 50
        Node common3 = new Node(50);

        // Connect 30 to 40
        common1.next = common2;

        // Connect 40 to 50
        common2.next = common3;

        // Create the first node of List A
        Node headA = new Node(10);

        // Connect 10 to 20
        headA.next = new Node(20);

        // Connect 20 to the common node 30
        headA.next.next = common1;

        // Create the first node of List B
        Node headB = new Node(15);

        // Connect 15 to 25
        headB.next = new Node(25);

        // Connect 25 to the common node 30
        headB.next.next = common1;

        // Find the intersection node
        Node result = findIntersection(headA, headB);

        // Print the value of the intersection node
        System.out.println("Intersection = " + result.data);
    }
}
