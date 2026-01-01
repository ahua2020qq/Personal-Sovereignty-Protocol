\# Core Principles (PRINCIPLES.md)



\## Preamble



This document outlines the foundational design and development principles of the Personal Sovereignty Protocol (PSP). These principles serve as our \*\*constitution\*\*—guiding every technical decision, implementation detail, and the evolution of the project. Any significant deviation requires open discussion and consensus within the community.



\## 1. Sovereignty by Default



\*   \*\*Statement\*\*: Data, computational tasks, and control over intelligent models must, by architectural default, reside with the end-user. The system's primary state of operation is within the user's controlled local environment.

\*   \*\*Practical Implication\*\*: The architecture is \*\*"offline-first"\*\*. Any operation requiring data or computation to leave the user's direct control (e.g., cloud collaboration) must require \*\*explicit, informed, and revocable consent\*\* from the user via a clear user interface \[1](@ref).



\## 2. Privacy as a First Principle



\*   \*\*Statement\*\*: Privacy is not an optional feature but a core architectural component. Protecting user data from unauthorized access and misuse is the highest priority.

\*   \*\*Practical Implication\*\*: Employ \*\*end-to-end encryption\*\* by default. Actively explore and integrate Privacy-Enhancing Technologies (PETs) like \*\*Zero-Knowledge Proofs (ZKPs)\*\* to enable "verifiable but invisible" trust. Data collection follows the principle of minimization \[4](@ref).



\## 3. Transparency and Verifiability



\*   \*\*Statement\*\*: The system must be a "glass box," not a "black box." Key processes, such as an agent's decision logic and data flow, must be auditable and explainable.

\*   \*\*Practical Implication\*\*: Core code must be open-source. The use of verifiable computation credentials is encouraged, allowing users or third parties to audit the execution and results of critical operations \[2](@ref).



\## 4. Keep It Simple, Stupid (KISS)



\*   \*\*Statement\*\*: Everything should be made as simple as possible, but no simpler. Simplicity leads to usability, understandability, and maintainability.

\*   \*\*Practical Implication\*\*: Write code that is concise, elegant, and appropriately abstracted. Avoid unnecessary complexity. A good question to ask is, "What is the simplest thing that could possibly work?" \[1,4](@ref).



\## 5. Don't Repeat Yourself (DRY)



\*   \*\*Statement\*\*: Every piece of knowledge or logic must have a single, unambiguous representation within a system.

\*   \*\*Practical Implication\*\*: Avoid duplicate code. Extract common functionality into shared methods, libraries, or services. Prolific duplication signifies a lack of design and abstraction, leading to code that is bloated, less clear, and harder to maintain \[1](@ref).



\## 6. You Aren't Gonna Need It (YAGNI)



\*   \*\*Statement\*\*: Do not add functionality until it is necessary.

\*   \*\*Practical Implication\*\*: Avoid over-engineering and speculative "future-proofing." Focus on meeting current requirements in the cleanest way possible. Implement extension points only when they are rationally anticipated from clear needs, not because they \*might\* be useful someday \[1,4](@ref).



\## 7. High Cohesion \& Loose Coupling



\*   \*\*Statement\*\*: Modules within the system should have high internal cohesion (elements within a module are strongly related) and be loosely coupled (modules have minimal dependencies on each other).

\*   \*\*Practical Implication\*\*: This leads to a system that is more resilient to change, easier to test, and simpler to maintain. A change in one module should have minimal impact on others \[2](@ref).



\## 8. Program to an Interface, Not an Implementation



\*   \*\*Statement\*\*: Depend on abstractions (interfaces) rather than concrete implementations.

\*   \*\*Practical Implication\*\*: This reduces interdependencies between modules. In practice, this means defining clear APIs and contracts between components, which facilitates swapping implementations and makes the system more flexible and testable \[1](@ref).



\## 9. Progressive Sovereignty \& Pragmatism



