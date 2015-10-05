

public class LQueue<T>
	{
		private Node front;
		private Node end;
		public LQueue()
		{
			front = null;
			end = null;
		}
		private class Node
		{
			public T element;
			public Node link = null;
			public void setElement(T x)
			{
				element = x;
			}
			public T getValue()
			{
				return element;
			}
			public void setNext(Node next)
			{
				link = next;
			}
			public Node next()
			{
				return link;
			}
		}
	public static class MyException extends RuntimeException{
		public MyException()
		{
			super();
		}
		public MyException(String message)
		{
			super(message);
		}
	}
		public void enqueue(T x)
		{
			Node last = new Node();
			last.setElement(x);
			if(front == null)
			{
				end = last;
				front = last;
			}
			else 
			{
				end.setNext(last);
				end = last;
			}
	}
		public T dequeue()
		{
			if(this.isEmpty()){
				throw new MyException("There is no item to dequeue");
			}
			T value = front.getValue();
			front = front.next();
			return value;
			
		}
		public boolean isEmpty()
		{
			if(front == null)
			{
				return true;
			}
			return false;
		}

	}
