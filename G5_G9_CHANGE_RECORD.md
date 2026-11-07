# G5/G9 产品修改记录

- 产品编号：$(@{number=65; product_id=JLZ-EDU-SK-053; chinese_name=转介绍沟通文案; english_name=Referral Communication Copy; repository_name=edu-referral-communication-copy; repository_url=https://github.com/jinlize-tech/edu-referral-communication-copy; product_type=Skill; category_code=05; category=05 家校服务中心; description=家长转介绍沟通内容。; target_users=System.Object[]; core_input=老生情况、转介绍对象、课程价值、关系阶段、奖励规则和沟通渠道; main_output=转介绍沟通文案、场景版本、跟进节奏、合规提醒和效果记录字段; product_risk=诱导性承诺、泄露其他家长信息或忽略奖励规则; dedup_label=无明显重复; dedup_note=与老带新活动策划区别：本产品只生成沟通内容和跟进节奏，不设计整体机制。; development_status=Planned / 待研发; license=Apache-2.0; spec_version=1.0.0; workbuddy_status=PLANNED_FOR_WORKBUDDY}.product_id)
- 产品名称：转介绍沟通文案
- 基线：EDUCATION_BASELINE_V1.0.0
- 基线提交：$BaselineCommit
- 原版本：1.0.0
- 新版本：1.0.1

## 本次修改

1. 强化产品专属执行流程、输入核对和输出验收规则。
2. 新增 scripts/validate_input.js，实际检查必填字段、冲突、未确认数据和敏感信息。
3. 新增正常、缺失、冲突、敏感信息和非法JSON场景输入。
4. 测试升级为 T1–T7 分层并保存逐项检查结果。
5. 安装包加入 Apache-2.0 LICENSE 和 THIRD_PARTY_NOTICES.md。
6. 安装包升级为 1.0.1，加入许可证、第三方声明和输入校验脚本，保留 1.0.0 ZIP。
7. 按本产品冻结规格补充专属处理规则、输入到成果的核对矩阵和去重边界。

## 产品专属增强

- 核心任务：家长转介绍沟通内容。
- 主要风险：诱导性承诺、泄露其他家长信息或忽略奖励规则
- 去重边界：与老带新活动策划区别：本产品只生成沟通内容和跟进节奏，不设计整体机制。

- 先确认事实、涉及对象、沟通目的、渠道、时间要求和必须披露的信息。
- 给家长或学生的结论必须区分事实、观察、建议和待核实内容。
- 只披露与该家庭直接相关且确有必要的学生信息，避免交叉泄露。
- 投诉、退款、安全和健康事项设置人工升级条件，不替代正式处置。

## 运行边界

- 本地模型行为：NOT_RUNTIME_VERIFIED
- WorkBuddy平台验证：WORKBUDDY_VALIDATION_NOT_IN_SCOPE
- 本轮不执行上传、安装、审核或正式发布。
