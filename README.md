Purpose




Current State

public class Person {

    private int id;
    private String firstName;
    private String lastName;
    private String email;
    private String password;
    //List of Events List<Event> @ManyToMany
    //Favorite category EventCategory @OneToMany

    //Methods
    //-getters and setters
    //-get back Favorite Events(returns all events that have to do with favorite category
}


Future Improvements

The Person class might also have the following references:

PersonProfile - a class to gather up all of the profile information about the user
List<Events> eventsAttending - to store events the user wants to attend
List<Events> eventsOwned - a different list, to store the events the user has created
Person would have a many-to-many relationship with Event via List<Events> eventsAttending. It would have a one-to-many relationship with Event via List<Events> eventsOwned.

