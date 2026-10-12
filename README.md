Transform the existing BorrowBack application into a real campus-based borrowing and lending platform specifically designed for PSG Institute of Technology and Applied Research (PSG iTech), Neelambur, Coimbatore.

This must be built as a functional real-world application, not just a visual prototype.

COLLEGE CONFIGURATION

College:
PSG Institute of Technology and Applied Research

Location:
Avinashi Road, Neelambur, Coimbatore – 641062, Tamil Nadu

Official email domain:
@psgitech.ac.in

Only verified PSG iTech students should be allowed to use the student platform.

Use the college identity throughout the application, but do not pretend that the platform is officially endorsed by the college unless an authorized administrator enables that status.

---

1. AUTHENTICATION

Create secure authentication using the PSG iTech college email.

Students should be able to:

- Register using their PSG iTech email
- Verify their email
- Log in
- Log out
- Reset their password
- Create and edit their profile

Only verified "@psgitech.ac.in" accounts should be able to access the student marketplace.

Create role-based access:

STUDENT
ADMIN

Students must never be able to access administrator functions.

---

2. STUDENT PROFILE

Each student profile should contain:

- Name
- Profile picture
- Department
- Year
- College email
- Verification badge
- Rating
- Items listed
- Current borrowings
- Borrowing history
- Lending history

Do not publicly display unnecessary personal information.

---

3. MAIN BORROWBACK HOME PAGE

The main concept should be immediately clear:

"Need something for a while? Borrow it from someone on campus."

Main actions:

[BROWSE ITEMS]

[LIST AN ITEM]

[REQUEST AN ITEM]

Show a simple explanation:

1. Find or request an item
2. Connect with a student
3. Agree on the borrowing terms
4. Borrow
5. Return
6. Review

Do not make the home page crowded.

---

4. BROWSE ITEMS

Students should be able to browse items currently available on campus.

Each item card should show:

- Item image
- Item name
- Category
- Condition
- Free / Paid
- Cost per day if paid
- Available dates
- Lender rating
- Pickup/lending location
- "View Details"

Categories:

- Books
- Calculators
- Electronics
- Lab Equipment
- Engineering Tools
- Stationery
- Sports Equipment
- Project Equipment
- Accessories
- Other

Add:

Search

Category filter

Availability filter

Free / Paid filter

Condition filter

Sort by:

- Recently listed
- Most borrowed
- Highest rated

Do NOT add unnecessary notifications for newly available products.

---

5. LIST AN ITEM

A student should be able to list something they are willing to lend.

Required fields:

Item name

Category

Description

Photos

Condition

Availability

Lending location

Free or Paid

If Paid:
Cost per day

Optional:

- Minimum borrowing period
- Maximum borrowing period
- Additional lending instructions

Example:

Scientific Calculator
Condition: Good
Availability: Available
Type: Paid
Cost: ₹10/day
Location: Library

The lender must be able to change availability later.

---

6. FREE VS PAID BORROWING

Every listing must clearly show:

FREE

or

PAID

If paid, show:

₹XX / day

The lender sets the daily cost when creating the listing.

Calculate the estimated total automatically:

Number of days × Cost per day

For example:

₹10/day × 4 days = ₹40

Do not build an unnecessary online payment system initially.

The platform should clearly state that the payment arrangement is between the users unless an administrator later enables an official payment system.

---

7. REQUEST AN ITEM

This is a major feature.

If a student searches for something and no suitable item is available, they should be able to select:

"Can't find what you need?"

[REQUEST AN ITEM]

The student can enter:

- Item name
- Category
- Description
- Quantity
- Required from date
- Required until date
- Preferred location
- Free / paid preference
- Optional message

Example:

"I need a scientific calculator from 10 October to 14 October for my mathematics lab."

---

8. ITEM REQUEST BOARD

Create a separate section:

"Student Requests"

Students can see active requests from other students.

Example:

REQUESTED

Scientific Calculator

Needed:
10 Oct – 14 Oct

Location:
Library

Posted by:
Verified student

[OFFER TO LEND]

If another student owns the required item, they can select:

"OFFER TO LEND"

The requester should then receive the offer.

The requester can accept or decline the offer.

Once accepted, create a borrowing request/transaction.

---

9. BORROWING REQUEST SYSTEM

For an available listing:

Borrower selects:

[REQUEST TO BORROW]

They specify:

- Start date
- Return date
- Optional message

The lender receives the request.

Lender can:

[ACCEPT]

[DECLINE]

If accepted:

- Reserve the item
- Show the agreed dates
- Show free/paid status
- Show cost per day
- Calculate estimated total
- Move the conversation to the chat section

---

10. PREVENT DOUBLE BOOKING

This is essential.

If an item is already reserved or borrowed during a particular period, another student must not be able to book the same item for overlapping dates.

Show:

"Unavailable from 12 Oct – 15 Oct."

Only allow valid dates.

---

11. CHAT SYSTEM

Create a completely separate "Chats" section.

Students should be able to communicate directly with the lender/borrower after a request is created.

Chat should support:

- Text messages
- Request/transaction reference
- Agreed dates
- Location
- Free/Paid status
- Cost per day
- Estimated total
- Borrowing status

Example chat header:

Scientific Calculator
₹10/day
12 Oct – 15 Oct
Pickup: Library

