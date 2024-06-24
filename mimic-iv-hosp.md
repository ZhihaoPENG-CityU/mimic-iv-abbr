|  ---                          |                  ---                                                                     |
|-------------------------------|------------------------------------------------------------------------------------------|
|                               |                                                                                          |
| **admissions.csv**            | **患者入院记录数据**   |
|                               |                                                                                          |
| **chartevents.csv.gz**        | **患者事件记录**                                                                          |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| admittime                     | 患者被接收为住院患者的日期和时间  |
| dischtime                     | 患者从医院出院的日期和时间  |
| deathtime                     | 患者在医院内死亡，则记录死亡日期和时间  |
| admission_type                | 患者被接收到医院的入院类型  |
| admit_provider_id             | 接收患者的医生或提供护理的医疗专业人员的标识符  |
| admission_location            | 患者被接收到医院的具体位置  |
| discharge_location            | 患者离开医院后的具体位置  |
| insurance                     | 患者的医疗保险类型  |
| language                      | 患者的使用语言  |
| marital_status                | 患者的婚姻状况  |
| race                          | 患者的种族或民族  |
| edregtime                     | 患者进入急诊室的日期和时间  |
| edouttime                     | 患者离开急诊室的日期和时间  |
| hospital_expire_flag          | 住院期间是否死亡的标志，1表示患者在住院期间死亡，0表示未死亡  |
|                               |                                                                                          |
|                               |                                                                                          |
| **diagnoses_icd.csv**         | **患者诊断相关的国际疾病分类（ICD）编码和描述**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| seq_num                       | 诊断在所有诊断中的顺序  |
| icd_code                      | 诊断的疾病或症状在ICD中的编码  |
| icd_version                   | 使用的ICD编码标准版本号  |
|                               |                                                                                          |
|                               |                                                                                          |
| **d_hcpcs.csv.gz,   d_icd_diagnoses.csv.gz, d_icd_procedures.csv.gz, d_labitems.csv.gz** | **补充说明文件**  |
|                               |                                                                                          |
|                               |                                                                                          |
| **drgcodes.csv**              | **用于医疗费用计算和统计分析的诊断相关组（Diagnosis Related Group）代码数据**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| drg_type                      | DRG类型 (DRG是根据患者入院诊断、手术情况、年龄、性别等因素进行分类的一种方法，用于决定医院住院费用的支付)  |
| drg_code                      | 标识具体DRG类别的代码  |
| description                   | DRG类别的描述说明  |
| drg_severity                  | DRG的严重程度，较高的数字表示更严重的疾病或手术|
| drg_mortality                 | DRG的死亡率指数，较高的数字表示更高的死亡风险|
|                               |                                                                                          |
|                               |                                                                                          |
| **emar.csv**                  | **电子药物管理记录数据**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| emar_id                       | 电子药物管理记录的标识符  |
| emar_seq                      | 电子药物管理记录的顺序号  |
| poe_id                        | 医嘱输入的标识符  |
| pharmacy_id                   | 药房的标识符  |
| enter_provider_id             | 录入提供者的标识符  |
| charttime                     | 药物管理记录的时间  |
| medication                    | 药物名称  |
| event_txt                     | 药物管理的具体情况  |
| scheduletime                  | 计划给药的时间  |
| storetime                     | 药物管理记录被存储的时间  |
|                               |                                                                                          |
|                               |                                                                                          |
| **emar_detail.csv**           | **患者药物治疗的电子药物管理记录数据**  |
| subject_id                    | 患者标识符  |
| emar_id                       | 电子药物管理记录的标识符  |
| emar_seq                      | 电子药物管理记录的顺序号  |
| parent_field_ordinal          | 标识具有父-子关系的字段之间层次结构的父字段顺序号  |
| administration_type           | 药物给予的方式  |
| pharmacy_id                   | 药房的标识符  |
| barcode_type                  | 用于扫描和识别药物的条形码类型  |
| reason_for_no_barcode         | 未使用条形码的原因  |
| complete_dose_not_given       | 完整剂量是否已给予的标志  |
| dose_due                      | 应给剂量的数量  |
| dose_due_unit                 | 应给剂量的单位  |
| dose_given                    | 实际给予剂量的数量  |
| dose_given_unit               | 实际给予剂量的单位  |
| will_remainder_of_dose_be_given  | 剩余剂量是否会继续给予的标志  |
| product_amount_given          | 实际给予的药物数量  |
| product_unit                  | 药物数量的单位  |
| product_code                  | 药物的代码  |
| product_description           | 药物的描述  |
| product_description_other     | 药物的其他描述  |
| prior_infusion_rate           | 之前的输液速率  |
| infusion_rate                 | 当前的输液速率  |
| infusion_rate_adjustment      | 输液速率调整方式  |
| infusion_rate_adjustment_amount  | 输液速率调整量  |
| infusion_rate_unit            | 输液速率的单位  |
| route                         | 给药途径  |
| infusion_complete             | 输液是否完成的标志  |
| completion_interval           | 完成间隔时间  |
| new_iv_bag_hung               | 是否更新输液袋  |
| continued_infusion_in_other_location  | 输液是否在其他位置继续进行的标志  |
| restart_interval              | 重新开始输液的间隔时间  |
| side                          | 给药侧面  |
| site                          | 给药部位  |
| non_formulary_visual_verification  | 非法定目视核对的标志  |
|                               |                                                                                          |
|                               |                                                                                          |
| **hcpcsevents.csv.gz**        | **补充说明文件**  |                               
|                               |                                                                                          |
|                               |                                                                                          |
| **labevents.csv**             | **患者实验室检测结果的数据**  |
| labevent_id                   | 实验室检查记录的标识符  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| specimen_id                   | 样本的标识符  |
| itemid                        | 检查项目的标识符  |
| order_provider_id             | 检查申请提供者的标识符  |
| charttime                     | 药物管理记录的时间  |
| storetime                     | 药物管理记录被存储的时间  |
| value                         | 检查结果值  |
| valuenum                      | 检查结果数值  |
| valueuom                      | 检查结果单位  |
| ref_range_lower               | 参考范围下限  |
| ref_range_upper               | 参考范围上限  |
| flag                          | 检查结果是否异常的标记  |
| priority                      | 检查优先级  |
| comments                      | 实验室检查结果的注释  |
|                               |                                                                                          |
|                               |                                                                                          |
| **microbiologyevents.csv**    | **微生物学检测事件数据**  |
| microevent_id                 | 微生物学事件的标识符  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| micro_specimen_id             | 微生物标本的标识符  |
| order_provider_id             | 开单医生的标识符 |
| chartdate                     | 记录日期  |
| charttime                     | 药物管理记录的时间  |
| spec_itemid                   | 标本项目的标识符   |
| spec_type_desc                | 标本类型的描述  |
| test_seq                      | 测试顺序号  |
| storedate                     | 标本的收集或储存日期  |
| storetime                     | 药物管理记录被存储的时间  |
| test_itemid                   | 测试项目的标识符  |
| test_name                     | 测试项目的名称  |
| org_itemid                    | 微生物组织的标识符  |
| org_name                      | 微生物组织的名称  |
| isolate_num                   | 不同微生物分离的编号  |
| quantity                      | 微生物的数量  |
| ab_itemid                     | 抗生素项目的标识符  |
| ab_name                       | 抗生素的名称  |
| dilution_text                 | 抗生素的稀释程度  |
| dilution_comparison           | 用于比较抗生素的稀释程度  |
| dilution_value                | 抗生素的稀释倍数  |
| interpretation                | 对测试结果的解释或诊断  |
| comments                      | 其他相关信息的备注  |
|                               |                                                                                          |
|                               |                                                                                          |
| **omr.csv.gz**                | **身高/体重/血压/BMI等测量值**  |
|                               |                                                                                          |
|                               |                                                                                          |
| **patients.csv.gz**           | **病人信息**  |
| subject_id                    | 患者标识符  |
| gender                        | 性别  |
| anchor_age                    | 匿名化处理的年龄  |
| anchor_year                   | 匿名化处理的年份（患者的真实年龄=anchor_age+admittime-anchor_year）  |
| anchor_year_group             | 匿名化处理的年龄区间  |
| dod                           | 死亡时间（1- read.csv("mimic_time.csv")； 2- survival_time =difftime(dmy(data$dod),date(dmy_hms(data$outtime)),units = "days"); 3- survival_time = as.numeric(data$survival_time)  |
|                               |                                                                                          |
|                               |                                                                                          |
| **pharmacy.csv**              | **药房数据，可能包含有关药品配送、管理和库存方面的信息**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| pharmacy_id                   | 药房的标识符  |
| poe_id                        | 医嘱输入的标识符  |
| starttime                     | 医生开药的时间  |
| stoptime                      | 医生停药的时间  |
| medication                    | 药物名称  |
| proc_type                     | 医生的处理方式  |
| status                        | 药物发放/管理员授权的状态  |
| entertime                     | 药物进入药房的时间  |
| verifiedtime                  | 验证药物信息的时间  |
| route                         | 药物的给药方式  |
| frequency                     | 药物的给药频率  |
| disp_sched                    | 药物的分配计划  |
| infusion_type                 | 静脉注射药物的类型  |
| sliding_scale                 | 血糖和胰岛素之间的滑动比例  |
| lockout_interval              | 注射药物的锁定时间间隔  |
| basal_rate                    | 基注射药物的基础速率  |
| one_hr_max                    | 药物的一小时最大剂量  |
| doses_per_24_hrs              | 药物的每24小时的使用次数  |
| duration                      | 药物的持续使用时间  |
| duration_interval             | 药物的持续使用时间间隔  |
| expiration_value              | 药物过期时间的值  |
| expiration_unit               | 药物过期时间的单位  |
| expirationdate                | 药物的过期日期  |
| dispensation                  | 药房完成配药的记录  |
| fill_quantity                 | 药房填充药物的数量  |
|                               |                                                                                          |
|                               |                                                                                          |
| **poe.csv**                   | **医生对患者的医嘱输入数据**  |
| poe_id                        | 医嘱输入的标识符  |
| poe_seq                       | 医嘱在医嘱组中的序列号  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| ordertime                     | 医嘱被下达的时间  |
| order_type                    | 医嘱的类型  |
| order_subtype                 | 医嘱的子类型  |
| transaction_type              | 医嘱相关的交易类型  |
| discontinue_of_poe_id         | 终止医嘱所属的原始医嘱ID  |
| discontinued_by_poe_id        | 执行终止操作的医嘱ID  |
| order_provider_id             | 下达医嘱医生的标识符  |
| order_status                  | 医嘱的当前状态  |
|                               |                                                                                          |
|                               |                                                                                          |
| **poe_detail.csv**            | **医嘱输入的详细数据**  |
| poe_id                        | 医嘱输入的标识符  |
| poe_seq                       | 医嘱在医嘱组中的序列号  |
| subject_id                    | 患者标识符  |
| field_name                    | 医嘱属性的名称  |
| field_value                   | 医嘱属性的值  |
|                               |                                                                                          |
|                               |                                                                                          |
| **prescriptions.csv**         | **对患者开具处方药物的数据**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| pharmacy_id                   | 药房的标识符  |
| poe_id                        | 医嘱输入的标识符  |
| poe_seq                       | 医嘱在医嘱组中的序列号  |
| order_provider_id             | 下达医嘱医生的标识符  |
| starttime                     | 医生开药的时间  |
| stoptime                      | 医生停药的时间  |
| drug_type                     | 药物类型  |
| drug                          | 药物的名称  |
| formulary_drug_cd             | 药物在药物目录中的代码  |
| gsn                           | 用于标识药物的全球服务网络码（Global Service Network Code）  |
| ndc                           | 用于唯一标识药物的国家药物编码（National Drug Code）  |
| prod_strength                 | 药物的剂量强度  |
| form_rx                       | 表示药物制剂形式的处方剂型  |
| dose_val_rx                   | 处方剂量的数值  |
| dose_unit_rx                  | 处方剂量的单位  |
| form_val_disp                 | 实际发放剂量的数值  |
| form_unit_disp                | 实际发放剂量的单位  |
| doses_per_24_hrs              | 药物的每24小时的使用次数  |
| route                         | 药物的给药方式  |
|                               |                                                                                          |
|                               |                                                                                          |
| **procedures_icd.csv**        | **患者手术或医疗过程相关的ICD编码和描述**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| seq_num                       | 诊断在所有诊断中的顺序  |
| chartdate                     | 记录日期  |
| icd_code                      | 诊断的疾病或症状在ICD中的编码  |
| icd_version                   | 使用的ICD编码标准版本号  |
|                               |                                                                                          |
|                               |                                                                                          |
| **provider.csv.gz**           | **provider_id补充说明文件**  |
|                               |                                                                                          |
|                               |                                                                                          |
| **services.csv**              | **患者接受医疗服务的数据**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| transfertime                  | 患者从一个服务部门转到另一个服务部门的时间  |
| prev_service                  | 患者转诊前所在的服务部门  |
| curr_service                  | 患者转诊后所在的服务部门  |
|  *Info*                       | *CMED：心血管内科治疗，心血管疾病的保守治疗； CSURG：心血管外科治疗，心血管疾病的手术治疗； DENT：牙齿/颌骨相关的牙科治疗； ENT：主要治疗耳鼻喉相关区域的耳鼻喉科治疗； GU：泌尿生殖器治疗，泌尿系统和生殖系统； GYN：妇科治疗，女性生殖系统和乳房等； MED：泛指内科相关治疗； NB：新生儿服务，主要指院内出生的； NBB：新生婴儿服务，主要指院内出生的； NMED：神经内科治疗，与脑相关的非手术治疗； NSURG：神经外科治疗，与脑相关的手术治疗； OBS：产科，产妇分娩及护理； ORTHO：骨科外科治疗，主要为涉及骨骼肌肉系统的手术； OMED：骨科治疗，主要为涉及骨骼肌肉系统内科保守治疗； PSURG：整形治疗，主要为人体的修复或重建（包括以美容或美学为目的的）； PSYCH：精神卫生治疗，主要指与情绪、行为、认知或认知相关的精神障碍； SURG：普外科治疗，主要指无法进行专科分类的手术种类； TRAUM：创伤外科治疗，由外来物理因素造成的身体伤害或损坏； TSURG：胸外科治疗，主要指腹部及颈部之间的胸部手术； VSURG：血管外科治疗，主要指与循环系统相关手术*|
|                               |                                                                                          |
|                               |                                                                                          |
| **transfers.csv**             | **患者转院的数据**  |
| subject_id                    | 患者标识符  |
| hadm_id                       | 患者的住院标识符  |
| transfer_id                   | 部门转移记录在该患者所有部门转移记录中的序号  |
| eventtype                     | 部门转移记录类型  |
| careunit                      | 患者所在病房的名称  |
| intime                        | 患者入住病房的时间  |
| outtime                       | 患者出院的时间  |
|                               |                                                                                          |
| **Reference**                 |                                                                                          |
|[R] MIMIC-III Clinical Database, PhysioNet | https://physionet.org/content/mimiciii/1.4/                                  |
|[R] MIMIC-IV, PhysioNet                    | https://physionet.org/content/mimiciv/2.2/icu/#files-panel                   |
|[R] Tencent                                | https://cloud.tencent.com/developer/article/2359852                          |
|                               |                                                                                          |
