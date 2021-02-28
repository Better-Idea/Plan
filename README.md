# Plan
**计划第一定律：计划赶不上变化**  
**计划第二定律：不忘初心，方得始终**

## Type
- 功能创建：FUNCA
- 功能增强：FUNCB
- 功能说明：HELPA
- 用法指引：HELPB
- 基础测试：TESTA
- 增强测试：TESTB
- 枯木新芽：MOVEA
- 生根发芽：MOVEB
- 最小设计：TINYA
- 一致设计：CONSA
- 多平台化：PLTFA
- 使国际化：PLTFB
- 隐藏细节：HIDEA

## Push
| Type  | Description                                                            |
|-------|------------------------------------------------------------------------|
| FUNCB | 使用 doxygen 格式的文档注释                                            |
| FUNCA | 初步封装套接字接口，先支持 linux 平台                                  |
| HIDEA | 在 docker/private/btree.hpp 中隐藏 SIMD 实现                           |
| TINYA | 给出 std::initializer_list 替代方案                                    |
| FUNCB | 让 macro/private/extern.log 通用化                                     |
| FUNCB | 在 macro/private/extern.log 底层实现使用缓存                           |
| FUNCA | 创建 Mix-C ISA 汇编器                                                  |
| FUNCA | 添加 docker/ring_buffer                                                |
| FUNCB | 解决 xinterface 子接口重载冲突问题                                     |
| FUNCB | 让 xinterface 支持接口间里氏转换                                       |
| FUNCB | 让 xinterface 支持强引用模式                                           |
| FUNCB | 让 xinterface 支持区分函数 const 修饰重载                              |
| FUNCB | 让 xinterface 支持去重功能                                             |
| FUNCA | 线程库设计                                                             |
| FUNCA | 为 Mix-C ISA 设计调用范式                                              |
| FUNCA | 基于 algo/mmu 的树形结构                                               |
| FUNCB | MMU 派生体系设计                                                       |
| FUNCB | 策划多线程版本的 GC                                                    |
| FUNCB | 让 macro/xstruct 支持引用类型成员变量指针                              |
| FUNCB | 让 macro/xstruct 支持反射抽象类                                        |
| FUNCB | 完善迭代器，增加顺序访问迭代器                                         |
| TINYA | 给函数使用合适的迭代器                                                 |
| FUNCB | 让 docker/hashmap 针对 sizeof(kv) < sizeof(uxx) 的内存节省优化         |
| FUNCA | 基于 setjmp + 清除栈的异常模型设计                                     |
| PLTFB | 给 README 添加英文版本                                                 |

## Pop
| Type  | Description                                                            |
|-------|------------------------------------------------------------------------|
| TINYA | 整理 memory/ 接口                                                      |
| CONSA | 使用 _v 后缀作为数值模板参数的提案                                     |
| CONSA | 关于模板参数、类内部私有模板别名统一使用 _t 后缀标识的提案             |
| HELPB | 编写包含范式更多细节                                                   |
| FUNCA | 初步封装 pthread，先支持 linux 平台                                    |
| MOVEB | 让 draft/json.hpp 转正到 lang/cxx/parse_json.hpp                       |
| TINYA | 关于 interface/ranger concept 约束部分有些乱，需要重构一下             |
| PLTFA | 支持 msvc                                                              |
| FUNCB | 让 xinterface 支持重载                                                 |
| FUNCB | 让 lang::cxx::ph 支持带占位符的格式化                                  |
| FUNCB | 完善 lang/cxx/ph                                                       |
| HELPA | 绿化 algo/                                                             |
| TINYA | 重构 lang/cxx/replace                                                  |
| FUNCB | 让 docker/array 支持动态分配的数组                                     |
| FUNCB | 将 xinterface 参数替换成模板 + concept 以优化性能                      |
| FUNCB | 改善 macro/xinterface 性能                                             |
| FUNCB | 让 macro/xinterface 支持继承                                           |
| FUNCB | 完善 docker/stack 锁机制                                               |
| FUNCB | 完善 docker/queue 锁机制                                               |
| FUNCB | 重构测试框架                                                           |
| FUNCB | 让 lock/policy_barrier 让所有独占式操作共用一个同步位                  |
| FUNCA | 设计模块多版本共存兼容惯用法                                           |
| FUNCB | 全局应用 xexport，并将 xuser::inc -> xuser                             |
| FUNCA | 封装 asin/acos/cosh/sinh                                               |
| FUNCA | 实现 math/atan                                                         |
| FUNCA | 创建 io/dir 目录基础功能                                               |
| FUNCB | 在 io/tty 中添加 read_line                                             |
| TESTA | algo/mmu                                                               |
| HELPA | algo/mmu                                                               |
| FUNCA | 规划文档注释规范 step 0                                                |
| FUNCA | 规划文档注释规范 step 0                                                |
| FUNCA | 细化 Mix-C 随机访问接口                                                |
| FUNCA | 给 Mix-F 新增 UART 接口                                                |
| FUNCB | 让 macro/xstruct 支持位域                                              |
| HELPB | 绿化：给 define/inf 添加帮助注释                                       |
| HELPB | 绿化：给 define/nan 添加帮助注释                                       |
| HELPB | 绿化：给 define/nullref 添加帮助注释                                   |
| FUNCA | 在 Mix-C ISA 完善 asm_ldkx 指令                                        |
| FUNCA | 在 Mix-C ISA 完善 asm_stkx 指令                                        |
| MOVEA | 迁移 Mix-C ISA                                                         |
| MOVEA | 迁移数字电路仿真库                                                     |
| FUNCB | 让 xitf 接口模板使用结构体，并支持继承                                 |
| PLTFA | 让 Mix-C 项目支持 linux                                                |
| PLTFA | 让 Mix-C 项目支持 msvc                                                 |
| FUNCB | 设计可配置并发度的 lock/policy_barrier                                 |
| FUNCB | lock/policy_barrier 增强，增加分类抽象                                 |
| FUNCA | 设计迭代器函数标准接口                                                 |
| HELPA | 给包含范式添加文档                                                     |
| FUNCB | 在 hashmap 考虑键值对初始化、赋值的正确性                              |
| FUNCB | 给 hashmap 添加 bit_indicator 增强 clear 时的性能                      |
| HLEPA | 让 gc/ 帮助文档清晰                                                    |
| FUNCB | 让 xstruct 支持序列化                                                  |
| HELPB | 给 lang/cxx/ 添加用法                                                  |
| FUNCB | 完成 xgc_field 到 xstruct 的过渡，并适配 gc/private/                   |
| MOVEA | 整合针对小容量内存设计的绘图缓冲区                                     |
| FUNCB | 让 lang/cxx/strlize 支持浮点                                           |
| FUNCB | 让 lang/cxx/parse 支持浮点                                             |
| FUNCB | 让 lang::cxx::ph 支持将多个元素当作一个整体对齐                        |
| TINYA | 创建公共外部 API 引用中心以减少 .cpp 数目                              |
| MOVEA | 整合内存分配算法                                                       |
| TESTA | 日期时间库-Date, Time 基础测试                                         |
| FUNCA | 日期时间库-Date, Time 设计                                             |

