# 案例 5：外企 Performance Review（工程师）

> 演示外企 STAR 框架 + Impact-Driven 调性
> 场景：Senior Engineer Performance Review，某 SaaS 公司

---

## 背景信息

**Employee**：李某某，5 年经验
**当前级别**：Senior Engineer
**Review 周期**：2024 H1
**Review 场合**：与 Manager 1:1 + 跨部门 Stakeholder Review
**风格**：标准英文，STAR 框架

---

## 原始素材（用户用中文提供）

```
- 做了核心系统的重构
- 性能好了一些
- 5 个人的团队，我参与了一些核心模块
- 用 Java 和 Go
- 业务方反馈还可以
- 救过两次线上事故
- 文档写得比较全
```

---

## 标准版润色（英文）

### Self-Evaluation

#### Accomplishment 1: Core Trading System Modernization

**Situation**: Our legacy monolithic trading system was hitting scalability limits, with peak-hour latency reaching 800ms and P0 incidents occurring quarterly, directly impacting the $20M annual revenue target from high-frequency customers.

**Task**: As a senior engineer on the team, I was tasked with leading the architectural redesign of the core order-matching engine to support 5x throughput within 2 quarters.

**Action**:
- **Architected** a new event-driven microservices design, replacing the legacy monolith's order-matching module
- **Led** the end-to-end migration of 3 critical modules, coordinating with 2 cross-functional teams (Platform, SRE)
- **Drove** 12 design reviews and aligned 5 senior stakeholders on the rollout plan
- **Owned** the production rollout with feature flags and progressive delivery

**Result**:
- **Core API latency: 800ms → 120ms** (6.7x improvement)
- **System throughput: 5x increase**, sustaining 12K QPS during peak load
- **P0 incidents in the new system: 0** (vs. 3 in the legacy system the prior year)
- The new architecture was **adopted as a reference design** by 2 other product teams

**Cross-functional leadership**: Successfully aligned Platform and SRE teams on a 4-week engagement plan, turning initial pushback on the timeline into active championship.

---

#### Accomplishment 2: Production Incident Response Leadership

**Situation**: In H1, our payment service experienced 2 P1 incidents, one of which affected 200K users and risked regulatory attention.

**Task**: I was on-call and led the incident response for both events, ensuring minimal user impact and post-mortem follow-through.

**Action**:
- **Led** incident triage across 4 teams (eng, SRE, product, support) for both events
- **Drove** root cause analysis, identifying a connection pool exhaustion issue and a downstream timeout configuration
- **Championed** the implementation of 2 permanent fixes (connection pool auto-scaling, default timeout policy)
- **Owned** the post-mortem write-up, presenting findings to the engineering leadership

**Result**:
- **Mean time to recovery (MTTR): reduced from 45min to 18min** (60% improvement)
- **Both P1 incidents had zero customer-facing data loss**
- **Permanent fixes deployed**, preventing recurrence of the same root cause
- My post-mortem process was **adopted as the team's standard template**

---

#### Accomplishment 3: Engineering Excellence & Team Enablement

**Action & Result**:
- **Established** a comprehensive code review practice, increasing PR review participation from 60% to 95%
- **Wrote** 5 architecture decision records (ADRs) that became the team's reference for new system design
- **Onboarded** 3 new engineers, **reducing time-to-first-PR from 1 month to 1 week**
- **Mentored** 1 junior engineer, who **received a "Exceeds Expectations" rating in their H1 review**

---

## 关键改动说明

| 原文（用户中文） | 润色后（英文） | 武器 |
|---|---|---|
| "做了核心系统的重构" | "Architected a new event-driven microservices design" | 动词升级（参与 → Architected）|
| "性能好了一些" | "Core API latency: 800ms → 120ms (6.7x improvement)" | 数据锚定（精确化 + 量化倍数）|
| "5 个人的团队，我参与了一些核心模块" | "Led the end-to-end migration of 3 critical modules, coordinating with 2 cross-functional teams" | 动词升级（参与 → Led）|
| "用 Java 和 Go" | （删除 - 技术栈不用列，PR 里有） | 雷区规避（不要列技术栈）|
| "业务方反馈还可以" | "Successfully aligned Platform and SRE teams" | 措辞规范化 |
| "救过两次线上事故" | "Led incident triage across 4 teams... Mean time to recovery: 45min → 18min" | STAR 框架 + 数据锚定 |
| "文档写得比较全" | "Wrote 5 ADRs that became the team's reference" | 价值闭环（不只写文档，是定义标准）|

---

## 评委 / Manager 追问预案

**Q1: You said "Architected" — what was your specific role vs. the team lead's role?**
> A: I was the **technical architect** of the new system. The team lead (my manager) drove the **project management and stakeholder alignment**, while I **owned the system design, key code modules, and technical decision-making**. We had a clear RACI split.

**Q2: The 6.7x latency improvement — is that p50, p95, or p99?**
> A: p95 at peak load. The numbers are based on Grafana dashboards over a 30-day window post-launch. **I can pull the exact dashboards for our follow-up.**

**Q3: How do you know the architecture was "adopted as a reference" by 2 other teams?**
> A: I was invited to present at the **quarterly engineering architecture review** in Q2, and the Platform team referenced my ADRs in their own new system design. **I have the meeting recording and can share it.**

---

## 外企 Performance Review 的核心原则

| 原则 | 说明 |
|---|---|
| **STAR 框架** | Situation → Task → Action → Result，缺一不可 |
| **数字必须精确** | 不只 "increased"，要 "from X to Y" |
| **动词要硬** | Worked on → Led / Drove / Architected / Championed |
| **Cross-functional 视角** | 外企必问：你和谁合作？ |
| **Impact-Driven** | 每个 bullet 都要回到 "the business value" |
| **个人贡献明确** | 不要只说 "we"，要说 "I" |

---

## 5 个常见外企 PR 反例

| ❌ 反例 | ✅ 改写 |
|---|---|
| "I was involved in the project" | "I **led** the architectural redesign of X" |
| "Performance improved" | "**API latency reduced from 800ms to 120ms** (6.7x)" |
| "We used Java and Go" | （删除 - 在 GitHub 上能查）|
| "I helped the team" | "I **drove** cross-team alignment with 5 senior stakeholders" |
| "I learned a lot" | "I **built** a reusable ADR template, **adopted as team standard**" |

---

## 外企 PR 加分小技巧

1. **每个 Result 都要带 % / 倍数 / Top X**
2. **用 "adopted as a standard" 描述沉淀**
3. **用 "cross-functional" 强调推动力**
4. **结尾必须有 "Learnings" 或 "Next Steps"**（外企标配）
5. **避免政治化 / 官腔 / 集体主义过度**

---

## 一句话总结

> **外企 PR 的核心是"Impact-Driven + Personal Accountability"：**
> **不是 "我们做了 X"，是 "I drove X, delivering Y impact, scaled to Z"**
