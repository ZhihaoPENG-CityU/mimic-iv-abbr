|  --- |                  ---                                     |
|-------------------------------|------------------------------------------------------------------------------------------|
| **caregiver.csv.gz**          | **补充说明文件 --- caregiver_id**                                                           |
|                               |                                                                                          |
|                               |                                                                                          |
| **chartevents.csv.gz**        | **患者事件记录**                                                                         |
| subject_id                    | 患者的唯一标识符。                                                                       |
| hadm_id                       | 入院号，表示患者的住院标识符。                                                           |
| stay_id                       | 留观号，指患者在医院中的留观期间的唯一标识符。                                           |
| caregiver_id                  | 护理人员标识符，表示执行该记录的护理人员。                                               |
| charttime                     | 记录时间，指事件发生的时间。                                                             |
| storetime                     | 存储时间，表示记录被存储的时间。                                                         |
| itemid                        | 项目ID，指记录的特定项目或测量。                                                         |
| value                         | 表示与该项目相关的测量值或描述。                                                         |
| valuenum                      | value数字格式的相同数据/null。                                                           |
| valueuom                      | 数值单位，表示测量值的单位。                                                             |
| warning                       | 警告标志，表示是否存在与该记录相关的警告。                                               |
|                               |                                                                                          |
|                               |                                                                                          |
| **d_items.csv.gz**            |                                                                                          |
| itemid                        | 表d_item的备用主键                                                                       |
| label                         | 表明ITEMID代表的值                                                                       |
| abbreviation                  | Metavision特有，LABEL的缩写                                                              |
| linksto                       | 数据链接到的表名                                                                         |
| category                      | ITEMID对应的数据类型，如‘IV Medication’表示药物通过静脉注射                              |
| uniname                       | ITEMID表示的测量方法的单位                                                               |
| param_type                    | 描述记录的数据类型：日期，数字或文本字段                                                 |
| lownormalvalue                | 实验室测试值下限                                                                         |
| highnormalvalue               | 实验室测试值上限                                                                         |
|                               |                                                                                          |
|                               |                                                                                          |
| **datetimeevents.csv**        | **该文件记录了与日期和时间相关的事件，例如护理措施、检查和药物管理等。**                 |
| subject_id                    | 患者的唯一标识符。                                                                       |
| hadm_id                       | 入院号，表示患者的住院标识符。                                                           |
| stay_id                       | 留观号，指患者在医院中的留观期间的唯一标识符。                                           |
| caregiver_id                  | 护理人员标识符，表示执行该记录的护理人员。                                               |
| charttime                     | 记录时间，指事件发生的时间。                                                             |
| storetime                     | 存储时间，表示记录被存储的时间。                                                         |
| itemid                        | 项目ID，指记录的特定项目或测量。                                                         |
| value                         | 数值，表示与该项目相关的测量值。                                                         |
| valueuom                      | 数值单位，表示测量值的单位。                                                             |
| warning                       | 警告标志，表示是否存在与该记录相关的警告。                                               |
|                               |                                                                                          |
|                               |                                                                                          |
| **icustays.csv**              | **该文件记录了患者在重症监护室（ICU）的留观信息。**                                      |
| subject_id                    | 患者的唯一标识符。                                                                       |
| hadm_id                       | 入院号，表示患者的住院标识符。                                                           |
| stay_id                       | 留观号，指患者在医院中的留观期间的唯一标识符。                                           |
| first_careunit                | 首次护理科室，表示患者在住院期间所在的第一个护理单元。                                   |
| last_careunit                 | 最后护理科室，表示患者在住院期间所在的最后一个护理单元。                                 |
| intime                        | 入院时间，指患者入院的时间。                                                             |
| outtime                       | 出院时间，表示患者出院的时间。                                                           |
| los                           | 住院天数，表示患者在医院中的住院天数。                                                   |
|                               |                                                                                          |
|                               |                                                                                          |
| **ingredientevents.csv**      | **包含有关药物成分的数据，可能包括使用的药物成分、剂量、途径和给药时间等相关信息。**     |
| subject_id                    |  患者的唯一标识符。                                                                      |
| hadm_id                       |  入院号，表示患者的住院标识符。                                                          |
| stay_id                       |  留观号，指患者在医院中的留观期间的唯一标识符。                                          |
| caregiver_id                  |  护理人员标识符，表示执行该记录的护理人员。                                              |
| starttime                     |  开始时间，指记录事件或处理开始的时间。                                                  |
| endtime                       |  结束时间，表示记录事件或处理结束的时间。                                                |
| storetime                     |  存储时间，表示记录被存储的时间。                                                        |
| itemid                        |  项目ID，指记录的特定项目或测量。                                                        |
| amount                        |  数量，表示与该项目相关的数值量。                                                        |
| amountuom                     |  数量单位，表示数值的单位。                                                              |
| rate                          |  速率，指与该项目相关的速率值。                                                          |
| rateuom                       |  速率单位，表示速率的单位。                                                              |
| orderid                       |  医嘱ID，表示与记录相关联的医嘱标识符。                                                  |
| linkorderid                   |  链接医嘱ID，指连接到当前记录的其他医嘱的标识符。                                        |
| statusdescription             |  状态描述，表示记录的状态描述。                                                          |
| originalamount                |  原始数量，表示原始数值量。                                                              |
| originalrate                  |  原始速率，指原始速率值。                                                                |
|                               |                                                                                          |
|                               |                                                                                          |
| **inputevents.csv**           | **包含有关液体或药物输入的数据，如给药途径、剂量、速率、开始时间和结束时间等相关信息。** |
| subject_id                    |  患者的唯一标识符。                                                                      |
| hadm_id                       |  入院号，表示患者的住院标识符。                                                          |
| stay_id                       |  留观号，指患者在医院中的留观期间的唯一标识符。                                          |
| caregiver_id                  |  护理人员标识符，表示执行该记录的护理人员。                                              |
| starttime                     |  开始时间，指记录事件或处理开始的时间。                                                  |
| endtime                       |  结束时间，表示记录事件或处理结束的时间。                                                |
| storetime                     |  存储时间，表示记录被存储的时间。                                                        |
| itemid                        |  项目ID，指记录的特定项目或测量。                                                        |
| amount                        |  数量，表示与该项目相关的数值量。                                                        |
| amountuom                     |  数量单位，表示数值的单位。                                                              |
| rate                          |  速率，指与该项目相关的速率值。                                                          |
| rateuom                       |  速率单位，表示速率的单位。                                                              |
| orderid                       |  医嘱ID，表示与记录相关联的医嘱标识符。                                                  |
| linkorderid                   |  链接医嘱ID，指连接到当前记录的其他医嘱的标识符。                                        |
| ordercategoryname             |  医嘱类别名称，表示医嘱的类别名称。                                                      |
| secondaryordercategoryname    |  辅助医嘱类别名称，指医嘱的辅助类别名称。                                                |
| ordercomponenttypedescription |  医嘱组件类型描述，表示医嘱组件的类型描述。                                              |
| ordercategorydescription      |  医嘱类别描述，表示医嘱的类别描述。                                                      |
| patientweight                 |  患者体重，表示患者的体重值。                                                            |
| totalamount                   |  总数量，表示与该项目相关的总数量。                                                      |
| totalamountuom                |  总数量单位，表示总数量的单位。                                                          |
| isopenbag                     |  是否为开袋状态，指示医嘱是否处于开袋状态。                                              |
| continueinnextdept            |  是否延续至下一科室，指示医嘱是否需要延续至下一个科室。                                  |
| statusdescription             |  状态描述，表示记录的状态描述。                                                          |
| originalamount                |  原始数量，表示原始数值量。                                                              |
| originalrate                  |  原始速率，指原始速率值。                                                                |
|                               |                                                                                          |
|                               |                                                                                          |
| **outputevents.csv**          | **包含有关液体或药物输出的数据，如排尿量、引流量等相关信息。**                           |
| subject_id                    |  患者的唯一标识符。                                                                      |
| hadm_id                       |  入院号，表示患者的住院标识符。                                                          |
| stay_id                       |  留观号，指患者在医院中的留观期间的唯一标识符。                                          |
| caregiver_id                  |  护理人员标识符，表示执行该记录的护理人员。                                              |
| charttime                     |  图表时间，指记录事件或测量的时间。                                                      |
| storetime                     |  存储时间，表示记录被存储的时间。                                                        |
| itemid                        |  项目ID，指记录的特定项目或测量。                                                        |
| value                         |  值，表示与该项目相关的数值。                                                            |
| valueuom                      |  值的单位，表示数值的单位。                                                              |
|                               |                                                                                          |
|                               |                                                                                          |
| **procedureevents.csv**       | **包含有关医疗过程或手术的数据，如手术类型、开始时间和结束时间等相关信息。**             |
| subject_id                    |  患者的唯一标识符。                                                                      |
| hadm_id                       |  入院号，表示患者的住院标识符。                                                          |
| stay_id                       |  留观号，指患者在医院中的留观期间的唯一标识符。                                          |
| caregiver_id                  |  护理人员标识符，表示执行该记录的护理人员。                                              |
| starttime                     |  开始时间，指记录事件或处理开始的时间。                                                  |
| endtime                       |  结束时间，表示记录事件或处理结束的时间。                                                |
| storetime                     |  存储时间，表示记录被存储的时间。                                                        |
| itemid                        |  项目ID，指记录的特定项目或测量。                                                        |
| value                         |  值，表示与该项目相关的数值。                                                            |
| valueuom                      |  值的单位，表示数值的单位。                                                              |
| location                      |  位置，指记录事件或处理发生的位置。                                                      |
| locationcategory              |  位置类别，表示位置的类别。                                                              |
| orderid                       |  医嘱ID，表示与记录相关联的医嘱标识符。                                                  |
| linkorderid                   |  链接医嘱ID，指连接到当前记录的其他医嘱的标识符。                                        |
| ordercategoryname             |  医嘱类别名称，表示医嘱的类别名称。                                                      |
| ordercategorydescription      |  医嘱类别描述，表示医嘱的类别描述。                                                      |
| patientweight                 |  患者体重，表示患者的体重值。                                                            |
| isopenbag                     |  是否为开袋状态，指示医嘱是否处于开袋状态。                                              |
| continueinnextdept            |  是否延续至下一科室，指示医嘱是否需要延续至下一个科室。                                  |
| statusdescription             |  状态描述，表示记录的状态描述。                                                          |
| originalamount                |  原始数量，表示原始数值量。                                                              |
| originalrate                  |  原始速率，指原始速率值。                                                                |
