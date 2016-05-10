ls -sh1 *sv

6.0M detroit-311.csv
152M detroit-blight-violations.csv
 27M detroit-crime.csv
4.3M detroit-demolition-permits.tsv

calls        19680   2014-07-14  2015-10-15
violations  307801   2004-03-16  2015-08-03
crimes      119931   2015-01-01  2015-12-10
permits       7133   2010-05-20  2015-08-28

detroit-blight-violations.csv
-----------------------------
ViolationStreetNumber,
ViolationStreetName,
MailingStreetNumber,
MailingStreetName,
MailingCity,
MailingState,
MailingZipCode,
...,
ViolationCategory=numeric: zero in many cases,
ViolationAddress="ViolationStreetNumber ViolationStreetName\nDetroit, MI\n(lat,lon)",
MailingAddress="MailingStreetNumber MailingStreetName\nMailingCity, MailingState MailingZipCode\n(lat,lon)"


detroit-311.csv
---------------
issue_type="short text", address, lat, lng, location = "(lat, lng)"


detroit-crime.csv
-----------------
Capital letters mostly
CATEGORY="short text" (larceny=Diebstahl),
OFFENSEDESCRIPTION="longer text",
ADDRESS, LON, LAT, LOCATION="Street in ADRESS\nNumber in ADDRESS\n(LAT, LON)"


detroit-demolition-permits.tsv
------------------------------
SITE_ADDRESS="StreetNumber Streetname"
CASE_TYPE="Three letter code",
CASE_DESCRIPTION=string,
site_location="StreetNumber StreetName\nCity, State\n(lat,lon) or EMPTY!!",
owner_location="StreetNumber StreetName\nCity, State\n(lat,lon) or EMPTY!!",
contractor_location="StreetNumber StreetName\nCity, State\n(lat,lon) or EMPTY!!",
geom="(lat,lon)" #  almost all EMPTY!!"
