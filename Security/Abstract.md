### 什么是安全

- 安全是对风险的度量，安全的程度取决于发生某种风险的可能性及其造成的损失程度
- 根据风险度量，可以划分出不同等级的信任域
- 高级信任域向低级信任域流动，无需边界检查；低级信任域向高级信任域流动，需要边界检查
- 风险评估的错误，意味着信任基础的失效，也就意味上层安全方案的失效


### 安全三要素

- 机密性（不可泄露）
- 完整性（一致性、不可篡改）
- 可用性


### 设计安全方案的思路

- 划分资产等级
- 威胁分析，确定风险来源/攻击面
  + 伪装     => 认证
  + 篡改     => 完整性
  + 抵赖     => 不可抵赖性
  + 信息泄露 => 机密性
  + 拒绝服务 => 可用性
  + 僭越权限 => 权限
- 风险评估
  + 可能造成哪些破坏
  + 攻击是否容易反复发生
  + 是否容易被掌握
  + 影响范围
  + 是否容易被发现
- 设计安全方案


### 设计安全方案的手段

- 黑名单、白名单
- 最小权限原则
- 纵深防御原则
  + 体系化
  + 在正确的地方做正确的事情
- 数据与代码分离原则
- 不可预测性
  + 通过随机化，让攻击无从下手
