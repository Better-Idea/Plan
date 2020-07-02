# Plan
**计划第一定律：计划赶不上变化**  
**计划第二定律：不忘初心，方得始终**

## Type
- FUNCA：功能创建
- FUNCB：功能增强
- TESTA：基础测试
- TESTB：增强测试
- MOVEA：枯木新芽
- TINYA：最小设计

## Push
| Type  | Description                                                            |
|-------|------------------------------------------------------------------------|
| FUNCA | 设计模块多版本共存兼容惯用法                                           |
| FUNCA | 让 xgc_field 支持序列化                                                |
| FUNCB | MMU 派生体系设计                                                       |
| FUNCB | 让 GC 支持反射抽象类                                                   |
| FUNCB | 策划多线程版本的 GC                                                    |
| FUNCA | 基于 setjmp + 清除栈的异常模型设计                                     |
| FUNCB | 完善迭代器，增加顺序访问迭代器                                         |
| TINYA | 给函数使用合适的迭代器                                                 |

## Pop
| Type  | Description                                                            |
|-------|------------------------------------------------------------------------|
| MOVEA | 整合针对小容量内存设计的绘图缓冲区                                     |
| FUNCB | 让 lang/cxx/strlize 支持浮点                                           |
| FUNCB | 让 lang/cxx/parse 支持浮点                                             |
| FUNCB | 让 lang::cxx::ph 支持将多个元素当作一个整体对齐                        |
| TINYA | 创建公共外部 API 引用中心以减少 .cpp 数目                              |
| MOVEA | 整合内存分配算法                                                       |
| TESTA | 日期时间库-Date, Time 基础测试                                         |
| FUNCA | 日期时间库-Date, Time 设计                                             |
