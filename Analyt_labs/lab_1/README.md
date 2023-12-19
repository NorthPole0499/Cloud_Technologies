# Аналитическая лабораторная работа №1 AWS. Варинат 11

### Цель работы:

Знакомство с облачными сервисами. Понимание уровней абстракции над инфраструктурой в облаке. Формирование понимания типов потребления сервисов в сервисной-модели. 
Сопоставление сервисов между разными провайдерами. Оценка возможностей миграции на отечественные сервисы.

### Дано:

1. Слепок данных биллинга от провайдера после небольшой обработки в виде SQL-параметров. Символ % в начале/конце означает,
   что перед/после него может стоять любой набор символов.
2. Google с документациями провайдера

### Ход работы

Необходимо импортировать файл .csv в Excel и определить соответствие каждого сервиса международного провайдера русскому сервису. 
Заполнить информацию об отечественных сервисах, сопоставляя их напротив AWS сервисам.


| Product Code            | Usage Type                   |  [lineItem/Operation] | lineItem/LineItemDescription | Russian Service                |
|-------------------------|------------------------------|-----------------------|------------------------------|--------------------------------|
| AmazonAthena            | %DataScanned%                |                       |                              | None                           |
| AmazonS3                | %StorageAnalytics%           |                       |                              | Yandex Object Storage          |
| APNFee                  |                              |                       | Tax%                         | Yandex Cloud Billing           |
| APNFee                  | %Purchase%                   |                       |                              | Yandex Cloud Billing           |
| AmazonAppStream         |                              |                       | Tax%                         | Yandex Data Streams            |
| AmazonAppStream         | %stream%                     |                       |                              | Yandex Data Streams            |
| AmazonAppStream         | %StoppedInstance%            |                       |                              | Yandex Data Streams            |
| AmazonAppStream         | %Win-User                    |                       |                              | Yandex Data Streams            |
| AmazonLex               |                              |                       | Tax%                         | SberDevices Dialog Platform    |
| AmazonLex               | %Req%                        |                       |                              | SberDevices Dialog Platform    |
| AmazonLightsail         | %DataXfer%                   |                       |                              | Yandex Compute Cloud           |
| AmazonLightsail         | %UnusedStaticIP              |                       |                              | Yandex Compute Cloud           |
| AmazonLightsail         | %BundleUsage%                |                       |                              | Yandex Compute Cloud           |
| AmazonLightsail         | %DiskUsage                   |                       |                              | Yandex Compute Cloud           |
| AmazonLightsail         | %SnapshotUsage               |                       |                              | Yandex Compute Cloud           |
| AmazonNeptune           |                              |                       | Tax%                         | Comindware ElasticData         |
| AmazonNeptune           | %InstanceUsage%              |                       |                              | Comindware ElasticData         |
| AmazonNeptune           | %StorageIOUsage%             |                       |                              | Comindware ElasticData         |
| AmazonNeptune           | %StorageUsage%               |                       |                              | Comindware ElasticData         |
| AmazonNeptune           | %BackupUsage%                |                       |                              | Comindware ElasticData         |
| AmazonManagedBlockchain | %Node%                       |                       |                              | QIWI Blockchain Technologies   |
| AmazonManagedBlockchain |                              |                       | Tax%                         | QIWI Blockchain Technologies   |
| AmazonManagedBlockchain | %Member                      |                       |                              | QIWI Blockchain Technologies   |
| AmazonMacie             |                              |                       |                              | None                           |
| AmazonML                | %AMLBoxUsage                 | DataStats             |                              | Yandex DataSphere              |
| AmazonML                | %BatchPredictionChunk        |                       |                              | Yandex DataSphere              |
| AmazonML                | %AMLBoxUsage                 | TrainModel            |                              | Yandex DataSphere              |
| AmazonML                | %AMLBoxUsage                 | EvaluateModel         |                              | Yandex DataSphere              |
| AWSConfig               |                              |                       | Tax%                         | Yandex Audit Trails            |
| AWSConfig               | %ConfigurationItemRecorded   |                       |                              | Yandex Audit Trails            |
| AWSConfig               | %ConfigRuleEvaluations       |                       |                              | Yandex Audit Trails            |
| AWSCostExplorer         |                              |                       | Tax%                         | Selectel оптимизация IT-затрат |
| AWSCostExplorer         | %APIRequest                  |                       |                              | Selectel оптимизация IT-затрат |
| AWSCostExplorer         | %DataStorage                 |                       |                              | Selectel оптимизация IT-затрат |
| AWSGlobalAccelerator    | Global-Accelerator-fixed-fee |                       |                              | Selectel SDN                   |
| AWSGlobalAccelerator    | %Bytes%                      |                       |                              | Selectel SDN                   |
| AWSGlobalAccelerator    |                              |                       | Tax%                         | Selectel SDN                   |
| AWSGlue                 | %DEVED-DPU-Hour%             |                       |                              | None                           |
| AWSGlue                 | %Catalog-Request             |                       |                              | None                           |
| AWSGlue                 | %Catalog-Storage             |                       |                              | None                           |
| AWSGlue                 | %Crawler-DPU-Hour%           |                       |                              | None                           |
| AWSGlue                 | %ETL-DPU-Hour%               |                       |                              | None                           |
| AWSGreengrass           | %ActiveGGC-Devices           | SingleNode            |                              | Yandex IoT Core                |
