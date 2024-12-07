# lecture6.2

> ### Memory technologies

>#### Classes of memory system

![alt text](image.png)

| **Criteria**         | **Type**      | **Description** |
|----------------------|---------------|-----------------|
| **Volatility**       | **Volatile**  | Requires electric power to keep the stored value. |
|                      | **Non-volatile** | Can retain its value without electric power. |
| **CPU Accessibility**| **Primary**   | Directly accessible by the CPU. |
|                      | **Secondary** | CPU access through indirect means of data transfer. |
| **Mutability**       | **Mutable**   | R/W allowed. |
|                      | **Immutable** | Read only. |
| **Access Restriction** | **Random access** | Any of the addressable units can be accessed. |
|                      | **Sequential access** | Memory must be retrieved in an order. |

> #### Attributes of memory technologies

 * Cost
    * The cost of manufacturing and maintenance
 * Compactness
    * The space occupied by memory
  * Throughput
    * The time taken to transfer an amount of data
 * Latency 
    * The time taken for a memory system to begin data transfer


>#### Memory hierarchy of a desktop computer

![alt text](image-1.png)

 
 >#### Static RAM & Dynamic RAM

 | Static RAM | Dynamic RAM |
|------------|--------------|
| Does not need refreshing | Needs constant refreshing |
| SRAM uses normal high speed CMOS technology. (flip-flops) | DRAM uses capacitors for storing bits in the form of charge. |
| Faster, but more expensive | Slower than SRAM because of refreshing time |
| Used as registers in CPU or Cache memory | Used in main memory |
| Technologies include: Synchronous SRAM, Asynchronous SRAM | Technologies include: EDO RAM, VRAM, DDR-RAM Synchronous DRAM |
