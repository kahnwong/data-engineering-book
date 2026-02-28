---
title: Tools
---

เครื่องมือต่างๆ ในโลก Data Engineering

## Change Data Capture

### [Debezium](https://debezium.io/)

Debezium คือ open-source platform สำหรับทำ Change Data Capture (CDC) หรือการตรวจจับการเปลี่ยนแปลงของข้อมูลใน database แบบ real-time

## Dashboard

### [Dash](https://dash.plotly.com/)

Dash เป็น Open Source Framework ในการทำ Dashboard Visualization ในรูปแบบ Web App สร้าวขึ้นบน `plotly.js`, `React` และ `Flask` ดังนั้น Dash จึงเหมาะสมสำหรับชาว Data ที่อาจจะไม่ได้เขียนเว็บมาก่อน ตัว Dash จึงเป็น python framework ที่คอยจัดการ Web App ให้ โดยสร้างขึ้นมาจากทีมงานเดียวกับ plotly

### [Kibana](https://www.elastic.co/kibana/)

Kibana คือ เครื่องมือแสดงข้อมูลด้วยภาพและสำรวจข้อมูลที่ใช้สำหรับการวิเคราะห์บันทึกและอนุกรมเวลา เป็น web UI ที่เชื่อมต่อกับ [Elasticsearch](##-Elasticsearch) และ [Logstash](##-Logstash) จึงเป็นเครื่องมือที่นิยมใช้ในการวิเคราะห์ Log สามารถสร้าง dashboard จากข้อมูลใน Elasticsearch ได้

### [Data Studio](https://datastudio.google.com/)

Data Studio คือเครื่องมือสำหรับสร้าง Dashboard ของทาง Google สามารถสร้างและใช้งานผ่าน Web Browser ได้ โดยสามารถแสดงข้อมูลในรูปแบบ Chart, Table, Maps และอื่น ๆ รวมถึงรองรับการเชื่อมต่อกับ service ภายนอกเช่น BigQuery, Dataprep, Google Analytics, Google Cloud Storage เป็นต้น

### [Redash](https://redash.io/)

Redash เป็นเครื่องมือสำหรับการทำ dashboard/visualize data ใช้งานผ่าน browser สามารถจัดการ data source ผ่าน Query Editor รองรับ data source ทั้ง SQL และ NoSQL
มีระบบ Alert และ Schedule refreshes คอยช่วย update data ให้เป็น up-to-date

### [Streamlit](https://streamlit.io)

Open-source Python library เอาไว้สร้าง data app (หรือ web app) สำหรับโปรเจค data
science กับ machine learning เราไม่จำเป็นต้องเขียน front-end เลย ลองเข้าไปดูตัวอย่างได้ที่
[Gallery](https://streamlit.io/gallery) ได้

### [Superset](https://superset.apache.org/)

Apache Superset เป็นโปรแกรม Visualization Tools/Business Intelligence ที่มีข้อดีคือใหม่และมีความเป็น Developer-based สูงมาก เนื่องจากเป็นโปรแกรมที่ใช้เชื่อมกับ Service ของ Big Data ต่างๆ เช่น Cloud Database, Data Warehouse เป็นต้น

## Datastore

### [Elasticsearch](https://www.elastic.co/)

Elasticsearch คือ โอเพนซอร์สสำหรับค้นหาข้อมูลต่างๆ(search engine database) และสามารถวิเคราะห์ข้อมูลแบบกระจายได้

Elastic Docs: <https://www.elastic.co/guide/index.html>

### [Druid](https://druid.apache.org/)

Druid เป็น real-time analytics database ที่เป็นลูกครึ่งระหว่าง columnar database กับ time-series database เหมาะสำหรับการทำ large scale analytics กับ time-series data

### [Hadoop](https://hadoop.apache.org/)

Hadoop หรือ Apache Hadoop คือ โอเพนซอร์ส framework สำหรับการประมวลผลข้อมูลขนาดใหญ่ บนกลุ่มเครื่องคอมพิวเตอร์ (cluster) Hadoop ถูกสร้างขึ้นตั้งแต่ปี 2006
Hadoop มีองค์ประกอบหลายส่วน เช่น

* HDFS สำหรับจัดการการจัดเก็บข้อมูล
* YARN สำหรับจัดการทรัพยากรในการประมวลผล
* MapReduce วิธีการแบบดั้งเดิมในการประมวลผลข้อมูลขนาดใหญ่แบบคู่ขนาน (parallel)
* Hive สำหรับการจัดการ data warehouse บน Hadoop ด้วยภาษา SQL (HiveQL)
* [Spark](##-Spark)สำหรับการประมวลผลข้อมูลขนาดใหญ่ ที่ได้รับความนิยมเป็นอย่างมาก

### [MongoDB](https://www.mongodb.com/)

MongoDB คือ โอเพนซอร์สสำหรับฐานข้อมูลเอกสาร (Document Database: ฐานข้อมูล NoSQL ชนิดหนึ่งซึ่งมีการเก็บข้อมูลในรูปแบบ JSON Object) ที่มีประสิทธิภาพสูง (High Performance) มีความพร้อมใช้งานสูง (High Availability) และมีการปรับขนาดอัตโนมัติ (Automatic Scaling)

### [Snowflake](https://www.snowflake.com/)

Snowflake คือ data warehouse ที่เป็น columnar database เหมาะสำหรับทีมที่มีความชำนาญใน sql เพราะสามารถเขียน sql pipelines ได้ตรงๆ โดยที่ไม่จำเป็นต้องใช้ python ในการสร้าง pipeline เพื่อเอาข้อมูลเข้า

## Data Catalog

### [Amundsen](https://www.amundsen.io/)

### [Marquez](https://marquezproject.github.io/marquez/)

Marquez สามารถรับ [OpenLineage](https://openlineage.io/) metadata เพื่อนำมาแสดงผลเป็น data lineage สำหรับ assets ทั้งหมดที่มีอยู่ในองค์กร

## Data Integration

### [Airbyte](https://airbyte.io/)

Airbyte เป็นเครื่องมือโอเพนซอร์สที่ช่วยทำให้ข้อมูลเชื่อมต่อ และสอดคล้องกันระหว่างแอพพลิเคชั่น API
และฐานข้อมูล กับระบบปลายทางที่เก็บข้อมูลอื่นๆ อาทิ เช่น Data Warehouse หรือ Data Lake

## Data Quality

### [Great Expectations](https://greatexpectations.io/)

Great Expectations เป็นเครื่องมือที่ช่วยให้เราดูแลรักษาคุณภาพของข้อมูล (data quality) ไว้ โดยผ่านฟังก์ชั่นการทำงานที่เข้าใจได้ง่าย อย่างเช่น `expect_table_row_count_to_be_between` ที่เอาไว้ตรวจสอบจำนวนแถวของตารางว่าควรจะมีจำนวนแถวอยู่ระหว่างเท่าไหร่ถึงเท่าไหร่ เป็นต้น

### [Soda Core](https://www.soda.io/core)

Soda Core เป็นเครื่องมือ open source ที่ช่วยเรื่อง data reliability มีทั้งแบบ CLI และ Python library เราสามารถที่จะเอามาใช้ตรวจสอบคุณภาพของข้อมูลใน data pipeline หรือในระบบ data observability ของเราได้

จะมีเครื่องมืออีกตัวหนึ่งที่ชื่อว่า [Soda Checks Language (SodaCL)](https://docs.soda.io/soda-cl/soda-cl-overview.html) ที่สร้างขึ้นมาบนตัว Soda Core อีกที โดยเราจะสามารถเขียนภาษาที่เป็น domain-specific language (DSL) ที่ถูกออกแบบมาเน้นให้ human-readable เพื่อที่ต้องการจะให้ใครก็ตามในองค์กรสามารถตรวจสอบคุณภาพของข้อมูลได้ด้วยตัวเอง

## Data Transformation

### [dbt](https://www.getdbt.com/)

* [dbt คืออะไรนะ?](https://zkan.hashnode.dev/what-is-dbt)
* [เริ่มต้นกับ dbt](https://zkan.hashnode.dev/get-started-with-dbt)
* [การจัดการโมเดลใน dbt และการทดสอบ](https://zkan.hashnode.dev/dbt-models-and-tests)

### [Spark](https://spark.apache.org/)

Spark หรือ Apache Spark เป็นเครื่องมือที่เราจะเอาไว้ประมวลผลข้อมูลขนาดใหญ่ หรือสร้างโมลเดล Machine Learning จากข้อมูลขนาดใหญ่ โดยที่เราสามารถนำเอาไปใช้กับ batch processing หรือ real-time processing ก็ได้

เครื่องมือตัวนี้แทบจะเป็นตัวเลือกในอันดับต้นๆ เลยก็ว่าได้ที่เอามาใช้ในการประมวลผลข้อมูลขนาดใหญ่ ตอนที่ประมวลผล Spark จะประมวลผลแบบ in-memory ทำให้การประมวลผลนั้นทำได้รวดเร็วมาก เมื่อเทียบกับ Hadoop MapReduce ที่ใช้การอ่านเขียนข้อมูลที่เป็นไฟล์จาก disk

Spark มี library ที่รองรับได้หลายภาษา เช่น Java, Scala, Python (PySpark), R (SparkR)

## Infrastructure

### [Docker](https://www.docker.com/)

Docker เป็นแพลตฟอร์มซอฟต์แวร์ที่แยกแอพพลิเคชั่นของคุณออกจากกัน โดยการเรียกใช้งานพวกมันในส่วนเฉพาะที่เรียกว่า Container โดย Docker Container จะมีส่วนที่คล้ายกันกับ Virtual Machine (VM) เพียงเล็กน้อย ตรงที่มันจะแยก Content ของมันออกจากซอฟต์แวร์อื่น ๆ ที่กำลังทำงานอยู่ในเครื่อง

Documentation: <https://docs.docker.com/>

### [Kubernetes](https://kubernetes.io/)

Documentation: <https://kubernetes.io/docs/home/>

Kubernetes หรือที่เรียกว่า K8s เป็นแพลตฟอร์มแบบ Open-source สำหรับช่วยให้การปฏิบัติงานต่างๆ ที่เกี่ยวข้องกับ Linux Container สามารถทำได้โดยอัตโนมัติ ลดกระบวนการติดตั้งหรือขยายแอปพลิเคชันที่รันบน Container ที่นักพัฒนาต้องลงมือทำด้วยตนเองให้เหลือน้อยที่สุด

## Monitoring & Observability

### [Grafana](https://grafana.com/)

Grafana คือ เครื่องมือโอเพนซอร์ส สำหรับการแสดงผลข้อมูลที่เป็นอนุกรมเวลา และสร้าง dashboard ได้ นิยมใช้ในการแสดงผลกราฟเพื่อดูแลประสิทธิภาพของระบบ (performance monitoring) สามารถต่อเชื่อมกับฐานข้อมูลได้หลายประเภท

### [Fluentd](https://www.fluentd.org/)

Open source data collector for unified logging layer

* [How Fluentd simplifies collecting and consuming logs | Fluentd simply explained](https://www.youtube.com/watch?v=5ofsNyHZwWE)

### [Logstash](https://www.elastic.co/logstash/)

Logstash คือ โอเพนซอร์สสำหรับงานประมวลผลข้อมูลฝั่งเซิร์ฟเวอร์ ที่สามารถนำเข้าข้อมูลจากแหล่งต่าง ๆ พร้อมกับแปลงข้อมูลให้อยู่ในรูปแบบที่ต้องการได้ นิยมใช้ในการ process ข้อมูลประเภท Log

## Orchestration

### [Airflow](https://airflow.apache.org/)

Airflow หรือ Apache Airflow คือโอเพนซอร์สแพลตฟอร์มประเภท task orchestrator ที่เราสามารถที่จะตรวจสอบ ทำตารางเวลา และเฝ้าสังเกต กระแสงาน หรือ Workflow ขั้นตอนการประมวลผลได้

การที่เราสามารถเขียนโค้ดเพื่อกำหนด Workflow ได้ จะทำให้เราดูแลรักษา Workflow ได้ง่ายขึ้น สามารถเก็บเป็นเวอร์ชั่น สามารถทดสอบ
และสามารถทำให้การทำงานร่วมกันง่ายขึ้นได้

* [Airflow 2.0 มีอะไรใหม่บ้าง มาดูกัน 🤩](https://medium.com/odds-team/airflow-2-0-%E0%B8%A1%E0%B8%B5%E0%B8%AD%E0%B8%B0%E0%B9%84%E0%B8%A3%E0%B9%83%E0%B8%AB%E0%B8%A1%E0%B9%88%E0%B8%9A%E0%B9%89%E0%B8%B2%E0%B8%87-%E0%B8%A1%E0%B8%B2%E0%B8%94%E0%B8%B9%E0%B8%81%E0%B8%B1%E0%B8%99-362aa07472ba)
* [เขียน Document ใน Airflow โดยใช้ doc_md](https://medium.com/pyconth/%E0%B9%80%E0%B8%82%E0%B8%B5%E0%B8%A2%E0%B8%99-document-%E0%B9%83%E0%B8%99-airflow-%E0%B9%82%E0%B8%94%E0%B8%A2%E0%B9%83%E0%B8%8A%E0%B9%89-doc-md-e2a29b489f7b)
* [Setup Airflow on Kubernetes with remote logging to GCS](https://mesodiar.com/setup-airflow-on-kubernetes-with-remote-logging-to-gcs-bf7869642b4c)
* [[Airflow] ย้ายไฟล์จาก GCS ไป BigQuery ด้วย GoogleCloudStorageToBigQueryOperator กัน !](https://medium.com/mils-blog/airflow-%E0%B8%A2%E0%B9%89%E0%B8%B2%E0%B8%A2%E0%B9%84%E0%B8%9F%E0%B8%A5%E0%B9%8C%E0%B8%88%E0%B8%B2%E0%B8%81-gcs-%E0%B9%84%E0%B8%9B-bigquery-%E0%B8%94%E0%B9%89%E0%B8%A7%E0%B8%A2-googlecloudstoragetobigqueryoperator-%E0%B8%81%E0%B8%B1%E0%B8%99-221f8d9b65c0)

### [Dagster](https://dagster.io/)

Dagster คือ เครื่องมือโอเพนซอร์สสำหรับสร้าง data pipeline ด้วย Python ที่มีแนวคิดในการพัฒนาและดูแล data assets สามารถเขียน pipeline จากในโค้ดได้โดยตรง พร้อม web UI ที่ตรวจสอบติดตามการรันได้

### [Flyte](https://docs.flyte.org)

Flyte คือ โอเพนซอร์สสำหรับสร้าง workflow เพื่อใช้งานบน container สามารถใช้งานร่วมกับ [Kubernetes](##-Kubernetes) ได้ โดยสามารถสร้าง pipeline ด้วย Flyte SDK ที่รองรับทั้ง Python Java และ Scala

### [Luigi](https://luigi.readthedocs.io/en/stable/)

Luigi คือ โอเพนซอร์สแพ็กเกจสำหรับสร้าง data pipeline แบบ batch ที่มีความซับซ้อน รองรับการรัน job ที่ใช้เวลาในการรันนาน และใช้ร่วมกับ Hadoop ได้ (เช่น Hive Spark) โดยใช้ภาษา Python Luigi ถูกสร้างขึ้นโดยบริษัท Spotify ตั้งแต่ปี 2012

### [Orchest](https://www.orchest.io/)

Orchest คือ open source สำหรับสร้าง data pipeline ด้วยวิธีง่ายๆ โดยตรงจากเบราว์เซอร์

### [Prefect](https://www.prefect.io/opensource/)

Prefect คือ open source สำหรับสร้าง data pipeline ด้วย Python โดยสามารถเขียน workflow ได้โดยตรงจาก code พร้อม web UI เพื่อตรวจสอบติดตามการรันได้

## Storage

### [AWS S3](https://aws.amazon.com/s3/)

AWS S3 หรือ Amazon Simple Storage Service เป็นพื้นที่จัดเก็บไฟล์บนคลาวด์ของทาง Amazon Web Services (AWS) เหมาะกับการใช้งานที่หลากหลาย เช่น จัดเก็บข้อมูลดิบ เว็บไซต์ แอปพลิเคชันมือถือ การสำรองข้อมูลและการคืนค่า การเก็บข้อมูลแบบถาวร รวมทั้งการวิเคราะห์ Big Data

### [Azure Blob Storage](https://azure.microsoft.com/services/storage/blobs)

Azure Blob Storage เป็นพื้นที่จัดเก็บไฟล์บนคลาวด์ของทาง Microsoft Azure ที่เหมาะสำหรับ Unstructured data โดยเฉพาะ

### [Google Cloud Storage](https://cloud.google.com/storage)

Google Cloud Storage เป็นพื้นที่จัดเก็บไฟล์บนคลาวด์ของทาง Google Cloud ที่สามารถเลือกภูมิภาค (region) ในการจัดเก็บไฟล์ได้หลากหลาย ซี่งช่วยให้การรับส่งไฟล์มีความหน่วงน้อย (low latency)

## Streaming

### [Kafka](https://kafka.apache.org/)

Apache Kafka เป็นซอฟต์แวร์จัดการ event streaming (บางที่เรียกว่า data pipeline) เพื่อนำข้อมูลปริมาณมากๆ เข้าระบบอย่างรวดเร็ว

### [Pulsar](https://pulsar.apache.org/)

Apache Pulsar คือ cloud-native, multi-tenant, high-performance solution สำหรับส่งข้อความแบบ server-to-server และการจัดคิวที่สร้างขึ้นบน publisher-subscribe (pub-sub) pattern โดย Pursar ผสมผสานคุณสมบัติที่ดีที่สุดของระบบการส่งข้อความแบบดั้งเดิม เช่น RabbitMQ เข้ากับระบบ pub-sub เช่น Apache Kafka ซึ่งเพิ่มหรือลดขนาดแบบไดนามิกโดยไม่ต้องหยุดทำงาน

## Data Science

### [Knime](https://www.knime.com/)

Knime คือ เครื่องมือใช้สำหรับการทำ end-to-end data science มีลักษณะคล้ายคลึงกับ [RapidMiner](##-RapidMiner) เช่น การเรียนรู้เครื่อง การเรียนรู้ลึก การทำเหมืองข้อมูล การวิเคราะห์การทำนาย (Predictive analysis) และการแปลผล นอกจากนั้นยังสามารถใช้ในการทำ Data mining (ขุดข้อมูล) และ Machine learning ซึ่งรวมไปถึงการโหลดและการแปลงข้อมูล (ETL) การประมวลผลล่วงหน้าและการวาดภาพจากข้อมูล การวิเคราะห์เชิงพยากรณ์และการสร้างแบบจำลองทางสถิติ การประเมินผลและการปรับใช้ ต่างๆ ทั้งยังมี Graphical User Interface (GUI) ที่เข้าใจง่ายผ่านการทำงานแบบ workflow diagram และสามารถเขียน code เพิ่มเติม ผ่านการทำงานแบบ customize workflow node ได้เช่นกัน

### [RapidMiner](https://rapidminer.com/)
