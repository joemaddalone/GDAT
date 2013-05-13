GDAT
====================

Because I fucking hate GedCom.


Proposed Data Stucture
---------------------

- Event
	+	Id	int
	+	Dt	date
	+	PlaceId	int
	+	EventTypeId	int

- EventPerson
	+	Id	int
	+	EventId	int
	+	PersonId	int
	
- EventType
	+	Id	int
	+	Title	varchar

- Media
	+	Id	int
	+	MediaTypeId	int
	+	FileName	varchar
	+	Source	varchar
	+	Comment	varchar

- MediaMap
	+	Id	int
	+	MediaId	int
	+	EventId	int
	+	Comment	varchar

- MediaType
	+	Id	int
	+	Title	varchar

- Person
	+	Id	int
	+	Fname	varchar
	+	Lname	varchar
	+	Mname	varchar
	+	Mother	int
	+	Father	int

- PersonAKA
	+	Id	int
	+	PersonId	int
	+	AKA	varchar
	+	AKATypeId	int

- PersonAKAType
	+	Id	int
	+	Title	varchar

- Place
	+	Id	int
	+	City	varchar
	+	State	varchar
	+	Province	varchar
	+	Region	varchar
	+	County	varchar
	+	Country	varchar
	+	PostalCode	varchar
	+	PlaceName	varchar
	+	Longitude	decimal
	+	Latitude	decimal