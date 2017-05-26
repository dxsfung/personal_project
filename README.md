# Facility Booking System

## Brainstorming:
The original idea of the project is to build an App for booking of facilities (e.g. a Tennis Court) in a residential estate's clubhouse. Once an MVP is built, the App should be easily adaptable to other similar functions (e.g. booking of rooms, shops, or co-owned properties/facilities).

### Simple User Stories:
* As an Administrator, I would like to create the database of facilities for booking by club members (each record should include the following fields:
  - facility name (e.g. "Tennis Court"),
  - a picture of the facility,
  - facility unit name (e.g. "1" for court 1 and "2" for court 2),
  - date of availability (e.g. "23/05/2017"),
  - time-slots (e.g. "07:00-08:00", "08:00-09:00"),
  - time-slot cost (e.g. "$20" for peak hours, "$15" for non-peak hours),
  - booking status (e.g. "available"/"booked"/"reserved-for-training").
* As an Administrator, each time-slot booking should be associated with a booking member's membership number (user_id).

* As a club member, I would like to see the status of facilities on a day-by-day basis [for the next 7 days]; the time-slot column can have different color-code per time-slot cell to indicate the price of the using that slot.
* As a member, I would like to book the desired time-slot by clicking the cell.
* As a member, I would like to see my list of slots booked and total costs of my bookings.



Based on Calendar example app by RichOnRails.com.  See http://richonrails.com/articles/building-a-basic-calendar-in-ruby-on-rails for details.

Adaptation done:

- gemfile: change sqlite3 to postgresql (switch gem 'sqlite3' to 'pg')
- use `bundle update` instead of `bundle install` (which solved the issue of `gem install json -v '1.8.1'` error)
- replace database.yml with one that uses postgresql
