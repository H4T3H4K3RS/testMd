

# Observer Template
## Designing
The Observer template is a behavioral design pattern that allows an object (subject) to notify other objects (observers) when its state changes. This pattern is often used in GUI applications, where the subject is a GUI element and the observers are graphical elements that need to be updated when the subject changes.

Below is the UML diagram for the Observer template:

![Observer Template UML Diagram](Observer_UML.png)

The UML diagram consists of four components: Subject, Observer, ConcreteSubject, and ConcreteObserver. 

The Subject is an interface that defines methods to attach, detach, and notify observers. 

The Observer is an interface that defines the update method which will be called when the subject changes. 

The ConcreteSubject is a class that implements the Subject interface and stores the state of the subject. 

The ConcreteObserver is a class that implements the Observer interface and contains the logic for updating the observer when the state of the subject changes.

## Implementation

The code for the Observer template is written in Java and consists of four classes: Subject, Observer, ConcreteSubject, and ConcreteObserver.

The Subject interface defines the methods for attaching, detaching, and notifying observers. The code for the Subject interface is given below:

```java
public interface Subject {
  void attach(Observer o);
  void detach(Observer o);
  void notifyObservers();
}
```

The Observer interface defines the method for updating the observer when the state of the subject changes. The code for the Observer interface is given below:

```java
public interface Observer {
  void update();
}
```

The ConcreteSubject class implements the Subject interface and stores the state of the subject. The code for the ConcreteSubject class is given below:

```java
public class ConcreteSubject implements Subject {
  private int state;
  private List<Observer> observers = new ArrayList<Observer>();
  
  public void setState(int state) {
    this.state = state;
    notifyObservers();
  }
  
  public void attach(Observer o) {
    observers.add(o);
  }
  
  public void detach(Observer o) {
    observers.remove(o);
  }
  
  public void notifyObservers() {
    for (Observer o : observers) 
      o.update();
  }
}
```

The ConcreteObserver class implements the Observer interface and contains the logic for updating the observer when the state of the subject changes. The code for the ConcreteObserver class is given below:

```java
public class ConcreteObserver implements Observer {
  public void update() {
    // Update the observer's state here
  }
}
```

## Notification of Traffic Police Posts Project

The project must implement the sending of messages to all traffic police posts.

The project can be implemented using the Observer template. The ConcreteSubject class will represent the traffic police posts and the ConcreteObserver class will represent the message to be sent.

First, the ConcreteSubject class needs to be modified to add a method for sending the messages. The code for the modified ConcreteSubject class is given below:

```java
public class ConcreteSubject implements Subject {
  private int state;
  private List<Observer> observers = new ArrayList<Observer>();
  
  public void setState(int state) {
    this.state = state;
    notifyObservers();
  }
  
  public void attach(Observer o) {
    observers.add(o);
  }
  
  public void detach(Observer o) {
    observers.remove(o);
  }
  
  public void notifyObservers() {
    for (Observer o : observers) 
      o.update();
  }
  
  public void sendMessage(String message) {
    for (Observer o : observers) 
      o.sendMessage(message);
  }
}
```

The ConcreteObserver class also needs to be modified to add a method for sending the messages. The code for the modified ConcreteObserver class is given below:

```java
public class ConcreteObserver implements Observer {
  public void update() {
    // Update the observer's state here
  }
  
  public void sendMessage(String message) {
    // Send the message to the traffic police post
  }
}
```

Finally, the main function needs to be implemented to send the messages to all the traffic police posts. The code for the main function is given below:

```java
public static void main(String[] args) {
  ConcreteSubject subject = new ConcreteSubject();
  ConcreteObserver observer1 = new ConcreteObserver();
  ConcreteObserver observer2 = new ConcreteObserver();
  
  subject.attach(observer1);
  subject.attach(observer2);
  
  subject.sendMessage("Traffic police post notification");
}
```

The above code will send the message “Traffic police post notification” to all the traffic police posts.