# 管理员信息表结构

```sql
CREATE TABLE `zdm_admin_permission` (
  `id` bigint(20) NOT NULL DEFAULT 0 COMMENT '主键id',
  `role_id` tinyint(4) NOT NULL DEFAULT 1 COMMENT '角色id',
  `permission_id` BIGINT(20) NOT NULL DEFAULT 0 COMMENT '权限ID',
  `create_admin_id` BIGINT(20) NOT NULL DEFAULT 0 COMMENT '授权管理员',
  `create_time` bigint(20) NOT NULL DEFAULT  0  COMMENT '授权时间',
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8 COMMENT='授权信息表';
```