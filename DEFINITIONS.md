# Definitions

### Defined terms

Words printed in italics, in markdown language seperated by single asterisks or single underscores, 
are defined terms in this file. This file's name is DEFINITIONS.md

## Medical terms

### R0h

Reproductive number of novel coronavirus. The number of Infections caused by a positive tested homo sapiens (h) before tested positive on the corresponding virus.

### Generalised Contact Class

Generalised Contact Class is a measure of physical contact between two individuals or animals. The class aims to guarantee a distance between two subjects for a set period of time. The class is described in SI units. Physical Barriers etc between two subjects are irrelevant for measuring Contact Class. Example: Generalised Contact Class A.

|Contact Class|Distance(m)        |Period of time(s)        |
|-------------|:------------------|:------------------------|
| A           | 0,75              | 300                     |
| B           | 1,00              | 300                     |
| C           | 1,25              | 300                     |
| D           | 1,50              | 300                     |
| E           | 1,75              | 300                     |
| F           | 2,00              | 300                     |
| G           | 2,25              | 300                     |
| H           | 2,50              | 300                     |
| I           | 2,75              | 300                     |
| J           | 3,00              | 300                     |
| K           | 3,25              | 300                     |
| L           | 3,50              | 300                     |
| M           | 3,75              | 300                     |
| N           | 4,00              | 300                     |
| O           | 4,25              | 300                     |
| P           | 4,50              | 300                     |
| Q           | 4,75              | 300                     |
| R           | 5,00              | 300                     |
| S           | 5,25              | 300                     |
| T           | 5,50              | 300                     |
| U           | 5,75              | 300                     |
| V           | 6,00              | 300                     |
| W           | 6,25              | 300                     |
| X           | 6,50              | 300                     |
| Y           | 6,75              | 300                     |
| Z           | 7,00              | 300                     |

### Contact Class CC[h|m|a]bpks

Contact Class CC[h|m|a]bpks after knowing the following of two subjects:
- h They are both homo sapiens
- m They are both mammals
- a They are both animals
- b Barriers were between them
- p Sexual penetration was done
- k Kissing was done
- s Sneezing was done improperly

Example: Two small mammals in a cage are in Contact Class CCms(A). Two humans sitting on a large bench are in Contact Class CCh(E)

### Sneeze

A sneeze, or sternutation, is a semi-autonomous, convulsive expulsion of air from the lungs through the nose and mouth, usually caused by foreign particles irritating the nasal mucosa. A sneeze expels air forcibly from the mouth and nose in an explosive, spasmodic involuntary action resulting chiefly from irritation of the nasal mucous membrane. This action allows for mucus to escape through the nasal cavity. Sneezing is possibly linked to sudden exposure to bright light, sudden change (fall) in temperature, breeze of cold air, a particularly full stomach, exposure to allergies, or viral infection. Because sneezes can spread disease through infectious aerosol droplets, it is recommended to cover one's mouth and nose with the forearm, the inside of the elbow, a tissue or a handkerchief while sneezing.

The function of sneezing is to expel mucus containing foreign particles or irritants and cleanse the nasal cavity. During a sneeze, the soft palate and palatine uvula depress while the back of the tongue elevates to partially close the passage to the mouth so that air ejected from the lungs may be expelled through the nose. Because the closing of the mouth is partial, a considerable amount of this air is usually also expelled from the mouth. The force and extent of the expulsion of the air through the nose varies. 

## Technical terms

### Timestamp
A string of ASCII 0-127 characters. The string length is between 28 and 42. 
It repesents a timestamp with a maximum error of exactitude of 60 seconds.
Concatenated from 6 substrings and separated by spaces as follows:
Day1 **space** Month **space** Day2 **space** Year **space** Time **space** Timezone

Day1: 6-9 characters Day of the week, can be Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday.

Month: 3-9 characters Month can be Januari, Februari, March, April, May, June, July, August, September, October, November, December.

Day2: 3-4 characters Day of the month ending in an appropriate suffix, can be 1st, 2nd, 3rd, 4th, 5th, 6th, 7th, 8th, 
9th, 10th, 11nd, 12th, 13th, 14th, 15th, 16th, 17th, 18th, 19th, 20th, 21st, 22nd, 23rd, 24th, 25th, 26th, 
27th,  28th, 29th, 30th, 31st. 

Year: 4 characters four character representation of a number 0000-9999

Time: 6 characters Two character representation of the hour 00-23 followed by : 
followed by two character representation of the minute 00-59 followed by h

