GDAT
====================

Because I fucking hate GedCom.


Proposed Data Stucture
---------------------

- Event
	+	Id	integer
	+	Dt	date
	+	PlaceId	integer
	+	EventTypeId	integer

- EventPerson
	+	Id	integer
	+   EventId	integer
	+   PersonId	integer

- EventType
	+	Id	integer
	+	Title	string

- Media
	+	Id	integer
	+	MediaTypeId	integer
	+	FileName	string
	+	Source	string
	+	Title	string

- MediaMap
	+	Id	integer
	+	MediaId	integer
	+	Comment	string

- MediaMapEvent
	+	Id	integer
	+	MapId	integer
	+	EventId	integer	

- MediaType
	+	Id	integer
	+	Title	string

- Person
	+	Id	integer
	+	Fname	string
	+	Mname	string
	+	Lname	string
	+	Mother	integer
	+	Father	integer

- PersonAKA
	+	Id	integer
	+	PersonId	integer
	+	AKA	string
	+   AKATypeId

- AKAType
	+	Id	integer
	+	Title	string	

- Place
	+	Id	integer
	+   PlaceName	string
	+	City	string
	+	State	string
	+	Province	string
	+	Region	string
	+	County	string
	+	Country	string
	+	PostalCode	string