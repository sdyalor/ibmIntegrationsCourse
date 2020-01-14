Queue Manager =>
```
  crtmqm -u QMGR1
  dspmq
  strmqm QMGR1
```
Intetration Node =>
  mqsicreatebroker BRKTEST1 -q QMGR1 -i userbus -a userbus
  //created stoped
  mqsilist
  mqsistart BRKTEST1
  mqsideletebroker BRKEST1

Execution Group =>
mqsicreateexecutiongroup BRKTEST1 -e EG_01
mqsilist

Queue Name

*QL.TEST.REQ.01*

runmqsc QMGR1
d //enter
  tooltips

```DEFINE QLOCAL (QL.TEST.REQ.01)```
```DEFINE QLOCAL (QL.TEST.RES.01)```
Check Local Queue List
DISPLAY QLOCAL (QL.*)
END
![](2020-01-14-12-50-54.png)
...

After trace creation
![](2020-01-14-12-58-50.png)
amqsput QL.TEST.REQ.01 QMGR1
HOLA MUNDO
![](2020-01-14-12-57-36.png)
![](2020-01-14-12-58-02.png)

const chain = [
  20B: "CELSO",
  20B: "",
  20B: ""
]

![](2020-01-14-14-13-38.png)
To access in esql
DECLARE cadena CHARACTER ";
//SET cadena = InputRoot.BLOB.BLOB
SET cadena = CAST InputRoot.BLOB.BLOB AS CHARACTER CCSID InputRoot.CodedCharSetId

SET ENVIRONMENT.cadena = cadena;
![](2020-01-14-14-21-54.png)

            julio   
            cesar   
            torres  
            julio               cesar               torres  