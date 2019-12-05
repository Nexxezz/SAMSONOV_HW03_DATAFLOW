TASK 1

1. Created sandbox-hdp and sandbox-hdf containers.
1.1 Preconfiqured NiFi according to a pre-configuration guide.
2.Completed Building an HVAC System Analysis Application tutorial.
2.1 Created AcquireHVACData Process Group(screenshot 1,2).
2.2 Added and configured GetHTTP processor(screenshot 3).
2.3 Added and configured UnpackContent processor(screenshot 4, 5).
2.4 Added and configured two PutHDFS processsors (screenshots 6-12).
2.5 Started Process Group flow.
2.6 Verified that NiFi stored data(screenshots 13-19).
2.7 Created Process Group via UI: uploaded template from acquire-hvac-data.xml file (screenshots 21-23).
2.8 Creataed Process group via REST call(screenshots 24, 25).
2.9 Checked that data uploaded to HDFS via Ambari File View(screenshots 26, 27).
  
TASK 2.
1. Downloaded and created Streamsets Data Collector container.
2. Created data pipeline for joining Hotels data(screenshot 28):
3. Read hotels data from HDFS.
4. Checked hotels data for incorrect(null) Longitude & Latitude values. Map incorrect values from OpenCage /
Geocoding API in the pipeline.
5. Generated geohash by Latitude & Longitude with geohash-java library with 5-charachers length in extra column.
6. Stored data in Kafka topic:
6.1 Created hotels-data topic in Kafka;
6.2Stored data in hotels-data topic with Kafka consumer destination;
6.3Viewed data from Kafka topic in HDP vconsole(screenshot 29).
