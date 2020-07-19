# 网络安全攻防·蓝队清单

> 在网络安全攻防蓝队方向的一些很酷的资源、工具和一些小玩意～

[网络安全（攻防）蓝队](https://en.wikipedia.org/wiki/Blue_team_(computer_security))是由一群能够识别信息技术系统中安全缺陷的人组成。他们能够验证安全防护措施的有效性，并且能持续监控系统并确保已采用的安全防御措施。  
尽管没有偏见，但这个列表更倾向于[自由软件](https://www.gnu.org/philosophy/free-sw.html)项目，而不是商业的产品和服务。  
关于攻防对抗的TTPs（战术、技术和过程），请查看这个项目：[awesome-pentest](https://github.com/fabacab/awesome-pentest).  

你的贡献和建议十分重要，欢迎来参与(✿◕‿◕)。请查看[贡献准则](CONTRIBUTING.md)来获取更多的信息。本项目是在[Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/)许可下进行的。

## 内容列表

//TODO，内容翻译结束后再进行

- [自动化工具](#自动化工具)
  - 代码库和绑定工具
- 安全管理、自动化和响应（SOAR）


## 自动化工具

### 杂乱的

- [Ansible Lockdown](https://ansiblelockdown.io/) - 以信息安全为主题的Ansible（运维工具）规则集合。经过精心地审核，并且维护积极。
- [Clevis](https://github.com/latchset/clevis) - 
对于自动解密的可插入式工具，经常被用做[Tang](https://github.com/latchset/tang)客户端。
- [DShell](https://github.com/USArmyResearchLab/Dshell) - 用Python编写网络取证分析框架，支持扩展，可快速开发插件来分析捕获的网络数据包。
- [Dev-Sec.io](https://dev-sec.io/) - 服务器增强框架，提供各种基准安全配置的Ansible，Chef和Puppet实现。
- [peepdf](https://eternal-todo.com/tools/peepdf-pdf-analysis-tool) - 支持脚本编写的PDF文件分析器。

### 代码库和绑定

- [MultiScanner](https://github.com/mitre/multiscanner) - 使用Python编写的文件分析框架，支持自动运行相关的工具，汇总输出帮助评估一组带分析的文件。
- [Posh-VirusTotal](https://github.com/darkoperator/Posh-VirusTotal) - 可与VirusTotal.com的API进行交互的PowerShell接口。
- [censys-python](https://github.com/censys/censys-python) - Python wrapper to the Censys REST API.
对Censys REST API的Python轻量级封装
- [libcrafter](https://github.com/pellegre/libcrafter) - High level C++ network packet sniffing and crafting library.
一个c++的高级库，用于创建和解码网络数据包。
- [python-dshield](https://github.com/rshipp/python-dshield) - 连接SANS ISC/DShiel API的Python接口。补充：SANS ISC是一个全球性的安全事件响应组织，为所有的Internet用户和组织提供免费的互联网攻击分析和预警服务。
- [python-sandboxapi](https://github.com/InQuest/python-sandboxapi) - 用于构建恶意软件沙箱集成的最小型、并且长期有效的的Python API。
- [python-stix2](https://github.com/oasis-open/cti-python-stix2) - 用于序列化和反序列化STIX（JSON形式）的Python API，以及一些用于常见任务的高级API。补充：STIX是用来交换威胁情报的一种语言和序列化格式，由MITRE联合DHS（美国国土安全部）发布。

### 安全编排自动化与响应（SOAR）

请另行查阅[Security Information and Event Management (SIEM)](#security-information-and-event-management-siem)，和[IR management consoles](#ir-management-consoles).

- [Shuffle](https://shuffler.io/) - Graphical generalized workflow (automation) builder for IT professionals and blue teamers.
用于IT专家和蓝队成员的图形化工作流（自动化）生成器。

## 云平台安全

另请参阅[asecure.cloud/tools](https://asecure.cloud/tools/).

- [Checkov](https://www.checkov.io/) - 对于Terraform（在DevOps实践中，代码即基础设施概念）的静态分析器。可以帮助检测CIS策略违规行为，并防止云安全策略配置错误。
    - 补充：Terraform是一种安全有效地构建、更改和版本控制基础设施的工具(基础架构自动化的编排工具)。[1]
    - 补充：[CIS](https://www.cisecurity.org/cis-benchmarks/)基准是安全配置系统的配置基线和最佳做法。[2]
- [Falco](https://falco.org/) - 行为活动监视器，旨在通过审核Linux内核和运行时数据（例如Kubernetes指标）进行拓展和丰富，以检测容器化的应用程序，以及主机和网络数据包流中的异常活动。
- [Istio](https://istio.io/) - Open platform for providing a uniform way to integrate microservices, manage traffic flow across microservices, enforce policies and aggregate telemetry data.提供统一的方式的开放平台，可以集成微服务，管理跨微服务的流量，执行策略和汇总遥测数据。
- [Kata Containers](https://katacontainers.io/) - 使用轻量级虚拟机来保护容器的运行时，这些虚拟机的情况和性能类似于容器，但是使用硬件虚拟化技术作为第二层防御，可以提供更强的工作负载隔离。
- [Managed Kubernetes Inspection Tool (MKIT)](https://github.com/darkbitio/mkit) - 可提供查询和验证托管Kubernetes群集对象以及群集内运行的工作负载/资源的几种与安全性相关的常见设置。
- [Prowler](https://github.com/toniblyx/prowler) -基于AWS-CLI命令的工具，用于Amazon Web Services帐户安全性评估和增强。
- [Scout Suite](https://github.com/nccgroup/ScoutSuite) - 开源的多云安全审核工具，可用于评估云环境的安全状态。
    - 补充：Muticloud，多云，是指在单个异构架构中使用多个[云计算](https://en.wikipedia.org/wiki/Cloud_computing)和[存储](https://en.wikipedia.org/wiki/Cloud_storage)服务。
- [gVisor](https://github.com/google/gvisor) - 用Go编写的应用程序内核，它实现Linux系统表面的很大一部分，用以在应用程序和主机内核之间提供隔离边界。






## References

[1] Terraform：简介，sparkdev，https://www.cnblogs.com/sparkdev/p/10052310.html
[2] Internet 安全中心 (CIS) 基准, [Robert Mazzoli](https://github.com/robmazz)，https://docs.microsoft.com/zh-cn/microsoft-365/compliance/offering-cis-benchmark?view=o365-worldwide