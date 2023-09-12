```

BenchmarkDotNet v0.13.8, Windows 11 (10.0.22621.2134/22H2/2022Update/SunValley2)
AMD Ryzen 9 5900HX with Radeon Graphics, 1 CPU, 16 logical and 8 physical cores
.NET SDK 7.0.306
  [Host]     : .NET 7.0.9 (7.0.923.32018), X64 RyuJIT AVX2
  DefaultJob : .NET 7.0.9 (7.0.923.32018), X64 RyuJIT AVX2


```
| Method | Size   | Max        | SortOrder  | Mean         | Error      | StdDev      |
|------- |------- |----------- |----------- |-------------:|-----------:|------------:|
| **Sort**   | **100000** | **100**        | **None**       |     **1.200 ms** |  **0.0237 ms** |   **0.0354 ms** |
| **Sort**   | **100000** | **100**        | **Ascending**  |     **1.080 ms** |  **0.0216 ms** |   **0.0594 ms** |
| **Sort**   | **100000** | **100**        | **Descending** |     **1.018 ms** |  **0.0200 ms** |   **0.0274 ms** |
| **Sort**   | **100000** | **100000**     | **None**       |     **1.633 ms** |  **0.0283 ms** |   **0.0237 ms** |
| **Sort**   | **100000** | **100000**     | **Ascending**  |     **1.190 ms** |  **0.0166 ms** |   **0.0138 ms** |
| **Sort**   | **100000** | **100000**     | **Descending** |     **1.161 ms** |  **0.0229 ms** |   **0.0483 ms** |
| **Sort**   | **100000** | **1000000**    | **None**       |     **4.879 ms** |  **0.2343 ms** |   **0.6797 ms** |
| **Sort**   | **100000** | **1000000**    | **Ascending**  |     **2.789 ms** |  **0.0535 ms** |   **0.0751 ms** |
| **Sort**   | **100000** | **1000000**    | **Descending** |     **2.778 ms** |  **0.0332 ms** |   **0.0294 ms** |
| **Sort**   | **100000** | **2147483647** | **None**       | **1,464.609 ms** | **27.0154 ms** |  **25.2702 ms** |
| **Sort**   | **100000** | **2147483647** | **Ascending**  | **1,476.686 ms** | **27.0281 ms** |  **25.2821 ms** |
| **Sort**   | **100000** | **2147483647** | **Descending** | **1,720.260 ms** | **50.4674 ms** | **144.8005 ms** |