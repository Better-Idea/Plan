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
- 最小设计：TINYA
- 多平台化：PLTFA
- 使国际化：PLTFB

## Push
| Type  | Description                                                            |
|-------|------------------------------------------------------------------------|
| MOVEA | 迁移数字电路仿真库                                                     |
| FUNCA | 线程库设计                                                             |
| FUNCB | 让 lock/policy_barrier 不能共享的同步域共用一个位指示器                |
| FUNCB | MMU 派生体系设计                                                       |
| FUNCB | 策划多线程版本的 GC                                                    |
| FUNCB | 让 macro/xstruct 支持位域                                              |
| FUNCB | 让 macro/xstruct 支持反射抽象类                                        |
| FUNCB | 在 io/tty 中添加 read_line                                             |
| FUNCB | 完善迭代器，增加顺序访问迭代器                                         |
| TINYA | 给函数使用合适的迭代器                                                 |
| FUNCA | 设计模块多版本共存兼容惯用法                                           |
| FUNCB | 让 docker/hashmap 针对 sizeof(kv) < sizeof(uxx) 的内存节省优化         |
| FUNCA | 基于 setjmp + 清除栈的异常模型设计                                     |
| PLTFB | 给 README 添加英文版本                                                 |

## Pop
| Type  | Description                                                            |
|-------|------------------------------------------------------------------------|
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

