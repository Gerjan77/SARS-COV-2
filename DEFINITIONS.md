# Definitions

### Defined terms

Words printed in italics, in markdown language seperated by single asterisks or single underscores, 
are defined terms in this file. This file's name is DEFINITIONS.md

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

| Make and type and model     | Kernel *timestamp*                 | Operating System  |
| --------------------------- |:----------------------------------:| -----------------:|
| Apple iPhone 5              |                                    |                   |
| Sony Xperia G3121           | Saturday May 11th 2019 01:14h JST  |     Android 8.0.0 |
| Asus Zenpad C7.0 P01Z       | Monday April 10th 2017 18:49h CST  |     Android 5.0.2 |

### Testing hardware

*Available hardware* with a kernel *timestamp* after Thursday Januari 1st 2015 00:00h UTC and before Sunday April 26th 2020 12:45h UTC with simcard, GPS and bluetooth.

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




