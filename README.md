# johannesburg vps：真实价格、实测延迟，以及 Vultr 的按小时计费固定费率方案如何胜过大多数本地月度报价

搜索 "johannesburg vps" 的用户通常有三个非常具体的问题：将服务器托管在南非的实际成本是多少？约翰内斯堡是否真的是正确的区域？以及哪家服务商能提供最佳价值？以下是简短回答：入门级定价从每月约 4 美元到 15 美元不等，具体取决于服务商；如果您的受众在南非（或在南半球的其他地方），约翰内斯堡是正确的选择；而 Vultr 是最具灵活性的选择——因为它以与纽约或阿姆斯特丹相同的固定价格提供约翰内斯堡区域，且按小时计费，无合同限制。

在少数几个例外情况下，专注于本地的服务商是更好的选择，本文也将涵盖这些情况。此外，还有延迟表、真实的年度成本，以及一份简短的部署指南。

> **时间紧迫？** 对于大多数希望服务南非用户的人来说，Vultr 的约翰内斯堡区域是合理的默认选择：1 vCPU / 1 GB / 25 GB SSD 的规格，含 1 TB 流量，每月 **$5**——这与它在其他每个区域的价格相同，且您可以按小时使用。👉 [Check Vultr's Johannesburg pricing](https://www.vultr.com/pricing/?ref=7268283)。如果您特别需要仅限加密货币且无需 KYC 的注册，OnionVPS 和 CrestVPS 等约翰内斯堡专家更适合——详细信息见下文。

## 约翰内斯堡甚至是否是您服务器的正确区域？

如果您的用户在南非或邻国，是的。如果他们在西欧、西非或南美，答案会复杂一些——将流量终端设在约翰内斯堡需要与您的用户位置匹配，而不是与地图匹配。

约翰内斯堡之所以成为自然选择，是因为它正是非洲互联网连接的地方。NAPAfrica 是该大陆最大的互联网交换中心，拥有超过 800 Gbps 的峰值流量，而 JINX 则增加了较旧的国内网络。由于在 NAPAfrica 上的对等互连（peering）是免费的（settlement-free），传递给南非 ISP 的流量成本很低且速度很快——这也是为什么约翰内斯堡大都市区的往返时间（round-trip time）能保持在个位数毫秒的原因。

### 从约翰内斯堡出发的实际延迟期望

这些数据来自几个专注于约翰内斯堡的服务商所公布的测量和中间数据（measured and median figures）。它们彼此一致，因此您可以将它们视为真实数据，而非最佳情况：

| 目的地 | 从约翰内斯堡出发的典型 RTT |
| --- | --- |
| 约翰内斯堡大都市区（桑顿、兰德堡） | 2–8 ms |
| 德班 | ~11 ms |
| 开普敦 | 18–24 ms |
| 温得和克 | ~12 ms |
| 马普托 | 8–19 ms |
| 卢萨卡 / 哈拉雷 | 21–25 ms |
| 哈博罗内 | ~37 ms |
| 内罗毕 | 49–62 ms |
| 拉各斯 | 68–70 ms |
| 迪拜 | ~118 ms |
| 伦敦 | 148–173 ms |
| 法兰克福 | ~119–180 ms |

从这些数据中可以清楚地看出两点。首先，欧洲到约翰内斯堡的往返时间在 150 ms 左右——这就是为什么从欧洲服务器服务南非用户会导致页面加载缓慢、VoIP 通话中断以及游戏体验无法进行的原因。其次，如果您的大多数用户在尼日利亚或加纳，拉各斯服务器的延迟约为约翰内斯堡服务器的三分之一。按用户所在位置选择您的区域。

### POPIA 以及数据驻留问题

南非的《个人信息保护法》（POPIA）由信息监管机构（Information Regulator）执行。它适用于从国内处理的任何个人数据，并且带有违规通知义务。如果这是您的顾虑，托管在约翰内斯堡会将数据保存在南非境内，大多数供应商会为您提供支持 POPIA 合规所需的文档。拥有南非客户并需要提供本地发票或增值税（VAT）会计的南非企业，通常也更倾向于使用本地公司——这也是稍后对比表格中的一个关键考量因素。

## Vultr 的约翰内斯堡方案：完整价格表

Vultr 维护一份全球统一价格表：约翰内斯堡实例的定价与纽约、阿姆斯特丹或东京相同。一些竞争对手会提高约翰内斯堡的价格（CrestVPS 将其定价为基准清单的 118%），而 Vultr 根本没有进行任何区域指数化调整。实际上，这意味着每月 $5 是约翰内斯堡云服务器的入门价格——对于该城市而言，这是目前被广泛宣传的最低报价。

存在一个注意事项：Vultr 最小的共享方案（512 MB RAM，每月 $2.50）仅在少数几个区域提供，约翰内斯堡不在其中。实际上，计划以 1 GB 方案起步。

### 云计算 — 常规性能（Cloud Compute – Regular Performance）

共享 vCPU，SSD 存储，适合网站、机器人（bots）、VPN 端点、游戏服务器和一般工作负载：

| 方案 | vCPU / RAM | 存储 | 传输量 | 每月 |  |
| --- | --- | --- | --- | --- | --- |
| Regular 1 GB | 1 / 1 GB | 25 GB SSD | 1 TB | $5 | [Deploy 1 GB](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| Regular 2 GB | 1 / 2 GB | 55 GB SSD | 2 TB | $10 | [Deploy 2 GB](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| Regular 4 GB | 2 / 4 GB | 80 GB SSD | 3 TB | $20 | [Deploy 4 GB](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| Regular 8 GB | 4 / 8 GB | 160 GB SSD | 4 TB | $40 | [Deploy 8 GB](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| Regular 16 GB | 6 / 16 GB | 320 GB SSD | 5 TB | $80 | [Deploy 16 GB](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| Regular 32 GB | 8 / 32 GB | 640 GB SSD | 6 TB | $160 | [Deploy 32 GB](https://www.vultr.com/products/cloud-compute/?ref=7268283) |

阶梯式定价持续到 16 vCPU / 64 GB（每月 $320）、24 vCPU / 96 GB（每月 $640）和 32 vCPU / 128 GB（每月 $1,280）的节点。

### 云计算 — 高性能（Cloud Compute – High Performance）

新一代硬件，采用 NVMe 存储和更快的单核性能。值得为数据库、电商和任何延迟敏感的应用多支付每月 $1 的费用：

| 方案 | vCPU / RAM | 存储 | 传输量 | 每月 |  |
| --- | --- | --- | --- | --- | --- |
| High Performance 1 GB | 1 / 1 GB | 25 GB NVMe | 1 TB | $6 | [Deploy 1 GB HP](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| High Performance 2 GB | 1 / 2 GB | 55 GB NVMe | 2 TB | $12 | [Deploy 2 GB HP](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| High Performance 4 GB | 2 / 4 GB | 80 GB NVMe | 3 TB | $24 | [Deploy 4 GB HP](https://www.vultr.com/products/cloud-compute/?ref=7268283) |
| High Performance 8 GB | 4 / 8 GB | 160 GB NVMe | 4 TB | $48 | [Deploy 8 GB HP](https://www.vultr.com/products/cloud-compute/?ref=7268283) |

16 GB 和 32 GB 的版本分别为每月 $96 和 $192。

### 如果您需要独占内核怎么办

Vultr 的 Optimized Cloud Compute 系列增加了独占 vCPU 方案，起价为 **每月 $28**（1 个独占 vCPU、2 GB RAM、32 GB NVMe、1 TB 传输量）。独占内核裸机服务器也可以从同一个约翰内斯堡区域部署。👉 [See Vultr's dedicated-core options for Johannesburg](https://www.vultr.com/products/optimized-cloud-compute/?ref=7268283)。

### 每个方案都包含的内容

每个实例都可以选择 Ubuntu、Debian、Rocky、AlmaLinux、FreeBSD 和 Windows Server，外加自定义 ISO 上传、原生 IPv6、防火墙组、快照（snapshots）、启动脚本以及完整的 API 和 CLI。自动备份增加约 20% 的实例价格；Windows 镜像需支付额外的许可费；可选的 DDoS 保护是一项付费附加服务。新账户附带可在前 30 天使用的 **$300** 试用额度，这足以在付款前实际运行一个约翰内斯堡服务器一个月。

## 约翰内斯堡 VPS 的实际成本

标价只是故事的一半。以下是 Vultr 约翰内斯堡方案的账单实际运作方式。

计费是按小时的，上限为月度费率。$5 的方案每小时大约 0.75 美分——每月 672 小时，您最多只需支付 $5。如果运行两周后将其销毁，您大约只需支付 $2.50。这是它与列表中其他所有服务商的核心区别，因为其他服务商都是按月计费且通常不支持退款：当 Hostiger 的计算方案在激活时预留，因此不支持退款，而 Vebloom 的方案按月提前收费时，Vultr 让您可以先使用后支付。

> 在约翰内斯堡部署一个 $6 的高性能实例，从您自己的用户那里 ping 一天，然后销毁它。该实验的总成本为 15–20 美分，这是任何月度合同供应商都无法复制的。

带宽超额费用为每 GB 约 1 美分，仅计算出站流量——入站是免费的。如果 $5 的方案超出了 1 TB 的额度 500 GB，您需要支付约 $5 的额外费用。对于正常访问量的网站，这很少会成为问题。

第二个因素没有出现在任何营销页面上：续费价格。Vultr 没有首次期限折扣，因此没有续费冲击。$5 的方案第一年成本为 $60，第二年也是 $60。相比之下，如果 Vebloom 的 $14.99 方案保持其承诺的续费价格，一年为 $179.88，而 CrestVPS 的 EdgeAfrica 方案年付享受 −30% 折扣后为每月 €4.87，随后恢复到 €6.96。👉 [Open Vultr's current plan list and compare the math yourself](https://www.vultr.com/pricing/?ref=7268283)。

## Vultr 与约翰内斯堡首选供应商的对比

这里有一个坦率的视角来看待这篇文章为什么存在。几家规模较小的服务商专门在约翰内斯堡运营，它们在某些方面做得更好。以下是经过验证的情况：

| 供应商 | 入门价格 | 入门规格 | 计费方式 | 值得了解 |
| --- | --- | --- | --- | --- |
| Vultr | $5/mo | 1 vCPU, 1 GB, 25 GB SSD, 1 TB | 按小时 | 所有区域统一价格；$300 试用额度 |
| OnionVPS | $4/mo | 首个列出的方案（2 GB, 40 GB NVMe, 3 TB）为 $6.65 | 按月 | 仅限加密货币，无 KYC，40 Gbit/s 上行 |
| CrestVPS | €6.96/mo | "EdgeAfrica" 线路，AMD Ryzen 9 7950X | 按月或按年（年付 −30%） | 约翰内斯堡价格为基准的 118%；仅限加密货币 |
| Randhost | €9.50/mo (excl. VAT) | 云 VPS，10 Gbps | 按月 | 首张发票 5 折；NAPAfrica 对等互连 |
| Hostiger | $10/mo | NVMe Gen4，1 Gbps 不限流量 | 按小时 | Tier-1 传输（Cogent, Lumen, GTT, Telia） |
| Vebloom | $14.99/mo | 1 核, 1 GB, 25 GB NVMe, 1 TB | 按月 | 续费价格锁定；19 个地区规格相同 |

对手方视角。如果您因为不想将姓名或卡片与服务器绑定而需要仅限加密货币支付和无需 KYC 的注册，OnionVPS 和 CrestVPS 正是专门做这个的——Vultr 接受卡和 PayPal，并非匿名。如果您想要一家可以开具南非增值税（VAT）发票并在您所在时区工作的本地公司，Randhost 或 Vebloom 更适合。而对于约翰内斯堡的雷竞技（Ryzen）专用线路，CrestVPS 的硬件阵容（包括 Ryzen 9 9950X 方案）比 Vultr 在该市公开列出的任何产品都更具针对性。

Vultr 胜出的地方在于价格和灵活性。没有其他列出的服务商能以更低的价格为约翰内斯堡提供 1 TB 流量的实例，且按小时计费、快照、API 和一键迁移到其他 31 个区域等额外功能是较小竞争对手难以匹配的。当一家单一区域服务商发生故障时，您的约翰内斯堡工作负载可以以相同的价格迁移到开普敦、圣保罗或法兰克福。

## 在 Vultr 上部署约翰内斯堡 VPS

从开始到拥有 SSH 访问权限大约需要五分钟：

1. **创建一个账户** — 邮箱、密码，使用卡或 PayPal 付款。$300 的试用额度会自动应用。
2. **打开部署页面** 并选择 *Cloud Compute*，然后选择 *Regular Performance* 或 *High Performance*。
3. **选择约翰内斯堡** 作为位置。方案列表和价格与您之前看到的一致。
4. **选择操作系统** — Ubuntu、Debian、Rocky、AlmaLinux、FreeBSD、Windows Server 或自定义 ISO。粘贴 SSH 公钥以实现免密码 root 登录。
5. **添加额外功能**（如果需要）— 原生 IPv6、自动备份、DDoS 保护、防火墙组 — 然后进行部署。配置在大约一分钟内完成，计费从当分钟开始按小时计算。

一个实用提示：配置一个 $6 的实例，从约翰内斯堡、德班和开普敦的用户那里运行 traceroute，并将数字与上面的表格进行对比。如果您自己的线路表现明显更差，请在第一个月结束前将其销毁，然后查看供应商的对等互连设置——但基于图表所示，这种情况不太可能发生。

## 常见问题

**Vultr 的约翰内斯堡区域定价是否与其美国或欧洲区域不同？**
不。Vultr 对每个区域的所有云计算方案收取相同费用，约翰内斯堡也不例外。上面 $5 的常规方案和 $6 的高性能方案是相同的全球价格。

**在承诺长期使用前，我可以测试延迟吗？**
可以——这就是按小时计费的意义。在几周内以每小时不到一美分的价格运行一个实例，从您的真实用户那里收集数据，然后保留或销毁它。您的费用最高仅为每月费率的一小部分。

**约翰内斯堡 VPS 的 POPIA 合规性如何？**
您的数据物理上保存在南非，因此 POPIA 的处理条件和违规通知义务将按原样适用。如果您处理的是来自南非个人的个人数据，这通常就是您所希望的；向您的服务商索取合规文档以放入您自己的记录中。

**我可以在 Vultr 上使用加密货币支付吗？**
Vultr 接受主要的银行卡和 PayPal。如果加密货币支付是硬性要求，OnionVPS（每月 $4 起）和 CrestVPS（每月 €6.96 起）都在约翰内斯堡运营仅限加密货币的账单，无需 KYC——这是它们相对于 Vultr 的核心优势。

**每个方案包含多少流量？** 在 $5–$6 的入门级方案上包含 1 TB 出站流量，随方案规模增加，最高可达 6 TB 以上。超额费用约为每 GB 1 美分，入站流量免费。

## 简短版本

根据您的实际情况进行选择。如果您的用户在南非，且您希望以最低的价格获得最大的灵活性，Vultr 的约翰内斯堡区域是显而易见的起点——$5 共享或 $6 高性能，按小时计费，且可在使用前测试。如果您需要独占内核，Vultr 的 Optimized 系列从每月 $28 起，或者您可以从 CrestVPS 或 Randhost 购买本地专用线路。如果匿名性和加密货币支付是不可妥协的，OnionVPS 是首选。如果您想运行 Windows 且希望由当地供应商计费，Vebloom 会明确宣传南非的 Windows VPS。👉 [Deploy your Johannesburg VPS on Vultr](https://bit.ly/VulTR) ——以每小时大约 0.75 美分的价格，您在阅读完本文所需时间内所消耗的额度几乎无法察觉。
