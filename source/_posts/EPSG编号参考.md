---
title: EPSG编号参考
date: 2021-07-22 20:53:52
tags: [学习, GIS]
---

## 空间坐标系对应EPSG编号

**WKT**(Well-known  text)是一种文本标记语言，用于表示矢量几何对象、空间参照系统及空间参照系统之间的转换。它的二进制表示方式，亦即WKB(well-known  binary)则胜于在传输和在数据库中存储相同的信息。该格式由开放地理空间联盟(OGC)制定。

**WKB**(well-known binary) 是WKT的二进制表示形式，解决了WKT表达方式冗余的问题，便于传输和在数据库中存储相同的信息。

**GeoJSON** 一种JSON格式的Feature信息输出格式，它便于被JavaScript等脚本语言处理，OpenLayers等地理库便是采用GeoJSON格式。此外，TopoJSON等更精简的扩展格式。

**SRID**空间参考标识符 是与特定坐标系、容差和分辨率关联的唯一标识符。RID 的填充方式及其所示含义取决于存储数据所用的数据库。目前有多种公认的标准 SRID，例如欧洲石油测绘组 (EPSG) 定义的 SRID。

**WKID**（Well-known  ID）空间参考的ID，常用语ArcGIS二次开发中。表示不同空间参考所对应的ID，例如WKID=4214表示GCS_Beijing_1954这种空间参考，4326代表WGS 84投影。我们常用到的、与中国相关的只有一百多个坐标参考，具体如下表所示：

