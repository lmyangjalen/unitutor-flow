# 在腾讯 WorkBuddy 用成真正的家教助手

[腾讯 WorkBuddy 官网](https://www.workbuddy.cn/) · [官方 Skill 使用说明](https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Skills-Market) · [官方专家使用说明](https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Expert-Center)

## 三个部件
1. 本仓库 `SKILL.md`：工作规则，不是存储数据库。
2. WorkBuddy 的**专家**：用来扮演 UniTutor 家教助理，接受你随口描述的任务。
3. 获授权的**私人文件工作区**：保存每个学生的长期档案、课次记录、讲义、应计和收款台账，才有可能下次自动接续。

## 首次配置
1. 在 GitHub 仓库点击 `Code → Download ZIP`，解压出包含 SKILL.md 的目录。
2. WorkBuddy 进入“专家·技能·连接器”中的“技能”，选择添加/导入本地技能包；按当前版本实际界面操作，并确认导入内容受信任。若无法直接导入 ZIP，可选择解压后的 Skill 目录或让 WorkBuddy 根据 SKILL.md 创建技能。
3. 新建一个仅用于家教的**私人工作目录**，只授权 WorkBuddy 对该目录读写，不授权整块磁盘。按 [数据模型](references/student-data-model.md) 创建子目录，将 [老师档案](templates/tutor-background.md) 填入私有工作区。不要把真实学生记录复制回公开 GitHub。
4. 可选：在“我的专家 → 创建专家”中设置角色：UniTutor Flow 大学生家教助手，擅长接单评估、个性化备课、家长沟通、上课总结、结算、下一课和长期记录；将本 Skill 的规则用于专家，具体关联方式依版本而定。
5. 用虚构数据验证读写：建 T001 档案、上一次试课、再说“按上节课继续备课”，检查是否真的读取和写入不同文件。
6. 每次上完课让它完成“六项课后闭环”，核对生成的 Word/PDF、结算表和下一课计划。若未真写入则不能称为保存。

## 分享/商业化
WorkBuddy 官方允许创建并分享专家的链接，接受者获得专家副本；分享不等于自动上架市场、也不等于自动具备收费入口。想上架专家/技能市场需要遵守开放平台规则；收费需要另行确认产品商业条款和模型成本，不能仅因为把 Skill 放到市场就假设可以赚钱。

优先验证：真实家教是否用得上、持续记录是否稳定、是否真正生成文件、隐私和学生隔离是否足够。付费差异可以来自账户化私有学生管理、长期记录同步、批量讲义与阶段报告等持续服务，而不仅是卖一个公开 SKILL.md。