Keep chat separate from general notifications.

Only allow conversations between users who have a legitimate borrowing/lending interaction or an accepted offer/request.

---

12. LOCATION

Do not force users to choose from predefined locations.

Allow the user to enter/select their preferred meeting or pickup location.

For example:

"Library entrance"

"Block 2 lobby"

"Near Mechanical Department"

"Main Gate"

Use a simple location text field and, if practical, allow campus map/location selection.

Do NOT require students to provide their home address.

---

13. BORROWING LIFECYCLE

Use the following status flow:

REQUESTED
↓
ACCEPTED
↓
RESERVED
↓
BORROWED
↓
RETURN DUE
↓
RETURNED
↓
COMPLETED

For rejected requests:

REQUESTED
↓
DECLINED

For cancelled transactions:

REQUESTED / ACCEPTED
↓
CANCELLED

Clearly display the current status.

---

14. RETURN SYSTEM

When the return date approaches, show a reminder inside the app.

Do not create excessive notifications.

The borrower can select:

"Mark as Returned"

The lender then confirms:

"Confirm Return"

After confirmation:

- Transaction becomes completed
- Item becomes available according to its availability settings
- Users can review each other

---

15. NOTIFICATION POLICY

Keep notifications minimal.

DO NOT notify users every time a new product becomes available.

DO NOT create unnecessary promotional notifications.

Only send important notifications such as:

- Borrow request received
- Borrow request accepted
- Borrow request declined
- Offer received for an item request
- Request/offer accepted
- Important chat message
- Borrowing starts
- Return due soon
- Item overdue
- Return confirmed
- Report/dispute update

Add notification preferences so students can control non-essential notifications.

---

16. DASHBOARD

Create a simple student dashboard.

Show:

My Borrowings

Current items I am borrowing

My Listings

Items I am lending

My Requests

Requests I have made

Item Requests

Requests I have posted

Pending Actions

Requests waiting for my response

Upcoming Returns

Items that need to be returned soon

Recent Chats

Do not overwhelm the dashboard with statistics.

---

17. ADMIN DASHBOARD

Create a separate admin portal.

Admin should be able to:

- View registered users
- View verified users
- Manage reported users
- View listed items
- Remove inappropriate listings
- View borrowing transactions
- View overdue items
- Manage item categories
- Resolve disputes
- Suspend accounts when necessary
- Review platform activity

Admin statistics:

- Total users
- Total listings
- Active borrowings
- Completed borrowings
- Active item requests
- Overdue transactions
- Reported issues

---

18. REPORTING AND SAFETY

Add a simple:

[REPORT]

option for:

- User
- Item
- Inappropriate listing
- Problem with borrowing
- Return dispute

The report should go to the admin dashboard.

Do not expose private user information to other students.

---

19. REVIEWS AND RATINGS

After a completed transaction, allow:

Borrower → Rate lender

Lender → Rate borrower

Rating:

★★★★★

Optional short review.

Display average rating on profiles and item listings.

---

20. DATABASE

Use a real persistent backend.

Create proper collections/tables for:

Users

Items

ItemRequests

BorrowRequests

Transactions

Chats

Messages

Reviews

Notifications

Reports

AdminUsers

Every record should have appropriate IDs, timestamps, ownership information, and status fields.

Do not use hard-coded fake data.

---

21. SECURITY

Implement proper database security rules.

A student should only be able to:

- Edit their own profile
- Edit their own listings
- Create their own requests
- View their own borrowing history
- View chats they are part of
- Send messages in authorized conversations
- Accept/decline requests involving their own listings

Students must not be able to modify another student's transactions, profile, listings, or messages.

---

22. MOBILE DESIGN

Make the application mobile-first.

Bottom navigation:

HOME
BROWSE
REQUEST
CHATS
PROFILE

Use a clean, modern campus-focused design.

Keep buttons large enough for mobile use.

---

23. NO FAKE DATA

This is extremely important.

Do not populate the production version with fake student accounts, fake transactions, or fake reviews.

If sample data is needed during development, clearly separate it into DEVELOPMENT/DEMO mode.

Production mode must use real authenticated PSG iTech users and real database records.

---

24. FINAL USER EXPERIENCE

The application should feel like:

"A trusted sharing network within PSG iTech."

The two main situations should both work:

SITUATION 1:

I need a calculator.

→ Search
→ Find available calculator
→ View price
→ Request
→ Chat
→ Meet at chosen location
→ Borrow
→ Return
→ Review

SITUATION 2:

I need a specific item but nobody has listed it.

→ Search
→ No results
→ Request an Item
→ Other students see the request
→ Someone offers to lend
→ Requester accepts
→ Chat
→ Agree on location and terms
→ Borrow
→ Return
→ Review

Make both workflows extremely simple.

---

25. PRODUCTION REQUIREMENT

The final application must be designed so that PSG iTech can potentially onboard real students.

Do not describe the application as officially owned or endorsed by PSG iTech unless an authorized college administrator has approved it.

Make the architecture scalable so that an authorized administrator can eventually manage the platform.

The final result should be a secure, database-connected, mobile-friendly campus borrowing and lending platform — not merely a frontend demonstration.# share-n-borrow
A student-friendly platform for lending, borrowing, requesting and sharing items within the campus community