\*   \*\*Statement\*\*: We value "shipping over perfection." In resource-constrained real-world scenarios, we accept pragmatic transitional solutions \*with the user's informed consent\*, but we must clearly articulate the trade-offs and risks and remain committed to iterative progress toward the ideal of full sovereignty.

\*   \*\*Practical Implication\*\*: The system should clearly indicate the security and privacy level of a current operation. Architecture design should reserve space for a smooth future transition from hybrid models to a fully offline model \[4](@ref).



---

\*These principles are the stars by which we navigate, not the shackles that bind us. They ensure that as we explore the unknown seas of technology, we never lose sight of our true north: defending individual dignity and autonomy.\*



\# 核心原则 (Core Principles)



本文档阐述了个人主权协议（PSP）在设计、实现与应用中必须遵循的核心原则。这些原则是本项目的\*\*宪法\*\*，任何偏离都必须经过社区的公开辩论与批准。



\## 1. 主权默认原则 (Sovereignty by Default)

\*   \*\*阐述\*\*：在技术架构上，\*\*数据、计算与智能模型的控制权必须默认归属于终端用户\*\*。系统的默认状态应是在用户完全掌控的本地环境中运行。

\*   \*\*技术体现\*\*：

&nbsp;   \*   “离线优先”是架构设计的出发点。

&nbsp;   \*   任何需要将数据或计算任务移交至用户控制范围之外的行为（如云端协同），必须提供明确的用户界面，获得用户的\*\*显式、知情同意\*\*，并可被随时撤销。



\## 2. 隐私第一原则 (Privacy as the First Principle)

\*   \*\*阐述\*\*：隐私不是附加功能，而是系统的\*\*基础架构\*\*。保护用户数据不被未授权访问和滥用，是设计的最高优先级。

\*   \*\*技术体现\*\*：

&nbsp;   \*   采用\*\*端到端加密\*\*技术。

&nbsp;   \*   积极探索和集成\*\*零知识证明（ZKPs）\*\* 等隐私增强技术，实现“可验证但不可见”的信任。

&nbsp;   \*   数据收集遵循最小化原则。



\## 3. 透明可信原则 (Transparency and Verifiability)

\*   \*\*阐述\*\*：系统必须是“透明的玻璃盒”，而非“神秘的黑箱”。关键流程，如智能体的决策逻辑、数据的流向，必须可审计、可解释。

\*   \*\*技术体现\*\*：

&nbsp;   \*   核心代码必须开源。

&nbsp;   \*   鼓励使用可验证的计算凭证，允许用户或第三方审计关键操作的执行过程与结果。



\## 4. 可互操作性与自由迁移 (Interoperability and Free Migration)

\*   \*\*阐述\*\*：防止新的“主权花园”垄断。用户必须能够自由地将其数字身份、数据资产及信誉在不同支持PSP的服务之间迁移，而不受任何单一供应商的锁定。

\*   \*\*技术体现\*\*：

&nbsp;   \*   采纳和贡献于开放标准（如W3C DID、可验证凭证等）。

&nbsp;   \*   确保数据格式和API接口的开放性。



\## 5. 渐进式主权与务实精神 (Progressive Sovereignty and Pragmatism)

\*   \*\*阐述\*\*：我们认同“完成比完美重要”。在资源受限的现实条件下，允许在\*\*用户知情且同意\*\*的前提下，采用务实的过渡方案（如使用受信任的云端计算资源），但必须明确其代价与风险，并致力于向完全主权的目标持续迭代。

\*   \*\*技术体现\*\*：

&nbsp;   \*   系统应能明确告知用户当前操作的安全与隐私级别。

&nbsp;   \*   架构设计应为未来从混合模式向完全离线模式的平滑过渡留出空间。



---

\*这些原则是我们航行的星辰，而非束缚我们的枷锁。它们确保我们在探索未知的技术海域时，永不偏离“捍卫个体尊严”的北极星。\*

