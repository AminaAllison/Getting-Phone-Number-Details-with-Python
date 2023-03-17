<h1>Getting Phonenumber Details</h1>

import phonenumbers as ph
<br />
from phonenumbers import carrier, geocoder, timezone
<br />

number = input("Enter phone number with country code: ")
<br />
number = ph.parse(number)
<br />
print(number)
<br />
print(timezone.time_zones_for_number(number))
<br />
print(carrier.name_for_number(number, "en"))
<br />
print(geocoder.description_for_number(number, "en"))
<br />
print("Valid phone number: ", ph.is_valid_number(number))
<br />
