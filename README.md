# mediapipe_video_analysis on kubernetes

For production level application

1. Model should keep being retrained and updated, therefore it should be decoupled with code.

2. 

## Architecture

Video Stream --> Docker(Kafka producer python) --> Docker(Kafka cluster) --> Docker(Kafka consumer python + mediapipe) --> monitoring
                                                                                                                       --> Display Dashboard  
                                                                                                                       
Video Stream --> Docker(Kafka producer python) --> Docker(Kafka cluster) --> Docker(Kafka Seldon Core) --> monitoring
                                                                                                       --> Display Dashboard


## Video Source

1. RTSP stream --> Kafka


## Install Zookeeper


## Install Kafka


## Reference

-- Detectron2 pipeline
-- Video Analysis Serving
