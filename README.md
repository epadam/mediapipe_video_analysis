# mediapipe_video_analysis on kubernetes

For production level application

1. Model should keep being retrained and updated, therefore it should be decoupled with code.

2. 

## Architecture

Video Source --> (Video Stream(webRTC/rtsp)) --> Docker(Kafka producer python) --> Docker(Kafka cluster) --> Docker(Kafka consumer/python + mediapipe or seldon core) 

-meta data-> Docker(kafka cluster) --> Docker(Spark)    --> Docker(Cassandra)     --> 
                                   --> Docker(Logstash) --> Docker(ElasticSearch) --> Docker(API) --> Docker(UI) -->
                                                                                  --> Docker(Kibana)             --> Browser

## Video Source
0. a video file
1. video source --> RTSP stream --> Kafka producer 

Dockerfile

## Reference

-- Detectron2 pipeline
-- Video Analysis Serving
