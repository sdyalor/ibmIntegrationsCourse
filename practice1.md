crtmqm QMGR1
strmqm QMGR1

mqsicreatebroker BRKTEST1 -q QMGR1 -i userbus -a userbus
mqsistart BRKTEST1


https://www.ibm.com/support/knowledgecenter/en/SSMKHH_9.0.0/com.ibm.etools.mft.doc/ac12610_.htm
https://www.ibm.com/support/knowledgecenter/en/SSTTDS_11.0.0/com.ibm.etools.mft.doc/ak05260_.html
https://www.ibm.com/support/knowledgecenter/en/SSMKHH_9.0.0/com.ibm.etools.mft.doc/ak05740_.htm
https://www.ibm.com/support/knowledgecenter/SSMKHH_9.0.0/com.ibm.etools.mft.doc/ak05911_.htm


mqsireportproperties BRKTEST1 -e EG_01 -o HTTPSConnector -r

https://www.ibm.com/support/knowledgecenter/es/SSMKHH_9.0.0/com.ibm.etools.mft.doc/ac16862_.htm

mqsisetdbparms BRK01 -n odbc::DBBRK -u USRBRK -p USRBRK
mqsicvp INODE -n myDsn


mqsisetdbparms BRKTEST1 -n odbc::ACE_SAMPLE -u ACE_SAMPLE -p acesample2019
mqsicvp BRKTEST1 -n ACE_SAMPLE





mqsireportproperties BROKERH1 -e EG_HU_RENIECREST -o HTTPConnector -r
mqsireportproperties myBroker -e default -o HTTPSConnector -r
mqsireportproperties myBroker -e default -o HTTPSConnector -r



SET OutputLocalEnvironment.Destination.HTTP.RequestIdentifier =
erddtcfyvgubhnjkm