Timezone: 1-5 characters abbreviation for the timezone.Can be A, ACDT, ACST,	ACT, ACWST, ADT, AEDT, AEST, AET,	AFT, AKDT, 
AKST, ALMT, AMST, AMT, ANAST, ANAT, AQTT, ART, AST, AT, AWDT, AWST, AZOST, AZOT, AZST, AZT, AoE, B, BNT, BOT, BRST, BRT, 
BST, BTT, C,	CAST, CAT, CCT,	CDT, CDT, CEST,	CET, CHADT, CHAST, CHOST, CHOT, CHUT, CIDST, CIST, CKT, CLST, CLT, COT, CST,
CT, CVT, CXT, ChST, D, DAVT, DDUT, E, EASST, EAST, EAT,	ECT, EDT, EEST,	EET, EGST, EGT, EST, ET, F, FET, FJST, FJT, FKST,
FKT, FNT, G, GALT, GAMT, GET, GFT, GILT, GMT, GST, GST, GYT, H, HDT, HKT, HOVST, HOVT, HST, I, ICT, IDT, IOT, IRDT, IRKST,	
IRKT, IRST, IST, JST,	K, KGT,	KOST,	KRAST, KRAT, KST,	KUYT, L, LHDT, LHST, LINT, M, MAGST, MAGT, MART, MAWT, MDT, MHT, MMT,	
MSD,	MSK,		MST,	MT,	MUT,	MVT,	MYT,		N,	NCT,	NDT,		NFDT,		NFT,		NOVST,		NOVT,		NPT,	NRT,	NST,		NUT,	NZDT,		NZST,		O,	
OMSST,	OMST,	ORAT,	P,	PDT,	PET,	PETST,	PETT,	PGT,	PHOT,	PHT,		PKT,		PMDT,	PMST,	PONT,	PST,	PT,	PWT,	PYST,
PYT, Q,	QYZT,	R,	RET,	ROTT,	S,	SAKT,	SAMT,	SAST,		SBT,		SCT,	SGT,		SRET,	SRT,	SST,	SYOT,	T,	TAHT,	TFT,		TJT,	TKT,	TLT,	
TMT,	TOST,	TOT,	TRT,		TVT,	U,	ULAST,		ULAT,	UTC,	UYST,	UYT,	UZT,	V,	VET,		VLAST,	VLAT,	VOST,	VUT,		W,	WAKT,	WARST,	WAST,
WAT,	WEST,			WET,	WFT,	WGST,		WGT,	WIB,	WIT,		WITA,		WST,	WT,		X,	Y,	YAKST,	YAKT,	YAPT,	YEKST,	YEKT,	Z
 
Example: Sunday April 26th 2020 12:45h UTC

### Available hardware

| Make and type and model     | Kernel *timestamp*                        | Operating System  |
| --------------------------- |:-----------------------------------------:| -----------------:|
| Apple iPhone 5c             | Thursday Jun 15th 2017 18:33h PDT         |        iOS 10.3.3 |
| Sony Xperia G3121           | Saturday May 11th 2019 01:14h JST         |     Android 8.0.0 |
| Asus Zenpad C7.0 P01Z       | Monday April 10th 2017 18:49h CST         |     Android 5.0.2 |

### Testing hardware

*Available hardware* with a kernel *timestamp* after Sunday Januari 1st 2017 00:00h UTC and before Sunday April 26th 2020 12:45h UTC with simcard, GPS and bluetooth.

### Compiling platform

Hardware with Operating System MacOS 10.15.4 Supplemental Update 19E287, and with the following third party software installed:
| Third party software                          | 
| --------------------------------------------- |
| Xcode 11.4.1                                  | 
| Command Line Tools for Xcode 11.4.1           | 
| Mono Framework MDK 6.6.0.166                  | 
| Xamarin Visual Studio 8.5.3.16                |                          
| .NET Core SDK 3.1.200                         | 
| .NET Core Runtime 2.1.16                      | 
| OpenJDK 1.8.0.25                              | 
| Xamarin Profiler 1.6.13                       | 
| Xamarin.Android 10.2.0.100                    | 
| Xamarin.iOS 13.16.0.13                        | 
| Xamarin.Mac 6.16.0.13                         | 
|                                               | 

### units

Imagine a square on the smartphone's display. The size of the square is the minimum of two numbers: 1/100 of the display's width and 1/100 of the display's height. A unit is the length of one vertice. It can be expressed in meter, vertical pixels, etc. Example: for a 62 mm x 104 mm display, the unit is 0.62 mm

### IMEI string

Commonly, opening the phone's dialler and typing `*#06#` will display its MEID or IMEI/SV.
Examples: IMEI 49-015420-323751-8 IMEI 357443089796941 IMEI/SV 4756794324562958 IMEI/SV 35-367543-945124-72 MEID a3f804c46de332 MEID a3-f8-04-c4-6d-e3-32
Characters other than 0, 1, 2, 3, 4, 5, 6 , 7, 8, 9, a, b, c , d, e, f, A, B, C, D, E, F are deleted. Spaces are added to create a string of length 16. This is the IMEI string. To display this the font "Calibri" black on white is used and the height of the 0 is at least 3.2 *units*.

### scrollbutton size

The scrollbutton size is 16 *units*

### Tasknumber

Ta where a is a number from 1..10. The tasknumber describes debug App functionality or App functionality

### debug App functionality

A debug app is fully functional if it performs the following tasks:

T1 - have an App startup button named 'SARS-COV-2'

T2 - display the *IMEI string*

T3 - show the GPS location

T4 - connect automatically via bluetooth to another platform running the same app. receive "Length 16d char "

T5 - show a down scroll button, This button reacts to pressing it, by moving all displayed textlabels down.

### App functionality

An app is fully functional if it performs the following tasks:

T6 - Don't log the *IMEI string* of another GSM running this app, if the distance is more than 1,00 meter for 300 seconds.

T7 - Log the *IMEI string* of another GSM running this app, if the distance is less than 0,75 meter for 300 seconds. 

T8 - Stay close to another GSM running this app.  Both press the startup button. Your log is visually and uneditable displayed on the other GSM. The other's log is displayed on your app.

T9 - The log is stored as system file on your platform. The log's storage location and name is randomized. 

T10 - Compare an installation file byte-for-byte with the installer file from your app store. They match exactly.

### Version

The app version shows what it can do 
va.b.c.d  

a : the group of testing hardware. a = 0 refers to the current *testing hardware* and can only increase if more hardware is added. 

b : All *tasknumbers* lower than b or equal to b are tested 'succes' on all *testing hardware* 

c : sequential number for further specified reasons to upgrade 

d : individual number for the developer to separate his or her sequential debug apps

for example, v0.1.0.0 shows an app startup button on iOS 10.3.3, Android 8.0.0, and Android 5.0.2
