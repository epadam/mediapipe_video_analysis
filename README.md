# mediapipe_video_analysis on kubernetes

Use mediapipe with kafka

In this example we try to wrap mediapipe in the predictor

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
