# dubbo-chaosMonkey
随机在线服务超时、网络故障模拟、服务重定向、资源限制等等

Chaos Monkey，可以随机关闭生产环境中的实例，确保网站系统能够经受故障的考验，同时不会影响客户的正常使用。
Latency Monkey，在服务的调用中引入人为的延时来模拟服务降级，测量上游服务是否会做出恰当响应。通过引入长时间延时，还可以模拟节点甚至整个服务不可用。
Conformity Monkey，查找不符合最佳实践的实例，并将其关闭。例如，如果某个实例不在自动伸缩组里，那么就该将其关闭，让服务所有者能重新让其正常启动。
Doctor Monkey，查找不健康实例的工具，除了运行在每个实例上的健康检查，还会监控外部健康信号，一旦发现不健康实例就会将其移出服务组。
Janitor Monkey，查找不再需要的资源，将其回收，这能在一定程度上降低云资源的浪费。
Security Monkey，这是Conformity Monkey的一个扩展，检查系统的安全漏洞，同时也会保证SSL和DRM证书仍然有效。
10-18 Monkey，进行本地化及国际化的配置检查，确保不同地区、使用不同语言和字符集的用户能正常使用Netflix。
Chaos Gorilla，Chaos Monkey的升级版，可以模拟整个Amazon Availability Zone故障，以此验证在不影响用户，且无需人工干预的情况下，能够自动进行可用区的重新平衡。
