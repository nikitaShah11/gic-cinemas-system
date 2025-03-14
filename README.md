# gic-cinemas-system
Introduction
This is a Java console-based prototype for a Cinema Booking System. The system allows users to:

Define a movie title and seating map.
Book tickets with automatic or manual seat selection.
View existing bookings using a booking ID.
Exit the system .
The application follows a structured approach by allocating seats from the farthest row and the center most column to seat allocation

Setup & Execution
Prerequisites
Java 11+
JUnit(jupiter) and Mockito for testing

Run the Application
To run the app please use the following instructions:
- Open the command terminal in the directory of the folder
- java -cp target/classes com.gic.cinemas.GicCinemaSystem

Project Structure
cinema-booking-system/
│── src/
│   ├── com/
│   │   ├── gic/
│   │   │   ├── cinemas/
│   │   │   │   ├── GicCinemaSystem.java  # Main Class
│   │   │   │
│   │   │   │── model/                   # Models
│   │   │   │   ├── Movie.java
│   │   │   │   ├── Seat.java
│   │   │   │   ├── SeatStatus.java
│   │   │   │
│   │   │   │── controller/               # Controllers
│   │   │   │   ├── BookingController.java
│   │   │   │   ├── UserInputHandler.java
│   │   │   │
│   │   │   │── infrastructure/           # Infrastructure
│   │   │   │   ├── GICCinemasFactory.java
│   │   │   │   ├── MovieFactory.java
│   │   │   │
│   │   │   │── repository/                # Repository
│   │   │   │   ├── BookingRepository.java
│   │   │   │
│   │   │   │── service/                   # Services
│   │   │   │   ├── BookingDisplayService.java
│   │   │   │   ├── BookingService.java
│   │   │   │   ├── IBookingService.java
│   │   │   │   ├── SeatAllocationService.java
│   │   │   │   ├── SeatReallocationService.java
│   │   │   │
│   │   │   │── strategy/                  # Strategy Pattern Implementations
│   │   │   │   ├── BestBlockSelectionStrategy.java
│   │   │   │   ├── FarthestRowSelectionStrategy.java
│   │   │   │   ├── MiddleMostSelectionStrategy.java
│   │   │   │   ├── OptimalSeatAllocationStrategy.java
│   │   │   │   ├── SeatAllocationStrategy.java
│   │   │   │
│   │   │   │── ui/                        # User Interface Components
│   │   │   │   ├── BookingMenu.java
│   │   │   │   ├── MainMenu.java
│
│── README.md                               
│── pom.xml                                
