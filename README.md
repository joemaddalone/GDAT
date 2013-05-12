GDAT
====================

Because I fucking hate GedCom.  It is the EDI to today's JSON.


Proposed Data Stucture
---------------------
Person
	+	Id	integer
	+	Fname	string
	+	Mname	string
	+	Lname	string
	+	Mother	integer
	+	Father	integer
	+	adoptedMother	integer
	+	adoptedFather	integer

PersonBirth
	Id	integer
	Date	date
	PlaceId	integer

PersonMarriage
	Id	integer
	Person1	integer
	Person2	integer
	PlaceId	integer

PersonDeath	
	Id	integer
	Person	integer
	PlaceId	integer
	Date	date

PersonAdoption
	Id	integer
	PersonId	integer
	Mother	integer
	Father	integer
	Date	date

PersonAKA
	Id	integer
	PersonId	integer
	AKAF(irst)	string
	AKAM(iddle)	string
	AKAL(ast)	string
	AKAN(ickname)	string
	
Place
	Id	integer
	City	string
	State	string
	Province	string
	Region	string
	County	string
	Country	string
	PostalCode	string

Media
	Id	integer
	FileName	string
	FileType	integer
	MediaComment	string
	MediaTitle	string

MediaComment
	MediaId	integer
	PersonId	integer
	Comment	string


MediaMap
	Id	integer
	MediaId	integer
	PersonId	integer

Filetype
	Id integer
	Title	string
	Extension	string
