|  --- |                  ---                                     |
|-------------------------------|------------------------------------------------------------------------------------------|
| **caregiver.csv.gz**          | **补充说明文件 --- caregiver_id**   |
|                               |                                                                                          |
|                               |                                                                                          |
| **chartevents.csv.gz**        | **患者事件记录**                                                                          |
| subject_id                    | 患者标识符  |
| hadm_id                       | 入院号，患者的住院标识符  |
| stay_id                       | 留观号，患者留院观察的标识符  |
| caregiver_id                  | 执行该记录护理人员的标识符  |
| charttime                     | 事件发生的时间  |
| storetime                     | 记录被存储的时间  |
| itemid                        | 记录的检测项目或特定项目的标识符  |
| value                         | 检测项目的测量值或描述  |
| valuenum                      | 数字格式数据或空值  |
| valueuom                      | 检测值的数值单位  |
| warning                       | 警告标志，表示是否存在与该记录相关的警告  |
|                               ||
|                               ||
| **d_items.csv.gz**            | 检测相关的数据说明  |
| itemid                        | 检测数据的标识符  |
| label                         | itemid的值  |
| abbreviation                  |label的缩写（Metavision特有）|
| linksto                       | 链接的表名  |
| category                      | itemid对应的数据类型  |
| uniname                       | itemid测量方法的单位  |
| param_type                    | 记录的数据类型  |
| lownormalvalue                | 实验室测试值下限  |
| highnormalvalue               | 实验室测试值上限  |
|                               |                                                                                          |
|                               |                                                                                          |
| **datetimeevents.csv**        | **与日期和时间相关的事件，如护理措施、检查和药物管理等**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 入院号，患者的住院标识符  |
| stay_id                       | 留观号，患者留院观察的标识符  |
| caregiver_id                  | 执行该记录护理人员的标识符  |
| charttime                     | 事件发生的时间  |
| storetime                     | 记录被存储的时间  |
| itemid                        | 记录的检测项目或特定项目的标识符  |
| value                         | 检测项目的测量值或描述  |
| valueuom                      | 检测值的数值单位  |
| warning                       | 警告标志，表示是否存在与该记录相关的警告  |
|                               |                                                                                          |
|                               |                                                                                          |
| **icustays.csv**              | **患者在重症监护室的留院观察信息**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 入院号，患者的住院标识符  |
| stay_id                       | 留观号，患者留院观察的标识符  |
| first_careunit                | 患者在住院期间所在的第一个护理单元  |
| last_careunit                 | 患者在住院期间所在的最后一个护理单元  |
| intime                        | 患者入院时间  |
| outtime                       | 患者出院的时间  |
| los                           | 患者在医院中的住院天数  |
|                               |                                                                                          |
|                               |                                                                                          |
| **ingredientevents.csv**      | **使用的药物成分、剂量、途径和给药时间等相关信息**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 入院号，患者的住院标识符  |
| stay_id                       | 留观号，患者留院观察的标识符  |
| caregiver_id                  | 执行该记录护理人员的标识符  |
| starttime                     | 事件开始的时间  |
| endtime                       | 事件结束的时间  |
| storetime                     | 记录被存储的时间  |
| itemid                        | 记录的检测项目或特定项目的标识符  |
| amount                        | 项目相关的数值量  |
| amountuom                     | 数值单位  |
| rate                          | 项目相关的速率值  |
| rateuom                       | 速率单位  |
| orderid                       | 与记录相关联的医嘱标识符  |
| linkorderid                   | 连接到当前记录的其他医嘱的标识符  |
| statusdescription             | 记录的状态描述  |
| originalamount                | 原始数值量  |
| originalrate                  | 始速率值  |
|                               |                                                                                          |
|                               |                                                                                          |
| **inputevents.csv**           | **给药途径、剂量、速率、开始时间和结束时间等液体或药物输入的数据** |
| subject_id                    | 患者标识符  |
| hadm_id                       | 入院号，患者的住院标识符  |
| stay_id                       | 留观号，患者留院观察的标识符  |
| caregiver_id                  | 执行该记录护理人员的标识符  |
| starttime                     | 事件开始的时间  |
| endtime                       | 事件结束的时间  |
| storetime                     | 记录被存储的时间  |
| itemid                        | 记录的检测项目或特定项目的标识符  |
| amount                        | 项目相关的数值量  |
| amountuom                     | 数值单位  |
| rate                          | 项目相关的速率值  |
| rateuom                       | 速率单位  |
| orderid                       | 与记录相关联的医嘱标识符  |
| linkorderid                   | 连接到当前记录的其他医嘱的标识符  |
| ordercategoryname             |  医嘱的类别名称  |
| secondaryordercategoryname    |  医嘱的辅助类别名称  |
| ordercomponenttypedescription |  医嘱组件的类型描述  |
| ordercategorydescription      |  医嘱的类别描述  |
| patientweight                 |  患者体重  |
| totalamount                   |  输入项目相关的总数量  |
| totalamountuom                |  总数量的单位  |
| isopenbag                     |  医嘱是否处于开袋状态  |
| continueinnextdept            |  医嘱是否需要延续至下一个科室  |
| statusdescription             | 记录的状态描述  |
| originalamount                | 原始数值量  |
| originalrate                  | 始速率值  |
|                               |                                                                                          |
|                               |                                                                                          |
| **outputevents.csv**          | **排尿量、引流量等液体或药物输出的数据**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 入院号，患者的住院标识符  |
| stay_id                       | 留观号，患者留院观察的标识符  |
| caregiver_id                  | 执行该记录护理人员的标识符  |
| charttime                     | 事件发生的时间  |
| storetime                     | 记录被存储的时间  |
| itemid                        | 记录的检测项目或特定项目的标识符  |
| value                         | 检测项目的测量值或描述  |
| valueuom                      | 检测值的数值单位  |
|                               |                                                                                          |
|                               |                                                                                          |
| **procedureevents.csv**       | **包含有关医疗过程或手术的数据，如手术类型、开始时间和结束时间等相关信息。**             |
| subject_id                    | 患者标识符  |
| hadm_id                       | 入院号，患者的住院标识符  |
| stay_id                       | 留观号，患者留院观察的标识符  |
| caregiver_id                  | 执行该记录护理人员的标识符  |
| starttime                     | 事件开始的时间  |
| endtime                       | 事件结束的时间  |
| storetime                     | 记录被存储的时间  |
| itemid                        | 记录的检测项目或特定项目的标识符  |
| value                         | 检测项目的测量值或描述  |
| valueuom                      | 检测值的数值单位  |
| location                      |  事件发生的位置  |
| locationcategory              |  位置的类别  |
| orderid                       | 与记录相关联的医嘱标识符  |
| linkorderid                   | 连接到当前记录的其他医嘱的标识符  |
| ordercategoryname             |  医嘱的类别名称  |
| ordercategorydescription      |  医嘱的类别描述  |
| patientweight                 |  患者体重  |
| isopenbag                     |  医嘱是否处于开袋状态  |
| continueinnextdept            |  医嘱是否需要延续至下一个科室  |
| statusdescription             | 记录的状态描述  |
| originalamount                | 原始数值量  |
| originalrate                  | 始速率值  |
