# Recipe of a hotel booking cancellation

# Your thriving hospitality suffers when someone cancels. But what if there were patterns to who cancels when and you could better prepare yourself for it. With this project we will explore this idea, with a dataset containing hotel booking details of hundreds of guests from around the world.

# With some key attributes complied in this dataset with respect to bookings, we try to analyze if they have any influence on cancelation. If there are patterns that help us make better decisions going forward it would always be helpful.

In this exploratory data analysis task, we find what leads to cancellation and answer a few other business questions to increase our revenue.

The Data: Here are the variables you will find in your data file:

•IsCanceled: Categorical Value indicating if the booking was canceled (1) or not (0)

•LeadTime: Integer, Number of days that elapsed between the entering date of the booking into and the arrival date

•StaysInWeekendNights: Integer, Number of weekend nights (Saturday or Sunday) the guest stayed or booked to stay at the hotel

•StaysInWeekNights: Integer, Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel

•Adults: Integer, Number of adults  
•Children: Integer, Number of children 
•Babies: Integer, Number of babies

•Meal: Categorical, Type of meal booked.

Categories are presented in standard hospitality meal packages:  Undefined/SC –no meal package; BB –Bed & Breakfast;
HB –Half board (breakfast and one other meal –usually dinner);
FB –Full board (breakfast, lunch and dinner)

•Country: Categorical, Country of origin. Categories are represented in the ISO 3155–3:2013 format

•MarketSegment: Categorical, Market segment designation. In categories, the term “TA” means “Travel Agents” and “TO” means “Tour Operators”

•IsRepeatedGuest: Categorical, Value indicating if the booking name was from a repeated guest (1) or not (0)

•PreviousCancellations: Integer, Number of previous bookings that were cancelled by the customer prior to the current booking

•PreviousBookingsNotCanceled: Integer, Number of previous bookings not cancelled by the customer prior to the current booking

•ReservedRoomType: Categorical, Code of room type reserved. Code is presented instead of designation for anonymity reasons

•AssignedRoomType: Categorical, Code for the type of room assigned to the booking.
Sometimes the assigned room type differs from the reserved room type due to hotel operation reasons (e.g.overbooking) or by customer request.
Code is presented instead of designation for anonymity reasons
•BookingChanges: Integer, Number of changes/amendments made to the booking from the moment the booking was entered on the PMS until the moment of check-in or cancellation

•DepositType: Categorical, Indication on if the customer made a deposit to guarantee the booking.
This variable can assume three categories: No Deposit –no deposit was made. Non Refund –a deposit was made in the value of the total stay cost. 
Refundable –a deposit was made with a value under the total cost of stay.

•CustomerType: Categorical, Type of booking, assuming one of four categories:  Contract -when the booking has an allotment or other type of contract associated to it; Group –when the booking is associated to a group;
Transient –when the booking is not part of a group or contract, and is not associated to other transient booking;
Transient-party –when the booking is transient, but is associated to at least other transient booking

•RequiredCardParkingSpaces: Integer, Number of car parking spaces required by the customer

•TotalOfSpecialRequests: Integer, Number of special requests made by the customer (e.g.twin bed or high floor)


## For exploratory work:

a.Histograms and boxplots of numeric variables are typically useful.
b.Producingtablesof categorical response variablesisoften helpful.
c.Dividing the data in cancelled and not-cancelled subsets and doing boxplots, using each of othergrouping variablesis often useful.
d.Barplots of cancelationsacross different categories is often useful
Since there is geographic info, you should make some sort of map:
To create a color gradient world map the rworldmap package and the joinCountryData2Map() and mapCountryData() functions might be helpful
It might be helpful to create a new column that is Detractor (it could be Boolean) and try to understand rules for predicting a Detractor.
