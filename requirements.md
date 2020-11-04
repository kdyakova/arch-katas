# Architectural drivers

1. 

# Requirements:
Availability, relability, performance - това идва от point of sales, бройка клиенти, очакваното предоставяне на услугата на други вендори

Scslability за фризерите и за лафките

Elasticity за лафките, щото фризерите работят и нощно време, а лафките не

Security -възнамеряват да събират лична информация, предпочитания и начина на плащане

API / extendability (тоя рекуаърмънр не съм сигурен как му беше научното име) - това идва от 3-party интегразията - първата точка....

## functional requirements
- The customers have to be able to locate the near Farmacy Food location.
- The customers have to be able to see the meals available in a specific location
- The customers have to able to find which meals that are appropriate for them
- The custoemrs should be able to search by meal??
- The system bring the best of knowledge to the forefront and helping customers understand what's extremely important - push messages to customers for health education or other marketing stuff
- the system should be able to gather health information for the custoemr and advice on healty food options
- the system should integrate and aggregate information from the fridges and the coffee shops so that:
  - an administrator/supplier at any time should be able to understand what purchase activity is across all of our nodes
  - an administrator/supplier at any time should be able to understand what inventory is looking like across our entire network
- The system should be accessibel through mobile app and web browser
- The system should have a low-tech version using SMS for not so tech found customers
- the system should have interface for supplyers
- the system should have fidelity or a loyalty program. This includes:
  - objective feedback for the taste
  - in app surveys
  - if a customer fill out their initial profile, we'll give them their first meal free
- the service shoudl be compatible with entity service providers for sign in like Facebook, login, or Gmail

Nice to have:
- the system should be able to advice for children meals too
- the system should monitor and notify for meals left on the shelfs for more then a three days
- the system should monitor and alert for meals left on the shelfs for more then a week
- a subscribed customer can order specific meals using the app and even personalized modified meals picked up from certain location
- the system should have a solution for donations:
  - one customer - donate a chunk of money toward paying for a group of people
  - another custoemr - push notification to say, hey, you've gotten a free meal

- Long term would like to allow multiple vendors to offer items through points of sale
- the system might have integration with smart watches or health trackers in order to track customer health statisctics


## non functional requirements
- The system should easily be expanded to specifically enable dozens of automated fridges and representative run kiosks to essentially handle thousands of customers regardless of where they may be in a geography
- the system should integrate with our third party smart fridge
- the system should integrate with the system in the coffee shops (kiosk??)
- the system should have an easy solution for internaltesting with a set of people(canary release)
- the system shouldn't increace the overall price of one meal - it should be budget friendly
- the system should support upto 1,500 to 2,000 meals a week by the end of 2021 and should be able to increase futher.
- the system should support six to eight locations before the end of the year 2020. this number should increase easyly
- the location will be distrebuted across USA
- in early 2021 of about 1,000 dedicated customers
- 10% of the custoemrs will become subscription customers. 
- the system should be cloud-based


## busyness requiremntes
- HIPAA compliance
- fridge temperature is set by state regulators

# Third party systems:
- smart fridges - Smart Fridges Produce item inventory levels and purchases. The smart fridges have a cloud based management system that handles communication with the Smart Fridge so obtaining this data would be through an API. https://drive.google.com/file/d/1BpwOi-QUy9xG7XaBwXzJ9jd0mdNAvjXa/view 
- kiosk -  a sublet space inside another business where we will sell our product but have an employee to handle the transactions through a point of sale. The same data should be accessible through the POS systems API’s
- QuickBooks
- Cheftec
- Toast - sale system
- Facebook, login, or Gmail for entity service providers for sign in

# System entrypoints
- mobile app
- kiosk
- website
- email
- SMS

# user types
- subscribed user - customer; age 18 to 65; with possible health issues
  - discounted tier - any low-income resident, college student, educator, senior citizen, or betterment
  - non-discounted tier
- non-subscribed user - customer; age 18 to 65; with possible health issues
  - discounted tier - any low-income resident, college student, educator, senior citizen, or betterment
  - non-discounted tier
- supplier
- administrator