![img](https://www.pianshen.com/images/467/2c6af49489cd9f4adb03bdbd237403fb.jpg)

Geographic Coordinate System 地理坐标

| **WKID** | **Geographic Coordinate System 地理坐标** |
| -------- | ----------------------------------------- |
| 4214     | GCS_Beijing_1954                          |
| 4326     | GCS_WGS_1984                              |
| 4490     | GCS_China_Geodetic_Coordinate_System_2000 |
| 4555     | GCS_New_Beijing                           |
| 4610     | GCS_Xian_1980                             |

- Projected Coordinate System 投影坐标

| EPSG | 投影坐标系名称                           | 经度最小 | 经度最大 | 中央经线 | 备注   |
| ---- | ---------------------------------------- | -------- | -------- | -------- | ------ |
| 4513 | CGCS2000 / 3-degree Gauss-Kruger zone 25 | 73.5     | 76.5     | 75       | 加代号 |
| 4514 | CGCS2000 / 3-degree Gauss-Kruger zone 26 | 76.5     | 79.5     | 78       | 加代号 |
| 4515 | CGCS2000 / 3-degree Gauss-Kruger zone 27 | 79.5     | 82.5     | 81       | 加代号 |
| 4516 | CGCS2000 / 3-degree Gauss-Kruger zone 28 | 82.5     | 85.5     | 84       | 加代号 |
| 4517 | CGCS2000 / 3-degree Gauss-Kruger zone 29 | 85.5     | 88.5     | 87       | 加代号 |
| 4518 | CGCS2000 / 3-degree Gauss-Kruger zone 30 | 88.5     | 91.5     | 90       | 加代号 |
| 4519 | CGCS2000 / 3-degree Gauss-Kruger zone 31 | 91.5     | 94.5     | 93       | 加代号 |
| 4520 | CGCS2000 / 3-degree Gauss-Kruger zone 32 | 94.5     | 97.5     | 96       | 加代号 |
| 4521 | CGCS2000 / 3-degree Gauss-Kruger zone 33 | 97.5     | 100.5    | 99       | 加代号 |
| 4522 | CGCS2000 / 3-degree Gauss-Kruger zone 34 | 100.5    | 103.5    | 102      | 加代号 |
| 4523 | CGCS2000 / 3-degree Gauss-Kruger zone 35 | 103.5    | 106.5    | 105      | 加代号 |
| 4524 | CGCS2000 / 3-degree Gauss-Kruger zone 36 | 106.5    | 109.5    | 108      | 加代号 |
| 4525 | CGCS2000 / 3-degree Gauss-Kruger zone 37 | 109.5    | 112.5    | 111      | 加代号 |
| 4526 | CGCS2000 / 3-degree Gauss-Kruger zone 38 | 112.5    | 115.5    | 114      | 加代号 |
| 4527 | CGCS2000 / 3-degree Gauss-Kruger zone 39 | 115.5    | 118.5    | 117      | 加代号 |
| 4528 | CGCS2000 / 3-degree Gauss-Kruger zone 40 | 118.5    | 121.5    | 120      | 加代号 |
| 4529 | CGCS2000 / 3-degree Gauss-Kruger zone 41 | 121.5    | 124.5    | 123      | 加代号 |
| 4530 | CGCS2000 / 3-degree Gauss-Kruger zone 42 | 124.5    | 127.5    | 126      | 加代号 |
| 4531 | CGCS2000 / 3-degree Gauss-Kruger zone 43 | 127.5    | 130.5    | 129      | 加代号 |
| 4532 | CGCS2000 / 3-degree Gauss-Kruger zone 44 | 130.5    | 133.5    | 132      | 加代号 |
| 4533 | CGCS2000 / 3-degree Gauss-Kruger zone 45 | 133.5    | 136.5    | 135      | 加代号 |
| 4534 | CGCS2000 / 3-degree Gauss-Kruger CM 75E  | 73.5     | 76.5     | 75       |        |
| 4535 | CGCS2000 / 3-degree Gauss-Kruger CM 78E  | 76.5     | 79.5     | 78       |        |
| 4536 | CGCS2000 / 3-degree Gauss-Kruger CM 81E  | 79.5     | 82.5     | 81       |        |
| 4537 | CGCS2000 / 3-degree Gauss-Kruger CM 84E  | 82.5     | 85.5     | 84       |        |
| 4538 | CGCS2000 / 3-degree Gauss-Kruger CM 87E  | 85.5     | 88.5     | 87       |        |
| 4539 | CGCS2000 / 3-degree Gauss-Kruger CM 90E  | 88.5     | 91.5     | 90       |        |
| 4540 | CGCS2000 / 3-degree Gauss-Kruger CM 93E  | 91.5     | 94.5     | 93       |        |
| 4541 | CGCS2000 / 3-degree Gauss-Kruger CM 96E  | 94.5     | 97.5     | 96       |        |
| 4542 | CGCS2000 / 3-degree Gauss-Kruger CM 99E  | 97.5     | 100.5    | 99       |        |
| 4543 | CGCS2000 / 3-degree Gauss-Kruger CM 102E | 100.5    | 103.5    | 102      |        |
| 4544 | CGCS2000 / 3-degree Gauss-Kruger CM 105E | 103.5    | 106.5    | 105      |        |
| 4545 | CGCS2000 / 3-degree Gauss-Kruger CM 108E | 106.5    | 109.5    | 108      |        |
| 4546 | CGCS2000 / 3-degree Gauss-Kruger CM 111E | 109.5    | 112.5    | 111      |        |
| 4547 | CGCS2000 / 3-degree Gauss-Kruger CM 114E | 112.5    | 115.5    | 114      |        |
| 4548 | CGCS2000 / 3-degree Gauss-Kruger CM 117E | 115.5    | 118.5    | 117      |        |
| 4549 | CGCS2000 / 3-degree Gauss-Kruger CM 120E | 118.5    | 121.5    | 120      |        |
| 4550 | CGCS2000 / 3-degree Gauss-Kruger CM 123E | 121.5    | 124.5    | 123      |        |
| 4551 | CGCS2000 / 3-degree Gauss-Kruger CM 126E | 124.5    | 127.5    | 126      |        |
| 4552 | CGCS2000 / 3-degree Gauss-Kruger CM 129E | 127.5    | 130.5    | 129      |        |
| 4553 | CGCS2000 / 3-degree Gauss-Kruger CM 132E | 130.5    | 133.5    | 132      |        |
| 4554 | CGCS2000 / 3-degree Gauss-Kruger CM 135E | 133.5    | 136.5    | 135      |        |
| 2401 | Beijing_1954_3_Degree_GK_Zone_25         | 73.5     | 76.5     | 75       | 加代号 |
| 2402 | Beijing_1954_3_Degree_GK_Zone_26         | 76.5     | 79.5     | 78       | 加代号 |
| 2403 | Beijing_1954_3_Degree_GK_Zone_27         | 79.5     | 82.5     | 81       | 加代号 |
| 2404 | Beijing_1954_3_Degree_GK_Zone_28         | 82.5     | 85.5     | 84       | 加代号 |
| 2405 | Beijing_1954_3_Degree_GK_Zone_29         | 85.5     | 88.5     | 87       | 加代号 |
| 2406 | Beijing_1954_3_Degree_GK_Zone_30         | 88.5     | 91.5     | 90       | 加代号 |
| 2407 | Beijing_1954_3_Degree_GK_Zone_31         | 91.5     | 94.5     | 93       | 加代号 |
| 2408 | Beijing_1954_3_Degree_GK_Zone_32         | 94.5     | 97.5     | 96       | 加代号 |
| 2409 | Beijing_1954_3_Degree_GK_Zone_33         | 97.5     | 100.5    | 99       | 加代号 |
| 2410 | Beijing_1954_3_Degree_GK_Zone_34         | 100.5    | 103.5    | 102      | 加代号 |
| 2411 | Beijing_1954_3_Degree_GK_Zone_35         | 103.5    | 106.5    | 105      | 加代号 |
| 2412 | Beijing_1954_3_Degree_GK_Zone_36         | 106.5    | 109.5    | 108      | 加代号 |
| 2413 | Beijing_1954_3_Degree_GK_Zone_37         | 109.5    | 112.5    | 111      | 加代号 |
| 2414 | Beijing_1954_3_Degree_GK_Zone_38         | 112.5    | 115.5    | 114      | 加代号 |
| 2415 | Beijing_1954_3_Degree_GK_Zone_39         | 115.5    | 118.5    | 117      | 加代号 |
| 2416 | Beijing_1954_3_Degree_GK_Zone_40         | 118.5    | 121.5    | 120      | 加代号 |
| 2417 | Beijing_1954_3_Degree_GK_Zone_41         | 121.5    | 124.5    | 123      | 加代号 |
| 2418 | Beijing_1954_3_Degree_GK_Zone_42         | 124.5    | 127.5    | 126      | 加代号 |
| 2419 | Beijing_1954_3_Degree_GK_Zone_43         | 127.5    | 130.5    | 129      | 加代号 |
| 2420 | Beijing_1954_3_Degree_GK_Zone_44         | 130.5    | 133.5    | 132      | 加代号 |
| 2421 | Beijing_1954_3_Degree_GK_Zone_45         | 133.5    | 136.5    | 135      | 加代号 |
| 2422 | Beijing_1954_3_Degree_GK_CM_75E          | 73.5     | 76.5     | 75       |        |
| 2423 | Beijing_1954_3_Degree_GK_CM_78E          | 76.5     | 79.5     | 78       |        |
| 2424 | Beijing_1954_3_Degree_GK_CM_81E          | 79.5     | 82.5     | 81       |        |
| 2425 | Beijing_1954_3_Degree_GK_CM_84E          | 82.5     | 85.5     | 84       |        |
| 2426 | Beijing_1954_3_Degree_GK_CM_87E          | 85.5     | 88.5     | 87       |        |
| 2427 | Beijing_1954_3_Degree_GK_CM_90E          | 88.5     | 91.5     | 90       |        |
| 2428 | Beijing_1954_3_Degree_GK_CM_93E          | 91.5     | 94.5     | 93       |        |
| 2429 | Beijing_1954_3_Degree_GK_CM_96E          | 94.5     | 97.5     | 96       |        |
| 2430 | Beijing_1954_3_Degree_GK_CM_99E          | 97.5     | 100.5    | 99       |        |
| 2431 | Beijing_1954_3_Degree_GK_CM_102E         | 100.5    | 103.5    | 102      |        |
| 2432 | Beijing_1954_3_Degree_GK_CM_105E         | 103.5    | 106.5    | 105      |        |
| 2433 | Beijing_1954_3_Degree_GK_CM_108E         | 106.5    | 109.5    | 108      |        |
| 2434 | Beijing_1954_3_Degree_GK_CM_111E         | 109.5    | 112.5    | 111      |        |
| 2435 | Beijing_1954_3_Degree_GK_CM_114E         | 112.5    | 115.5    | 114      |        |
| 2436 | Beijing_1954_3_Degree_GK_CM_117E         | 115.5    | 118.5    | 117      |        |
| 2437 | Beijing_1954_3_Degree_GK_CM_120E         | 118.5    | 124.5    | 120      |        |
| 2438 | Beijing_1954_3_Degree_GK_CM_123E         | 121.5    | 121.5    | 123      |        |
| 2439 | Beijing_1954_3_Degree_GK_CM_126E         | 124.5    | 127.5    | 126      |        |
| 2440 | Beijing_1954_3_Degree_GK_CM_129E         | 127.5    | 130.5    | 129      |        |
| 2441 | Beijing_1954_3_Degree_GK_CM_132E         | 130.5    | 133.5    | 132      |        |
| 2442 | Beijing_1954_3_Degree_GK_CM_135E         | 133.5    | 136.5    | 135      |        |
| 2349 | Xian_1980_3_Degree_GK_Zone_25            | 73.5     | 76.5     | 75       | 加代号 |
| 2350 | Xian_1980_3_Degree_GK_Zone_26            | 76.5     | 79.5     | 78       | 加代号 |
| 2351 | Xian_1980_3_Degree_GK_Zone_27            | 79.5     | 82.5     | 81       | 加代号 |
| 2352 | Xian_1980_3_Degree_GK_Zone_28            | 82.5     | 85.5     | 84       | 加代号 |
| 2353 | Xian_1980_3_Degree_GK_Zone_29            | 85.5     | 88.5     | 87       | 加代号 |
| 2354 | Xian_1980_3_Degree_GK_Zone_30            | 88.5     | 91.5     | 90       | 加代号 |
| 2355 | Xian_1980_3_Degree_GK_Zone_31            | 91.5     | 94.5     | 93       | 加代号 |
| 2356 | Xian_1980_3_Degree_GK_Zone_32            | 94.5     | 97.5     | 96       | 加代号 |
| 2357 | Xian_1980_3_Degree_GK_Zone_33            | 97.5     | 100.5    | 99       | 加代号 |
| 2358 | Xian_1980_3_Degree_GK_Zone_34            | 100.5    | 103.5    | 102      | 加代号 |
| 2359 | Xian_1980_3_Degree_GK_Zone_35            | 103.5    | 106.5    | 105      | 加代号 |
| 2360 | Xian_1980_3_Degree_GK_Zone_36            | 106.5    | 109.5    | 108      | 加代号 |
| 2361 | Xian_1980_3_Degree_GK_Zone_37            | 109.5    | 112.5    | 111      | 加代号 |
| 2362 | Xian_1980_3_Degree_GK_Zone_38            | 112.5    | 115.5    | 114      | 加代号 |
| 2363 | Xian_1980_3_Degree_GK_Zone_39            | 115.5    | 118.5    | 117      | 加代号 |
| 2364 | Xian_1980_3_Degree_GK_Zone_40            | 118.5    | 121.5    | 120      | 加代号 |
| 2365 | Xian_1980_3_Degree_GK_Zone_41            | 121.5    | 124.5    | 123      | 加代号 |
| 2366 | Xian_1980_3_Degree_GK_Zone_42            | 124.5    | 127.5    | 126      | 加代号 |
| 2367 | Xian_1980_3_Degree_GK_Zone_43            | 127.5    | 130.5    | 129      | 加代号 |
| 2368 | Xian_1980_3_Degree_GK_Zone_44            | 130.5    | 133.5    | 132      | 加代号 |
| 2369 | Xian_1980_3_Degree_GK_Zone_45            | 133.5    | 136.5    | 135      | 加代号 |
| 2370 | Xian_1980_3_Degree_GK_CM_75E             | 73.5     | 76.5     | 75       |        |
| 2371 | Xian_1980_3_Degree_GK_CM_78E             | 76.5     | 79.5     | 78       |        |
| 2372 | Xian_1980_3_Degree_GK_CM_81E             | 79.5     | 82.5     | 81       |        |
| 2373 | Xian_1980_3_Degree_GK_CM_84E             | 82.5     | 85.5     | 84       |        |
| 2374 | Xian_1980_3_Degree_GK_CM_87E             | 85.5     | 88.5     | 87       |        |
| 2375 | Xian_1980_3_Degree_GK_CM_90E             | 88.5     | 91.5     | 90       |        |
| 2376 | Xian_1980_3_Degree_GK_CM_93E             | 91.5     | 94.5     | 93       |        |
| 2377 | Xian_1980_3_Degree_GK_CM_96E             | 94.5     | 97.5     | 96       |        |
| 2378 | Xian_1980_3_Degree_GK_CM_99E             | 97.5     | 100.5    | 99       |        |
| 2379 | Xian_1980_3_Degree_GK_CM_102E            | 100.5    | 103.5    | 102      |        |
| 2380 | Xian_1980_3_Degree_GK_CM_105E            | 103.5    | 106.5    | 105      |        |
| 2381 | Xian_1980_3_Degree_GK_CM_108E            | 106.5    | 109.5    | 108      |        |
| 2382 | Xian_1980_3_Degree_GK_CM_111E            | 109.5    | 112.5    | 111      |        |
| 2383 | Xian_1980_3_Degree_GK_CM_114E            | 112.5    | 115.5    | 114      |        |
| 2384 | Xian_1980_3_Degree_GK_CM_117E            | 115.5    | 118.5    | 117      |        |
| 2385 | Xian_1980_3_Degree_GK_CM_120E            | 118.5    | 121.5    | 120      |        |
| 2386 | Xian_1980_3_Degree_GK_CM_123E            | 121.5    | 124.5    | 123      |        |
| 2387 | Xian_1980_3_Degree_GK_CM_126E            | 124.5    | 127.5    | 126      |        |
| 2388 | Xian_1980_3_Degree_GK_CM_129E            | 127.5    | 130.5    | 129      |        |
| 2389 | Xian_1980_3_Degree_GK_CM_132E            | 130.5    | 133.5    | 132      |        |
| 2390 | Xian_1980_3_Degree_GK_CM_135E            | 133.5    | 136.5    | 135      |        |

高斯-克吕格3度带与6度带投影图

![img](https://www.pianshen.com/images/492/efbee108895c64e5fccbca2926b5026c.JPEG)



原文链接：https://www.pianshen.com/article/1836888579/

