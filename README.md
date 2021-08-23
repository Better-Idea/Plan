# Plan
**计划第一定律：计划赶不上变化**  
**计划第二定律：不忘初心，方得始终**

## Type
- 功能预研
- 功能创建
- 功能增强
- 功能说明
- 用法指引
- 基础测试
- 增强测试
- 枯木新芽
- 生根发芽
- 最小设计
- 层次设计
- 一致设计
- 隐藏细节
- 多平台化
- 代码回顾
- 问题修复
- 使国际化

## Push
| 类别     | 描述                                                                   |
|----------|------------------------------------------------------------------------|
| 层次设计 | 让 concurrency/lock/ 不依赖 thread_self::yield()                       |
| 多平台化 | 让 linux 平台的线程也使用信号量作为 suspend/resume 的操作对象          |
| 一致设计 | 统一 extern.memory 中两种分配算法的内存使用计数器                      |
| 层次设计 | 使用函数底层实现 + 类上层包装的模式                                    |
| 功能预研 | 设计结构化模板配置参数                                                 |
| 功能预研 | 设计基于 [[no_unique_address]] 的属性范式                              |
| 功能增强 | 使用 doxygen 格式的文档注释                                            |
| 功能增强 | 让 GC 支持修改指向时的共享安全                                         |
| 功能增强 | 让 GC 支持前台线程自行[外析构]特定的[平凡类型]以减少队列压力           |
| 功能增强 | 让结构嵌套的容器对接 GC 接口                                           |
| 功能创建 | 初步封装套接字接口，先支持 linux 平台                                  |
| 隐藏细节 | 在 docker/private/btree.hpp 中隐藏 SIMD 实现                           |
| 最小设计 | 给出 std::initializer_list 替代方案                                    |
| 功能增强 | 让 macro/private/extern.log 通用化                                     |
| 功能增强 | 在 macro/private/extern.log 底层实现使用缓存                           |
| 功能创建 | 创建 Mix-C ISA 汇编器                                                  |
| 功能创建 | 添加 docker/ring_buffer                                                |
| 功能增强 | 解决 xinterface 子接口重载冲突问题                                     |
| 功能增强 | 让 xinterface 支持接口间里氏转换                                       |
| 功能增强 | 让 xinterface 支持强引用模式                                           |
| 功能增强 | 让 xinterface 支持区分函数 const 修饰重载                              |
| 功能增强 | 让 xinterface 支持去重功能                                             |
| 功能创建 | 线程库设计                                                             |
| 功能创建 | 为 Mix-C ISA 设计调用范式                                              |
| 功能创建 | 基于 algo/mmu 的树形结构                                               |
| 功能增强 | MMU 派生体系设计                                                       |
| 功能增强 | 让 macro/xstruct 支持引用类型成员变量指针                              |
| 功能增强 | 让 macro/xstruct 支持反射抽象类                                        |
| 功能增强 | 完善迭代器，增加顺序访问迭代器                                         |
| 最小设计 | 给函数使用合适的迭代器                                                 |
| 功能增强 | 让 docker/hashmap 针对 sizeof(kv) < sizeof(uxx) 的内存节省优化         |
| 功能创建 | 基于 setjmp + 清除栈的异常模型设计                                     |
| 使国际化 | 给 README 添加英文版本                                                 |

