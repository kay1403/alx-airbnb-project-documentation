# Backend Requirements – Airbnb Clone

## 1. User Authentication
- Endpoint: POST /api/register/
- Input: email, password, name, role
- Output: JWT token
- Rules: Unique email, password ≥ 8 characters

## 2. Property Management
- Endpoint: POST /api/properties/
- Input: title, description, images, price, availability
- Output: Created property JSON
- Rules: Required title, positive price

## 3. Booking System
- Endpoint: POST /api/bookings/
- Input: property ID, booking dates
- Output: booking confirmation
- Rules: No date conflicts, valid range
- Performance: 95% responses < 2s

## 4. Payments
- Endpoint: POST /api/payments/
- Input: booking ID, payment method
- Output: confirmation + receipt
- Integration: Stripe
