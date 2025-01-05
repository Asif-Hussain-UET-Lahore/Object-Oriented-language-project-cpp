

### Project Report: Flight Reservation System

#### Overview
The uploaded project is a **Flight Reservation System** implemented in C++. It provides functionalities for managing flights, handling reservations, and booking tickets. The system supports both **International** and **Domestic Flights** with distinct requirements for each.

---

#### Key Features
1. **Flight Management**:
   - Add, remove, update, and search flights (both international and domestic).
   - View all flights categorized as international or domestic.

2. **Reservation Management**:
   - Book tickets for flights, with input validation (e.g., ensuring seat availability).
   - Remove or search for specific reservations.
   - View all reservations categorized as international or domestic.

3. **Passenger Interaction**:
   - A portal for passengers to book, view, or search for their reservations.
   - Ensures passengers provide necessary details like name, age, CNIC, and seat preferences.

4. **File Handling**:
   - Flight and reservation data are stored and managed in text files (e.g., `InternationalFlight.txt`, `DomesticFlight.txt`, `applyticket.txt`, etc.).
   - Dynamic updates to files for adding, removing, and modifying entries.

5. **Access Control**:
   - Password and ID authentication for accessing the **Flight Manager** and **Reservation Manager** interfaces.

6. **Command-Line Menu System**:
   - Interactive menus for accessing different functionalities based on user roles (e.g., flight manager, reservation manager, passenger).

---

#### Classes and Responsibilities
1. **Flight** (Base Class):
   - Manages basic flight details such as flight number, departure/arrival cities, times, dates, and seat availability.

2. **InternationalFlight** (Derived Class):
   - Adds attributes for visa requirements and immigration details.
   - Overrides methods for managing international flight-specific functionality.

3. **DomesticFlight** (Derived Class):
   - Adds attributes for domestic regulations.
   - Handles domestic flight-specific functionality.

4. **FlightManager**:
   - Coordinates operations like adding, removing, and searching flights.
   - Validates flight existence in corresponding files.

5. **Passenger**:
   - Stores and manages passenger details for ticket bookings.

6. **FlightTicket**:
   - Manages ticket issuance and seat assignment for passengers.

7. **Reservation**:
   - Provides interfaces for viewing all flights and reservations.
   - Handles reservation booking for international and domestic flights.

8. **ReservationManager**:
   - Extends reservation management functionality.
   - Facilitates ticket removal and searching for reservations.

---

#### Strengths
- **Object-Oriented Design**: Effective use of inheritance and polymorphism to differentiate international and domestic flight operations.
- **File Handling**: Persistent storage of data ensures the system can retrieve and modify records efficiently.
- **User Role-Based Functionality**: Clear separation of responsibilities for flight managers, reservation managers, and passengers.
- **Validation**: Ensures operations like seat booking check for conflicts.

---

#### Areas for Improvement
1. **Error Handling**:
   - Limited error handling for invalid inputs and file operations.
   - Could benefit from structured exception handling.

2. **Data Storage**:
   - Text files are used for storage, which may not be scalable for larger datasets. Consider transitioning to a database for better performance and query capabilities.

3. **Code Efficiency**:
   - Repeated code for similar functionalities (e.g., adding and searching flights) can be refactored for reusability.

4. **User Interface**:
   - Text-based menus are functional but could be enhanced with a GUI for a better user experience.

---

#### Conclusion
This project provides a solid foundation for a **Flight Reservation System** with comprehensive features for managing flights and reservations. It demonstrates effective use of OOP principles and file handling but could benefit from optimizations in error handling, data storage, and code structure.
