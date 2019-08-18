# administration
###### 本工具提供了中国大陆省市县镇村5个行政级别的数据，数据来源于网上，供大家使用。
###### 分成两种格式
## 第1种
###### 把所有数据放置在一张表中，表结构
CREATE TABLE `administration` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `province_id` bigint(20) unsigned NOT NULL,
  `province_name` char(64) NOT NULL,
  `city_id` bigint(20) unsigned NOT NULL,
  `city_name` char(64) NOT NULL,
  `county_id` bigint(20) unsigned NOT NULL,
  `county_name` char(64) NOT NULL,
  `town_id` bigint(20) unsigned NOT NULL,
  `town_name` char(64) NOT NULL,
  `village_id` bigint(20) unsigned NOT NULL,
  `village_name` char(64) NOT NULL,
  PRIMARY KEY (`id`),
  UNIQUE KEY `village_id` (`village_id`)
) ENGINE=InnoDB AUTO_INCREMENT=668390 DEFAULT CHARSET=utf8 COMMENT='省市县镇村数据';

## 第2种
把省、市、县、镇、村5种数据分别放在5张表中。
