
## $$DOC.txt
```
MEMBERS WTOETPS1 AND WTOETPS2 ARE MODIFICATIONS OF THE COCA-COLA WTO
  EXITS.  THESE EXITS WILL WRITE AN SMF RECORD FOR EACH MOUNT AND DISMOUNT
  IN ADDITION TO THE DISPLAY OF WHERE A TAPE WAS IF IT WAS RECENTLY
  MOUNTED.  MODIFICATIONS HAVE ALSO BEEN MADE TO CREATE A USER CVT WHICH
  WAS NEEDED BY THE EXITS.

MEMBER WTOTAPMT MAY BE USED TO WRITE AN SMF RECORD FOR EACH TAPE MOUNT
  IF THE WTOETPS1 AND WTOETPS2 MODULES ARE NOT USED.

MEMBER WTOERWAT IS A MODIFICATION OF THE COCA-COLA EXIT WHICH WILL
  RESPOND 'WAIT' TO MESSAGE IEF238D AND WRITE AN SMF RECORD TO INDICATE
  THE ALLOCATION RECOVERY CONDITION.

MEMBER WTOTAPAL IS THE EXIT TO ONLY WRITE THE SMF RECORD FOR ALLOCATION
  RECOVERY.

MEMBERS LISTGDGC AND LISTGDGP ARE A PAIR OF PROGRAMS THAT COMPRISE
  THE LISTGDG TSO COMMAND.  THIS COMMAND WILL LIST THE ATTRIBUTES OF
  A GDG AND THE MOST RECENTLY CREATED GENERATIONS.  THE NUMBER OF
  GENERATIONS RETAINED IN THE CATALOG MAY BE CHANGED UPON REQUEST.  NEW
  GDG BASE ENTRIES MAY ALSO BE CREATED. THIS COMMAND WORKS WITH ICF
  CATALOGS AND HAS SUPPORT FOR 3380 DISK AND 3480 CARTS.  THE COMMAND
  IS IN TWO PARTS:  THE ALLOCATION PIECE WHICH IS WRITTEN IN ASSEMBLER;
  AND THE LOGIC PIECE WRITTEN IN PL1.

MEMBER IKJEFF10 IS A TSO SUBMIT EXIT
  THIS EXIT WILL CONDITIONALLY CHECK THE JOB CARD SUBMITTED TO VERIFY
  THAT THE JOBNAME STARTS WITH THE USERID OR FIRST N CHAR OF USERID.
  THE EXECUTION CLASS, MSGCLASS, AND TIME PARAMETERS ARE ALSO
  CONDITIONALLY CHECKED AND MAY BE MANDITORY AND/OR IN THE APPROPRIATE
  TABLES.   A TIME PARAMETER MAY ALSO BE INSERTED BY THE EXIT.
  ALL CHECKING IS BASED ON THE USERID AND THE PRIVILIGES ALLOWED THAT
  USER IN THE UIDTABLE.
  JOB CLASSES MAY HAVE FLAGS TO REQUIRE TIME PARAMETERS OR REQUIRE NOT
  TO HAVE THEM. ALSO, THERE MAY BE MAX TIME AND DEFAULT TIME BY CLASS.
  COMMAND AND CERTAIN JES 2 CONTROL CARDS WILL NOT BE ALLOWED IN THE
  SUBMITTED JCL.
```
