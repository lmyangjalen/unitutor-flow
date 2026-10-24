# 外部档案与内部事件结构

每名学生一个独立**私有**工作区，例：
```
private-workspace/
├── tutor-profile.md                  # 老师自身优势、时间和接单条件
└── students/
    └── T001/
        ├── profile.md                # 外部学生/家长档案
        ├── sessions.md               # 内部课堂事件，按时间追加
        ├── communications.md         # 每次与家长沟通的变化
        ├── billing.csv               # 真实课时、计费、到期与收款状态
        ├── next-lesson.md            # 下一课资料和准备
        └── materials/                # 教案、学生讲义、教师答案
```

- **外部/低频**：学生编号、年级科目教材、基线证据、兴趣和具体课堂行为（事实/猜测分开）；家长明确的目标与沟通偏好；费率、单课时长、频率、约定结算周期、区域级地点、单程交通时间与成本；家庭可参与的合理学习安排。学生档案会随新证据改变。
- **内部/高频**：每次日期、实际课时、教材、独立和提示后正确情况、错因、作业、学生反馈、沟通、结算、下节课安排。按时间追加，保留来源和修改原因。
- **billing.csv 推荐列**：`session_id,date,actual_hours,rate_per_hour,accrued_amount,due_date,status,received_amount,paid_at,notes`。status 使用 `unknown,not_due,due,partial,paid,waived`，不能把“应计”写成“已付”。
- **权限**：只有 AI 确实获准读写该私人目录时才能承诺保存；否则只输出可复制文本。核对学生编号，绝不串档。保留最少必要数据，不把真实学生身份、精确地址或付款资料放入公开 GitHub。
