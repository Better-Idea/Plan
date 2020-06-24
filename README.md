# Plan
**计划第一定律：计划赶不上变化**

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
| FUNCB | MMU 派生体系设计                                                       |
| TINYA | 创建公共外部 API 引用中心以减少 .cpp 数目                              |
| FUNCB | 策划多线程版本的 GC                                                    |
| FUNCA | 基于 setjmp + 清除栈的异常模型设计                                     |
| FUNCB | 完善迭代器，增加顺序访问迭代器                                         |
| TINYA | 给函数使用合适的迭代器                                                 |

## Pop
| Type  | Description                                                            |
|-------|------------------------------------------------------------------------|
| MOVEA | 整合内存分配算法                                                       |
| TESTA | 日期时间库-Date, Time 基础测试                                         |
| FUNCA | 日期时间库-Date, Time 设计                                             |
