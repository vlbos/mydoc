1. 数据服务表
| 中文表名   | 数据服务表   |    |    | 
|:----|:----|:----|:----|
| 英文表名   |    |    |    | 
| 英文短表名   |    |    |    | 
| 表功能描述   |    |    |    | 
| 中文字段名           |   英文字段名               | 字段类型   |      字段描述    | 
| 数据服务ID    |    | 整型   |  注册id：int 从1开始自增，用于表示一类预言机服务   | 
| 服务价格   |    | 整型   |    | 
| 费用类型   |    | 整型   |  按次，月   | 
| 数据格式   | data_format   | 字符串   |  data_format：提前约定数据展现形式，比如：Jianeng2Hongyang:100   | 
| 数据类型   |    | 整型   | (确定性/非确定性) type：是指数据提者提供的数据是否允许差异   | 
| 准则   | criteria   | 字符串   | （出现时评判准则）  备注类型   | 
| 接受方式     | accept_mode     | 整型   |  数据接受规则  比例/人数   | 
| 声明    | registration_instructions   |    |    | 
| 数据注入方式    | data_injection_mode   | 整型   | 数据注入方式    链上直接，链接间接（over oracle），链外   | 
| 基础抵押金额   | basic_mortgage_amount   | 整型   | 基础抵押金额    | 
| 数据收集持续时间   |    | 整型   | 数据收集持续时间（从第一个数据提供者注入数据算起，多久后不再接受同一project_id ^update_number 的数据）duration   | 
| 数据提供者上限   |    | 整型   | 数据提供者上限（大于3） data_provider_max_namber    | 
| 数据更新周期 |    | 整型   | 数据更新周期   | 
| 数据更新开始时间 |    | 整型   | 数据更新开始时间   | 
| 风险控制金额 |    | 整型   | 风险控制金额   | 
|  冻结标记 |    | 整型   |  冻结标记   | 
| 申诉冻结期   |    | 整型   | 申诉冻结期     转账后在指定时间段内申诉有效   | 
| 超出风险控制额冻结期   |    | 整型   | 超出风险控制额冻结期   | 
| 紧急标记   |    | 整型   |    | 
| 风险担保ID   |    | 整型   |    | 
| 暂停服务抵押金额   |    | 整型   |    | 
| 状态   |    | 整型   |    | 


2. 数据使用者基本信息表
| 中文表名 | 数据使用者基本信息表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 |    |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 数据使用者ID   |    | 整型 |    | 
| 数据使用者publickey   |    | 字符串 |    | 
| 数据使用者账户   |    | 整型 |    | 
| 状态   |    | 整型 |    | 
| 创建时间   |    | 整型 |    | 


3. 数据提供者基本信息表
| 中文表名 | 数据提供者基本信息表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 |    |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 数据提供者ID   |    | 整型 |    | 
| 数据提供者账户   |    | 整型 |    | 
| 数据提供者publickey   |    | 字符串 |    | 
| 总抵押金额   |    | 整型 |    | 
| 未确认金额   |    | 整型 |    | 

4. 数据服务提供表
| 中文表名 | 数据服务提供表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 | 数据提供服务 数据提供服务商 关系表 |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 数据服务ID     |    | 整型 |    | 
| 数据提供者public key   |    | 字符串 |    | 
| 数据提供者账户   |    | 整型 |    | 
| 抵押金额   |    | 整型 |    | 
| 服务收入   |    | 整型 |    | 
| 公示信息   |    | 字符串   |    | 
| 停止服务标记   |    | 整型   |    | 


5. 数据服务使用表
| 中文表名 | 数据服务使用表   |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 | 数据提供服务 数据使用者 关系表 |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 数据服务ID    |    | 整型 |    | 
| 接收数据合约账户   |    | 整型 |    | 
| 接收数据acion名称   |    | 字符串 |    | 
| 预付款   |    | 整型 |    | 
| 消费额   |    | 整型 |    | 

6. 
7. 取消提供数据服务申请表
| 中文表名 | 取消提供数据服务申请表   |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 | 取消数据提供者资格申请表 |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 申请ID   |    | 整型 |    | 
| 数据服务ID      |    | 整型 |    | 
| 数据提供者ID   |    | 整型 |    | 
| 取消申请状态   |    | 整型 |    | 
| 取消申请时间   |    | 整型 |    | 
| 取消申请完成时间   |    | 整型   |    | 

# 
8. 数据服务请求表
| 中文表名 | 数据服务请求表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 |    |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 请求ID    |    | 整型 |    | 
| 请求数据服务ID   |    | 整型 |    | 
| 请求签名   |    | 字符串 |    | 
| 请求时间   |    | 整型 |    | 
| 请求内容   |    | 字符串 |   定义规则   | 

9. 数据服务提供记录表  
| 中文表名 | 数据服务提供记录表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 | 主要记录了数据提供者的数据状态以及证据等，用来辅助预言项目表完成预言数据交付。 |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 数据服务ID   |    | 整型 |    | 
| 数据更新序列号     | update_number   | 整型 |    | 
| 数据状态标记     | data_status_flag   | 整型 |    | 
| 具体数据json    |    | 字符串 |    | 
| 数据提供者签名    |    | 字符串 |    | 
| 更新时间   | update_time   | 整型   |    | 

10. 数据服务使用记录表
| 中文表名 | 数据服务使用记录表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 |    |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 使用ID   |    | 整型 |    | 
| 数据更新序列号   | update_number   | 整型 |    | 
| 数据使用者签名    |    | 字符串 |    | 
| 数据服务请求ID   |    | 整型 |    | 
| 使用时间   |    | 整型 |    | 

