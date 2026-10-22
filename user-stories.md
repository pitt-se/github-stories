# E1: Room booking
Students can find and reserve study rooms.

## US1: Reserve a room
As a student, I want to reserve a study room so that I have a guaranteed place to work.
FR: FR2, FR5
Priority: Must
MVP: yes

- [ ] The student can pick a room, a date, and a time slot.
- [ ] A booking that overlaps an existing booking is rejected, and the user sees which booking it conflicts with.
- [ ] The confirmed booking appears in the student's list of bookings.

## US2: Cancel a booking
As a student, I want to cancel my booking so that others can use the room.
FR: FR6
Priority: Should
MVP: no

- [ ] The student can cancel a booking up to the start time.
- [ ] A cancelled time slot becomes available to other students immediately.

# E2: Room administration
Staff can manage the rooms that can be booked.

## US3: Add a room
As a staff member, I want to add a room so that students can book it.
FR: FR9
Priority: Must
MVP: yes

- [ ] Staff can enter a room name, building, and capacity.
- [ ] The new room can be booked right away.
