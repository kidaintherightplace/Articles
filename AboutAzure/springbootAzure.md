### Azure 笔记



1. Blob 存储
   - 适用于云的对象存储解决方案。
   - 适合存储巨量的非结构化数据。即不遵循特定数据模型或定义的数据，如文本或二进制数据。
   - 只能同时有一个用户去连接操作。
   - Paas 
   - 责任共担模式
   - Capex 资本性支出，固定资产等。
   - Opex  企业管理支出
   - 功能类似于百度网盘，区别在于对象存储非字节存储。
   - 

2. springboot显示blob list

   - 登录后点击帐户

   - azure.myblob.usl=blobEndpoint… 

   - azure.myblob.container=mfiafd

   - Jar 包： com.azure:azure-storage-blob:12.4.8

   - `private BlobContainerLient container(){`

     `BlobServervicelient serviceClient = new BlobServiceClientBuilder().connectionString(Azureurl).buildClient();`

     `BlobContainerClient container = serviceClient.getBlobContainerClient(containerName);`

     `BlobContainerClient container = serviceClient.getBlobContainerClient(containerName);`

     `return container;`

     `}`