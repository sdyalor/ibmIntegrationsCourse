Queue Manager =>
  crtmqm -u QMGR1
  dspmq
  strmqm QMGR1
Intetration Node =>
  mqsicreatebroker BRKTEST1 -q QMGR1 -i userbus -a userbus
  //created stoped
  mqsilist
  mqsistart BRKTEST1
  mqsideletebroker BRKEST1
  Execution Group =>
mqsicreateexecutiongroup BRKTEST1 -e EG_01