import java.util.*;
import java.lang.*;
import java.io.*;

class Codechef
{
    public static void main(String[] args) throws java.lang.Exception
    {
        LinkedList LL = new LinkedList();
        LL.disp();
        LL.atend(12);
        LL.atend(13);
        LL.disp();
        LL.afterx(15, 2);
        LL.disp();
        LL.delete(2);
        LL.disp();

    }
    static class Node {
        int data;
        Node next;

        Node(int data) {
            this.data = data;
            this.next = null;
        }
    }
    static class LinkedList {
        Node head;

        LinkedList() {
            head = new Node(10);
            Node secondNode = new Node(11);
            head.next = secondNode;
            Node third = new Node(17);
            secondNode.next = third;
        }

        void disp() {
            Node temp = head;
            while (temp != null) {
                System.out.print(temp.data + " --> ");
                temp = temp.next;
            }
            System.out.println("null");
        }

        void atend(int data) {
            Node newnode = new Node(data);
            Node temp = head;
            while (temp.next != null) {
                temp = temp.next;
            }
            temp.next = newnode;
        }
        void afterx(int data, int n) {
            Node temp = head;
            int count = 0;
            Node newnode = new Node(data);
            while (temp.next != null) {
                temp = temp.next;
                count++;
                if (count == n) {
                    Node after = temp.next;
                    temp.next = newnode;
                    newnode.next = after;
                    break;
                }
            }

        }

        void delete(int n) {
            if (head == null) {
                System.out.println("List is empty");
                return;
            }
            if (n == 1) {
                head = head.next;
                return;
            }

            Node temp = head;
            int count = 1;
            while (temp != null && count < n - 1) {
                temp = temp.next;
                count++;
            }

            if (temp == null || temp.next == null) {
                System.out.println("Position " + n + " does not exist.");
                return;
            }
            temp.next = temp.next.next;
        }

    }

}
