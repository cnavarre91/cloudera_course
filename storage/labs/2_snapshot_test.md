1- Create "precious" directory
   #hdfs dfs -mkdir -p /precious

2-Allowing creation of snapshots:
  #hdfs dfsadmin -allowSnapshot  /precious

3-Copying the required file to precious:
  #hdfs dfs -put /tmp/SEBC.zip /precious

4-Creating a Snapshot
   #hdfs dfs -createSnapshot /precious sebc-hdfs-test
   
5-Trying to remove dir precious:
  #hdfs dfs -rm -r -skipTrash /precious
Result: rm: The directory /precious cannot be deleted since /precious is snapshottable and already has snapshots

6-Trying to remeve file SBEC.zip
   #hdfs dfs -rm -r -skipTrash /precious/SEBC.zip
   
7-Recovering the deleted file
   #hdfs dfs -cp /precious/.snapshot/sebc-hdfs-test/SEBC.zip /precious
   
   
