# Basic-Railway-Ticket-Booking-System

# 🚆 Train Ticket Booking System (Python + Pandas)

This is a simple **console-based train ticket booking system** built using Python and pandas. It allows users to:
- Check availability of seats in different trains and classes (Sleeper or AC)
- Book tickets if available
- Generate a unique PNR number for each booking
- Show the updated seat availability after booking

---

## 📦 Features

- Store train information in a `pandas` DataFrame
- Real-time seat availability check
- Ticket booking functionality
- Automatic fare calculation
- Random PNR number generation
- Updates to available seats after booking

---

## 🛤️ Trains Available

| Train Name         | Sleeper Seats | AC Seats | Sleeper Price | AC Price |
|--------------------|---------------|----------|----------------|----------|
| Shatabdi Express   | 100           | 50       | ₹500           | ₹1200    |
| Rajdhani Express   | 150           | 75       | ₹700           | ₹1500    |
| Garib Rath         | 200           | 60       | ₹300           | ₹800     |
| Duronto Express    | 120           | 40       | ₹600           | ₹1000    |

---

## 🧪 Sample Output

Tickets booked successfully!
PNR Number: JBPT8PN2QOXJM3RY5J
Total fare: 2400

Tickets booked successfully!
PNR Number: NMZVTXR4GB8OPFH9OP
Total fare: 3500

Updated Train Availability:
Train Sleeper Seats AC Seats Sleeper Price AC Price
0 Shatabdi Express 100 48 500 1200
1 Rajdhani Express 145 75 700 1500
2 Garib Rath 200 60 300 800
3 Duronto Express 120 40 600 1000


---

## 📄 How It Works

### 1. Check Seat Availability
```python
check_availability(train_name, class_type, num_seats)
````

2. Book Tickets

book_tickets(train_name, class_type, num_seats)
Reduces available seats in the selected class

Generates a random 18-character alphanumeric PNR

Calculates and prints the total fare

🧰 Technologies Used
Python 3.x

pandas

random (standard library)

🏁 Getting Started
Requirements:
Python 3.x

pandas library

Run the Code:
Save the script as train_booking.py or open it in a Jupyter notebook.

Run the script or cells in order.

Customize bookings using the book_tickets() function.

📌 Notes
Class type must be either 'Sleeper' or 'AC'

Train name must exactly match one in the list

Booking fails gracefully if invalid inputs or unavailable seats
