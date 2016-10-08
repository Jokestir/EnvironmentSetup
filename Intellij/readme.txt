intellij optimization:


- disable all unused plugins (settings -> plugins)

- disable spell check (settings -> inspections)

- Add below to idea64.exe.vmoptions in bin folder

- load the jar

-server
-Xms2048m
-Xmx2048m
-XX:NewSize=512m
-XX:MaxNewSize=512m
-XX:PermSize=512m
-XX:MaxPermSize=512m
-XX:+UseParNewGC
-XX:ParallelGCThreads=4
-XX:MaxTenuringThreshold=1
-XX:SurvivorRatio=8
-XX:+UseCodeCacheFlushing
-XX:+UseConcMarkSweepGC
-XX:+AggressiveOpts
-XX:+CMSClassUnloadingEnabled
-XX:+CMSIncrementalMode
-XX:+CMSIncrementalPacing
-XX:+CMSParallelRemarkEnabled
-XX:CMSInitiatingOccupancyFraction=65
-XX:+CMSScavengeBeforeRemark
-XX:+UseCMSInitiatingOccupancyOnly
-XX:ReservedCodeCacheSize=64m
-XX:-TraceClassUnloading
-ea
-Dsun.io.useCanonCaches=false

(do the same forpycharm,android studio)






