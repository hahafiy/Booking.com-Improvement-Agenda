Functional Requirements :- 
FR1: Real-Time Availability Check
The system shall check room availability in real time whenever a guest opens the extension option and again at the moment the guest confirms the extension to prevent double-booking.
FR2: Stay Extension Request
The system shall allow a guest with an active booking to request an extension of one or more additional nights and shall display the price per extra night and the total cost before the guest confirms.
FR3: Extension Cutoff
The system shall disable the in-app extension option 24 hours before the scheduled check-out time and display a message directing the guest to the front desk.
FR4: Reminder Notifications
The system shall send push notifications based on length of stay for stays longer than 3 days, at 7 days and 3 days interval before check-out. Meanwhile, for shorter stays, at 48 hours before check-out. Each notification shall include a link to the extension option.
FR5: Alternative Suggestions
When the guest’s current room is unavailable for the requested extension, the system shall suggest alternatives, such as a different room type or a nearby date, instead of showing a dead-end error.
FR6: Price and Availability Alerts
The system shall notify the guest if the price or availability changes between viewing and confirming an extension, and shall explain what changed and include every detail on the booking extension.
FR7: Online Check-In
The system shall allow guests to confirm their personal details and estimated arrival time through the app before arrival.
FR8: Early Check-In Request
The system shall allow guests to submit an early check-in request with their expected arrival time, and shall show the request status (pending, approved, or declined) once the hotel responds.
FR9: Extension Confirmation
Once an extension is confirmed, the system shall update the booking details and send the guest a confirmation showing the new check-out date and total price.
Non-Functional Requirements :- 

NFR1: Performance
The system shall return room availability results within 3 seconds under normal network conditions and shall complete the final availability re-check at confirmation within 5 seconds so guests are not left waiting or tempted to retry and submit duplicate requests.
NFR2: Reliability and Data Consistency
The system shall prevent double-booking by treating the confirmation-time availability check as the final authority and shall ensure that a failed or interrupted extension request never results in a guest being charged without an updated booking. If a connection drops mid-request, the system shall show the guest the actual booking status when they reconnect.
NFR3: Usability
The extension flow shall be complete in no more than 3 steps from the notification or booking page and all messages such as sold-out notices, price changes and cutoff messages shall be written in plain language that tells the guest what happened and what they can do next.
NFR4: Security and Privacy
The system shall protect guest personal information and booking details with encryption in transit and at rest and shall require the guest to be logged in to their own account before viewing or changing a booking. Online check-in data such as ID or contact details shall only be accessible to the guest and the relevant hotel.
NFR5: Accessibility and Compatibility
The app shall support both IOS and Android following common accessibility guidelines and remain usable on slower mobile connections
NFR6: Notification Dependability
Reminder notifications shall be delivered within 5 minutes of their scheduled time and the guest shall be able to view or turn off reminders in their notification settings so they stay helpful rather than annoying.
