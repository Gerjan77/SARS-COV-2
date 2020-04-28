# Definitions

### Defined terms

Words printed in italics, in markdown language seperated by single asterisks or single underscores, 
are defined terms in this file. This file's name is DEFINITIONS.md

### Timestamp
A string of ASCII 0-127 characters. The string length is between 28 and 42. 
It repesents a timestamp with a maximum error of exactitude of 60 seconds.
Concatenated from 6 substrings and separated by spaces as follows:
Month **space** Day1 **space** Year **space** Day2 **space** Time **space** Timezone
Month: 3-9 characters Month can be Januari, Februari, March, April, May, June, July, August, September, October, November, December.
Day1: 3-4 characters Day of the month ending in an appropriate suffix, can be 1st, 2nd, 3rd, 4th, 5th, 6th, 7th, 8th, 
9th, 10th, 11nd, 12th, 13th, 14th, 15th, 16th, 17th, 18th, 19th, 20th, 21st, 22nd, 23rd, 24th, 25th, 26th, 
27th,  28th, 29th, 30th, 31st. 
Year: 4 characters four character representation of a number 0000-9999
Day2: 6-9 characters Day of the week, can be Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday.
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
 
Example: April 26th 2020 Sunday 12:45h UTC

### Available hardware

| Make and type     | Kernel *timestamp*                 | Operating System  |
| ----------------- |:----------------------------------:| -----------------:|
| Apple iPhone 5    |                                    |                   |
| Sony Xperia G3121 | May 11th 2019 Saturday 01:14 JST   |     Android 8.0.0 |
| Asus Zenpad C7.0  |                                    |                   |

### Testing hardware

*Available hardware* with a kernel *timestamp* after Jan 1st 2015 Thursday 00:00h UTC and before April 26th 2020 Sunday 12:45h UTC
with simcard, GPS and bluetooth.