build:
	docker build -t apache-spark:2.4.8 .
compose:
	docker-compose up
	#See https://localhost:4040 for spark UI
exec:
	docker exec -it spark-master /bin/bash
submit:
	./spark-submit --master spark://0.0.0.0:7077 --name spark-pi --class org.apache.spark.examples.SparkPi  local:///opt/spark/examples/jars/spark-examples_2.12-3.4.0.jar 100