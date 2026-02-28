# Fragmentation in Operating System

## What is Fragmentation?

Fragmentation refers to the wastage of memory that occurs when memory is allocated and deallocated over time, leading to unusable memory spaces.

There are two main types of fragmentation:

1. Internal Fragmentation
2. External Fragmentation

---

# 1. Internal Fragmentation

## Definition

Internal fragmentation occurs when the memory block allocated to a process is larger than the memory required by that process. The unused space inside the allocated block is wasted.

## Example

- Memory block size = 10 KB
- Process requires = 8 KB
- Allocated = 10 KB
- Used = 8 KB
- Wasted = 2 KB

The 2 KB wasted space inside the allocated block cannot be used by another process.

## Where It Occurs

- Fixed partition memory allocation
- Paging system (last page)

## Key Points

- Wastage occurs inside allocated block
- Caused by fixed-size memory blocks
- Cannot be used by other processes

---

# 2. External Fragmentation

## Definition

External fragmentation occurs when total free memory is sufficient to satisfy a request, but the available memory is not contiguous (not in one continuous block).

## Example

Memory Layout:

- Free 5 KB
- Used 10 KB
- Free 4 KB
- Used 6 KB
- Free 3 KB

Total free memory = 12 KB

If a process requires 10 KB, it cannot be allocated because there is no single continuous 10 KB block.

## Where It Occurs

- Dynamic partitioning
- Contiguous memory allocation

## Key Points

- Free memory exists but is scattered
- Requires contiguous memory
- Can prevent allocation despite sufficient total memory

---

# Internal vs External Fragmentation

| Feature | Internal Fragmentation | External Fragmentation |
|----------|-----------------------|------------------------|
| Wastage Location | Inside allocated block | Outside allocated blocks |
| Memory Continuous Issue | No | Yes |
| Occurs In | Fixed partition, Paging | Dynamic partition |
| Solution | Reduce block size | Compaction |

---

# Solutions to Fragmentation

## 1. Compaction
- Rearranges memory to combine scattered free blocks into one large block.
- Used to reduce external fragmentation.

## 2. Paging
- Divides memory into fixed-size pages and frames.
- Eliminates external fragmentation.
- May cause internal fragmentation.

## 3. Segmentation
- Divides memory into logical segments (code, stack, data).
- Can cause external fragmentation.
- Does not cause internal fragmentation.

