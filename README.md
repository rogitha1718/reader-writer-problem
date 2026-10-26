# EX NO 5 – Reader-Writer Problem

## Aim
To study the Reader-Writer problem.

## Domain / Use Case
Concurrent product inventory management.

## Files
| File | Description |
|------|-------------|
| `ex5_reader_writer.c` | Reader-Writer solution using a `pthread_rwlock_t` |
| `ex5_output.png` | Program output |

## Description
A shared product (price = 99.99, stock = 100) is read by two reader threads (5 reads each) and updated by one writer thread (3 updates: price −1, stock −5). Readers can read at the same time; the writer gets exclusive access.

## Compile and run
```bash
gcc ex5_reader_writer.c -o reader_writer -pthread
./reader_writer
```

## Output
![Output](ex5_output.png)

## Definition
**Reader-Writer Problem** – a synchronization problem where many threads share a resource. Multiple readers may read simultaneously, but a writer needs exclusive access, so synchronization is needed to avoid inconsistency.

## Result
Successfully provided a solution to the Reader-Writer problem.
