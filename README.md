# MITRE Range-Angle (Unstructured)

**Overview:**

This dataset contains measurements similar to the the MITLL range-angle protocol, but taken in an unstructured manner.  Unlike the range-angle protocol (Structured Contact Tracing Protocol, V.2.0), testers chose their own range, angle and number of tests per set.  As a result the dataset does not contain complete range-angle sets, but there is more variety in environment, phone carrying position, pose, etc.  The data was collected by 12 MITRE employees at their homes.

This data was collected using the original version of the BluetoothProx app (V1.0), before metadata such as phone carrying position, pose, etc. was embededded in the log file.  The files have been post processed to match the format of the new version of the app (V2.0) to the extent possible.

**The following are differences between this test procedure / file format and the current range-angle protocol (_Structured Contact Tracing Protocol, V.2.0_) test procedure / file format:**

- Testers did not follow a structured test sequence.  They chose their own range, angle and conditions for each test.
- Each log file contains data for a single range, angle and set of conditions
- Data was collected for 60 seconds per test
- For all tests, person with the receiving device was standing with device in their hands (in typical "texting" position).  Only the position and pose of the beacon device was changed.
- Beacon devices used nRF Connect to send advertising packets instead of the BlueProx app.  This allowed both iOS and Android devices to used.  In total, 7 iOS devices and 4 Android devices were used as the beacon device.  (Device types are reported in log files as "self_tester" and "partner_tester".)
- Log files have a comment field with additional details.

Refer to Index.xlsx for a summary of log files.  In some cases, photos provided by the test participants are included in the subfolders.

##Contact:
	Mark Krangle
	The MITRE Corporation
	mkrangle@mitre.org
	781-271-7008
