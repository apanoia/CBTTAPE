
## $$README.txt
```

ASSEMBLE THIS USING THE SOURCE LIBRARY AS THE FIRST MEMBER OF THE
CONCATENATED SYSLIB DATASET.  YOU'LL ALSO NEED SYS1.MACLIB, AND
POSSIBLY MODGEN.  USE THE BATCH OPTION; THERE ARE SEVERAL SEPARATE
SOURCE DECKS STACKED.

DO NOT LINK WITH SPECIAL OPTIONS.  THIS PROGRAM IS NOT REENTRANT,
REUSABLE OR REFRESHABLE.  ALLOW THE BINDER TO ASSIGN THE RMODE/AMODE
ATTRIBUTES BY DEFAULT, ACCORDING TO THE CSECT FLAGS.

THE MODLIST PROGRAM WAS DEVELOPED AS A STOP-GAP MEASURE, TO TRY AND
KEEP A HANDLE ON OUR OS/VS COBOL TO COBOL II CONVERSION PROJECT.
THE ONLY KNOWN BUG LEFT IS IN DEALING WITH MODULES THAT MAY LOAD
ABOVE THE 16M LINE.  SOMETIMES THEY WORK OK; SOMETIMES NOT.

THE OUTPUT FOR EACH LMOD STARTS WITH A LINE OF HYPHENS.  THE FIRST
LINE BELOW THAT DETAILS THE LMOD INFO, INCLUDING SOME LKED
ATTRIBUTES.  BELOW THAT ARE LINES FOR EACH CSECT IN THE LMOD, MARKED
BY CS-(NAME) FOR EACH CSECT.  WHERE POSSIBLE, COBOL COMPILER OPTIONS
THAT WERE IN EFFECT FOR THE CSECT ARE DETAILED.  THE VARIOUS
COMPILERS THAT ARE NOW RECOGNIZED ARE ANS4, OS/VS (LISTED AS VSR1)
AND COBOL II (LISTED AS C2)

THE PAN STAMP IS AN IN-HOUSE REQUIREMENT, SO THAT WE CAN MATCH
SOURCE WITH LMOD CODE.  SINCE SOMEONE ELSE MIGHT BE USING THE SAME
MECHANISM, I'VE LEFT THAT CODE INTACT.

THIS IS A REPORT PROGRAM ONLY AND THEREFORE NEEDS ONLY READ ACCESS
TO ANY LOADLIB IT PROCESSES.

USE AS YOU SEE FIT; BUT I'D APPRECIATE HAVING ANY MODS SENT BACK TO
ME, TO INCORPORATE IN LATER VERSIONS AS NEEDED.

MY FULL IDENTIFICATION, AND E-MAIL ADDRESS, ARE IN THE COMMENTS AT
THE BEGINNING OF THE SOURCE CODE.
```
