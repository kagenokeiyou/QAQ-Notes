# Git 教程

## 关于 Git

git 是一个分布式版本控制软件，最初由 Linus Torvalds 创作，于 2005 年以 GPL 许可协议发布。最初目的是为了更好地管理 Linux 内核开发而设计。

自2002年开始，Linus Torvalds 决定使用 BitKeeper 作为 Linux 内核主要的版本控制系统用以维护代码。因为 BitKeeper 为专有软件，这个决定在社群中长期遭受质疑。在 Linux 社群中，特别是 Richard Stallman 与自由软件基金会的成员，主张应该使用开放源代码的软件来作为 Linux 内核的版本控制系统。Linus Torvalds 曾考虑过采用现成软件作为版本控制系统（例如 Monotone），但这些软件都存在一些问题，特别是性能不佳。现成的方案，如 CVS 的架构，受到 Linus Torvalds 的批评。

2005年，Andrew Tridgell 写了一个简单程序，可以连接 BitKeeper 的仓库，BitKeeper 著作权拥有者 Larry McVoy 认为 Andrew Tridgell 对 BitKeeper 内部使用的协议进行逆向工程，决定收回无偿使用 BitKeeper 的许可。Linux 内核开发团队与 BitMover 公司进行磋商，但无法解决他们之间的歧见。Linus Torvalds 决定自行开发版本控制系统替代 BitKeeper，以十天的时间编写出 git 第一个版本。