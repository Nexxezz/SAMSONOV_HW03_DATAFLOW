TASK 1.
1. Created sandbox-hdp and sandbox-hdf containers.
2.Preconfiqured NiFi according to a pre-configuration guide.
3.Created AcquireHVACData Process Group(screenshot 1,2).
2. Added and configured GetHTTP processor(screenshot 3).
3. Added and configured UnpackContent processor(screenshot 4, 5).
4. Added and configured two PutHDFS processsors (screenshots 6-12).
5. Started Process Group flow.
6. Verified that NiFi stored data(screenshots 13-19).
7. Created Process Group via UI: uploaded template from acquire-hvac-data.xml file (screenshots 21-23).
8. Creataed Process group via REST call(screenshots 24, 25).
9. Checked that data uploaded to HDFS via Ambari File View(screenshots 26, 27).
  
TASK 2.
1. Downloaded and created Streamsets Data Collector container.
2. Created data pipeline(screenshot 28):
	copied hotels data to HDFS;
	added Hadoop FS Standalone origin for reading hotels data from HDFS;
	added sample processor which include code that check hotels csv files /
	for incorrect(null) Latitude and Longitude values, maped them to correct /
	values(based on addres,city and country columns in hotels files) /
	with OpenCage Geocoding API;
	generated geohash values based on Latitude and Longitude values with geohash-java library;
	created hotels-data topic in Kafka;
	stored data in hotels-data topic with Kafka consumer destination;
	viewed data from Kafka topic in HDP vconsole(screenshot 29).