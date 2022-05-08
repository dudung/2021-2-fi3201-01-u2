## Comparing two number

Salah satu diagram alir untuk membandingkan dua buah bilangan adalah sebagai berikut.


```python
%load_ext nb_js_diagrammers
```


```python
%%mermaid_magic -h 160

flowchart TD
    B([ Mulai ]);
    E([ Selesai ]);
    I[/ x, y /];
    D1{ x > y};
    D2{ x = y};
    S1[ s = 'x > y'];
    S2[ s = 'x < y'];
    S3[ s = 'x = y'];
    O[/ s /];
    B --> I;
    I --> D1;
    D1 -- Y --> S1;
    D1 -- T --> D2;
    D2 -- Y --> S3;
    D2 -- T --> S2;
    S1 --> O;
    S2 --> O;
    S3 --> O;
    O --> E;
```




<iframe srcdoc="&lt;html&gt;
    &lt;body&gt;
        &lt;script src=&quot;https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js&quot;&gt;&lt;/script&gt;
        &lt;script&gt;
            mermaid.initialize({ startOnLoad: true });
        &lt;/script&gt;

        &lt;div class=&quot;mermaid&quot;&gt;

flowchart TD
    B([ Mulai ]);
    E([ Selesai ]);
    I[/ x, y /];
    D1{ x &gt; y};
    D2{ x = y};
    S1[ s = &#x27;x &gt; y&#x27;];
    S2[ s = &#x27;x &lt; y&#x27;];
    S3[ s = &#x27;x = y&#x27;];
    O[/ s /];
    B --&gt; I;
    I --&gt; D1;
    D1 -- Y --&gt; S1;
    D1 -- T --&gt; D2;
    D2 -- Y --&gt; S3;
    D2 -- T --&gt; S2;
    S1 --&gt; O;
    S2 --&gt; O;
    S3 --&gt; O;
    O --&gt; E;

        &lt;/div&gt;

    &lt;/body&gt;
&lt;/html&gt;
" width="100%" height="160"style="border:none !important;" "allowfullscreen" "webkitallowfullscreen" "mozallowfullscreen"></iframe>


