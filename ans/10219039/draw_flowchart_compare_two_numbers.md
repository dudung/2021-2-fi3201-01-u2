![](draw_flowchart_compare_two_numbers.png)

```mermaid
%%mermaid_magic -h 160

flowchart TD
    B([ Mulai ]);
    E([ Selesai ]);
    I[/ x /];
    D1{ x > 0};
    D2{ x = 0};
    S1[ sign = 1];
    S2[ sign = 0];
    S3[ sign = -1];
    O[/ sign /];
    B --> I;
    I --> D1;
    D1 -- Y --> S1;
    D1 -- T --> D2;
    D2 -- T --> S3;
    D2 -- Y --> S2;
    S1 --> O;
    S2 --> O;
    S3 --> O;
    O --> E;
```