11. 申诉者表
| 中文表名 | 申诉者表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 |    |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 申诉ID |    | 整型 |    | 
| 申诉者 |    | 整型 |    | 
| 数据服务ID |    | 整型 |    | 
| 申诉时间 |    | 整型 |    | 
| 申诉状态 |    | 整型 |    | 
| 申诉原因 |    | 整型 |    | 
| 是否发起人 |    | 整型 |    | 
| 仲裁方式 |    | 整型 | 仲裁方式  大众仲裁，多轮仲裁 | 

# 
12. 职业仲裁员表   
| 中文表名 | 职业仲裁员表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 |   存储了仲裁人员的基本信息 |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 仲裁员ID   |    | 整型 |    | 
| 仲裁员账户   |    | 整型 |    | 
| 仲裁员publickey   |    | 整型 |    | 
| 仲裁员仲裁正确率   |    | 整型 |    | 
| 仲裁员抵押金额   |    | 整型 |    | 
| 仲裁员公示信息   |    | 字符串 |    | 
| 仲裁邀请次数   |    | 整型 |    | 
| 仲裁应答次数   |    | 整型 |    | 
| 仲裁员账户   |    | 整型 |    | 
| 恶意仲裁员标记   |    | 整型 |    | 
| 状态    |    | 整型   | 状态  服务中，暂停服务   | 

#   
13. 仲裁案件申请表    
| 中文表名 | 仲裁案件申请表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 | 仲裁流程的主体结构之一，其主要作用是将仲裁流程与预言流程关联，并提供仲裁框架上的支持。 |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 仲裁项ID    |    | 整型 |    | 
| 数据服务ID   |    | 整型 |    | 
| 数据更新序列号   |    | 整型 |    | 
| 仲裁阶段   |    | 整型 |    | 
| 终审结果   |    | 整型 |    | 
| 仲裁证据信息      |    | 字符串   | 仲裁证据，辩论平台信息   ipfs hash链接   | 

14. 仲裁过程记录表   
| 中文表名 | 仲裁过程记录表    |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 |  仲裁过程详细信息存储的数据表，与仲裁申请 一起完成整个仲裁过程。 |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 仲裁过程ID   |    | 整型 |    | 
| 仲裁项ID   |    | 整型 |    | 
| 仲裁次数   |    | 整型 |    | 
| 仲裁申请人列表   |    | 字符串 |    | 
| 仲裁应答方列表   |    | 字符串 |    | 
| 仲裁抵押款   |    | 整型 |    | 
| 仲裁人列表   |    | 字符串 |    | 
| 仲裁人仲裁结果列表   |    | 字符串 |    | 
| 仲裁结果   |    | 整型 |    | 
| 仲裁方式 |    | 整型 | 仲裁方式  大众仲裁，多轮仲裁 | 

15. 仲裁结果表  
| 中文表名 | 仲裁结果表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 | 辅助计算仲裁人仲裁正确率 |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 结果ID   |    | 整型 |    | 
| 仲裁员ID   |    | 整型 |    | 
| 仲裁项ID   |    | 整型 |    | 
| 仲裁人仲裁结果   |    | 整型 |    | 
| 仲裁过程记录ID   |    | 整型 |    | 

# 
16. 公正奖励表   
| 中文表名 | 公正奖励表    |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 |  在“行贿信息无条件可达”的假设下用来保存补偿仲裁员证据的表结构（当有人对仲裁员进行行贿，仲裁员只要能提供相同的证据给oracle 就可以得到相同的金额作为补偿）。 |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 数据服务ID   |    | 整型 |    | 
| 仲裁项ID   |    | 整型 |    | 
| 仲裁员证据    |    | 仲裁过程ID | 仲裁员证据  ipfs hash链接   | 

  转账冻结表 
| 中文表名 | 转账冻结表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 | 保证抵押金额恢复（当有资金被支出则数据提供者同时会有相应的抵押金被冻结，当一定时间后 抵押金将被释放） |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 冻结ID   |    | 整型 |    | 
| 数据服务ID   |    | 整型 |    | 
| 开始冻结时间   |    | 整型 |    | 
| 冻结时长   |    | 整型 |    | 
| 冻结金额   |    | 整型 |    | 
| 状态    |    | 整型   |    | 

17. 转账延迟表 
| 中文表名 | 转账延迟表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 | 保证处于风险控制中的超出担保金额部分资金延迟发放（当数据使用这所涉及的金额已经超出数据提供者的抵押金额将触发风控逻辑，进行数据的延迟发放） |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 延迟ID   |    | 整型 |    | 
| 数据服务ID   |    | 整型 |    | 
| 开始时间   |    | 整型 |    | 
| 延迟发放账户   |    | 整型 |    | 
| 延迟发放时长   |    | 整型 |    | 
| 延迟发放金额   |    | 整型 |    | 
| 状态   |    | 整型 |    | 

18. 风险担保表
| 中文表名 | 风险担保表 |    |    | 
|:----|:----|:----|
| 英文表名 |    |    |    | 
| 英文短表名 |    |    |    | 
| 表功能描述 |    |    |    | 
| 中文字段名         |   英文字段名             | 字段类型 |      字段描述  | 
| 风险担保ID |    | 整型 |    | 
| 风险担保账户 |    | 整型 |    | 
| 风险担保金额 |    | 整型 |    | 
| 风险担保时长 |    | 整型 |    | 
| 风险担保签名 |    | 字符串 |    | 




  