## Pop
| 类别     | 描述                                                                   |
|----------|------------------------------------------------------------------------|
| 代码回顾 | 回顾 2021/08/23 Mix-C 项目提交的代码                                   |
| 代码回顾 | 回顾 2021/08/22 Mix-C 项目提交的代码                                   |
| 代码回顾 | 回顾 2021/08/16 Mix-C 项目提交的代码                                   |
| 问题修复 | 修复 GC 剪枝 BUG                                                       |
| 一致设计 | 引入匈牙利命名法修饰变量名称                                           |
| 功能增强 | 策划多线程版本的 GC                                                    |
| 功能增强 | 支持多线程版 tiny_allocator                                            |
| 最小设计 | 整理 memory/ 接口                                                      |
| 一致设计 | 使用 _v 后缀作为数值模板参数的提案                                     |
| 一致设计 | 关于模板参数、类内部私有模板别名统一使用 _t 后缀标识的提案             |
| 用法指引 | 编写包含范式更多细节                                                   |
| 功能创建 | 初步封装 pthread，先支持 linux 平台                                    |
| 生根发芽 | 让 draft/json.hpp 转正到 lang/cxx/parse_json.hpp                       |
| 最小设计 | 关于 interface/ranger concept 约束部分有些乱，需要重构一下             |
| 多平台化 | 支持 msvc                                                              |
| 功能增强 | 让 xinterface 支持重载                                                 |
| 功能增强 | 让 lang::cxx::ph 支持带占位符的格式化                                  |
| 功能增强 | 完善 lang/cxx/ph                                                       |
| 功能说明 | 绿化 algo/                                                             |
| 最小设计 | 重构 lang/cxx/replace                                                  |
| 功能增强 | 让 docker/array 支持动态分配的数组                                     |
| 功能增强 | 将 xinterface 参数替换成模板 + concept 以优化性能                      |
| 功能增强 | 改善 macro/xinterface 性能                                             |
| 功能增强 | 让 macro/xinterface 支持继承                                           |
| 功能增强 | 完善 docker/stack 锁机制                                               |
| 功能增强 | 完善 docker/queue 锁机制                                               |
| 功能增强 | 重构测试框架                                                           |
| 功能增强 | 让 lock/policy_barrier 让所有独占式操作共用一个同步位                  |
| 功能创建 | 设计模块多版本共存兼容惯用法                                           |
| 功能增强 | 全局应用 xexport，并将 xuser::inc -> xuser                             |
| 功能创建 | 封装 asin/acos/cosh/sinh                                               |
| 功能创建 | 实现 math/atan                                                         |
| 功能创建 | 创建 io/dir 目录基础功能                                               |
| 功能增强 | 在 io/tty 中添加 read_line                                             |
| 基础测试 | algo/mmu                                                               |
| 功能说明 | algo/mmu                                                               |
| 功能创建 | 规划文档注释规范 step 0                                                |
| 功能创建 | 规划文档注释规范 step 0                                                |
| 功能创建 | 细化 Mix-C 随机访问接口                                                |
| 功能创建 | 给 Mix-F 新增 UART 接口                                                |
| 功能增强 | 让 macro/xstruct 支持位域                                              |
| 用法指引 | 绿化：给 define/inf 添加帮助注释                                       |
| 用法指引 | 绿化：给 define/nan 添加帮助注释                                       |
| 用法指引 | 绿化：给 define/nullref 添加帮助注释                                   |
| 功能创建 | 在 Mix-C ISA 完善 asm_ldkx 指令                                        |
| 功能创建 | 在 Mix-C ISA 完善 asm_stkx 指令                                        |
| 枯木新芽 | 迁移 Mix-C ISA                                                         |
| 枯木新芽 | 迁移数字电路仿真库                                                     |
| 功能增强 | 让 xitf 接口模板使用结构体，并支持继承                                 |
| 多平台化 | 让 Mix-C 项目支持 linux                                                |
| 多平台化 | 让 Mix-C 项目支持 msvc                                                 |
| 功能增强 | 设计可配置并发度的 lock/policy_barrier                                 |
| 功能增强 | lock/policy_barrier 增强，增加分类抽象                                 |
| 功能创建 | 设计迭代器函数标准接口                                                 |
| 功能说明 | 给包含范式添加文档                                                     |
| 功能增强 | 在 hashmap 考虑键值对初始化、赋值的正确性                              |
| 功能增强 | 给 hashmap 添加 bit_indicator 增强 clear 时的性能                      |
| 功能说明 | 让 GC/ 帮助文档清晰                                                    |
| 功能增强 | 让 xstruct 支持序列化                                                  |
| 用法指引 | 给 lang/cxx/ 添加用法                                                  |
| 功能增强 | 完成 xgc_field 到 xstruct 的过渡，并适配 GC/private/                   |
| 枯木新芽 | 整合针对小容量内存设计的绘图缓冲区                                     |
| 功能增强 | 让 lang/cxx/strlize 支持浮点                                           |
| 功能增强 | 让 lang/cxx/parse 支持浮点                                             |
| 功能增强 | 让 lang::cxx::ph 支持将多个元素当作一个整体对齐                        |
| 最小设计 | 创建公共外部 API 引用中心以减少 .cpp 数目                              |
| 枯木新芽 | 整合内存分配算法                                                       |
| 基础测试 | 日期时间库-Date, Time 基础测试                                         |
| 功能创建 | 日期时间库-Date, Time 设计                                             |

