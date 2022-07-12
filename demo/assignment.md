---
template: assignment.tex
subjectcode: TDT1234
subjectname: Introduction to \LaTeX
assignment: 0
title: Lorem ipsum dolor
---

# Equations
Sed porta purus eu risus blandit vestibulum. Pellentesque blandit sed velit ac porta. Donec augue arcu, maximus et rhoncus eu, consequat quis turpis. Morbi pretium odio enim, quis ornare odio ornare tempus. Quisque finibus elit eu purus ultricies gravida. 

> consequat quis turpis. Morbi pretium odio enim, quis ornare odio ornare tempus. Quisque finibus elit eu purus ultricies gravida. 

* [Table Section](#tables)
* [Figure Section](#figures)
* [Code Listing Section](#code-listings)

Aenean diam ante, malesuada vel condimentum vitae, laoreet ac risus. Duis ac nulla laoreet, bibendum lorem at, vulputate purus. Sed egestas, purus eget blandit malesuada, ipsum dui accumsan massa, eu aliquet turpis purus.

## Sed tincidunt dapibus nibh sit amet porttitor. 
Interdum et malesuada fames ac ante ipsum primis in faucibus. In pellentesque nibh ut lorem auctor, et dapibus odio sollicitudin. Maecenas faucibus nunc a orci maximus eleifend [@eq:md].

$$ \frac{\Omega}{\Theta}=\sum_{i=0}^k\sqrt[3]{4\cdot5} $$ {#eq:md}

### Donec dui elit 
Rhoncus eu ultrices at, facilisis quis leo. Nam porttitor congue urna, vitae gravida augue ultricies porttitor. In massa risus, varius id commodo sed, varius sit amet elit. In sed massa quis purus semper dignissim. In elementum malesuada erat, nec euismod diam ultricies ut. Proin bibendum, lectus non sagittis suscipit, lorem urna tincidunt mauris, at mollis enim felis et metus [@eq:aligned]. 

$$\begin{aligned}
    f_1(n) &= n^2 + 12n + 4 \\
    f_2(n) &= 4(\lg n)      \\
    f_3(n) &= n^2 \cdot 42n \\
    f_4(n) &= n +2          \\
    g_1(n) &= \lg n + 45    \\
    g_2(n) &= 5n - 3        \\
    g_3(n) &= 3n^3          \\
    g_4(n) &= (n+5)^2
\end{aligned}$$ {#eq:aligned}

## In elementum malesuada erat. 
Nec euismod diam ultricies ut. Proin bibendum, lectus non sagittis suscipit, lorem urna tincidunt mauris, at mollis enim felis et metus [@eq:latex].

\begin{equation}
\frac{\Omega}{\Theta}=\sum_{i=0}^k\sqrt[3]{4\cdot5}
\label{eq:latex}
\end{equation}

# Tables
Mauris porta felis tincidunt, semper sapien eu, volutpat eros. Vestibulum facilisis libero eu lacus volutpat bibendum sed imperdiet ligula [@tbl:md].

| Lorem | Ipsum |      Sit |
|:------|:-----:|---------:|
| Color |   A   | Sit Amet |
: Mauris sit amet sollicitudin vehicula.
{#tbl:md}

## Mauris porta sem diam
Mauris porta felis tincidunt, semper sapien eu, volutpat eros. Vestibulum facilisis libero eu lacus volutpat bibendum sed imperdiet ligula. Aenean finibus turpis purus, vitae sollicitudin metus sodales vitae. Vestibulum tempus porta velit. In eu lacus nisi. Donec cursus scelerisque nisl, vel tempus erat posuere vitae. Nunc vestibulum lacus posuere pretium ultrices. Morbi pharetra libero erat, a malesuada lectus mollis et. Suspendisse efficitur, mauris sit amet sollicitudin vehicula, sem libero sagittis nisi, vel tincidunt diam lacus ac nibh. Morbi maximus, magna non egestas rutrum, libero mauris scelerisque nunc, in elementum libero tortor sit amet libero. Morbi id facilisis neque, non pellentesque nisl. Cras blandit, nibh ac pulvinar suscipit, nunc neque commodo magna, luctus vehicula lacus arcu ut dui. Quisque sed nisl nec purus vehicula elementum [@tbl:latex].

\begin{table}
    \centering
    \begin{tabular}{ | l | l | c | c | c | c | }
        \hline
        Is Output        & Layer Type    & Number of Filters        & Kernel Size & Stride & Padding \\
        \hline
             &  Conv2d       &         32               &      3      &    1    &    1   \\
             &  ReLU         &         -                &      -      &    -    &    -   \\
             &  MaxPool2d    &         -                &      2      &    2    &    -   \\
             &  Conv2d       &         64               &      3      &    1    &    1   \\
        Yes  &  ReLU         &         -                &      -      &    -    &    -   \\
        \hline
             &  Conv2d       &         64               &      3      &    1    &    1   \\
             &  ReLU         &         -                &      -      &    -    &    -   \\
             &  Conv2d       &   output$\_$channels[0]  &      3      &    2    &    1   \\
        Yes  &  ReLU         &         -                &      -      &    -    &    -   \\
        \hline
             &  Conv2d       &         128              &      3      &    1    &    1   \\
             &  ReLU         &         -                &      -      &    -    &    -   \\
             &  Conv2d       &   output$\_$channels[1]  &      3      &    2    &    1   \\
        Yes  &  ReLU         &         -                &      -      &    -    &    -   \\
        \hline
    \end{tabular}
    \caption{Luctus vehicula lacus arcu ut dui.}
    \label{tbl:latex}
\end{table}



# Figures
Mauris porta felis tincidunt, semper sapien eu, volutpat eros. Vestibulum facilisis libero eu lacus volutpat bibendum sed imperdiet ligula. Cras blandit, nibh ac pulvinar suscipit, nunc neque commodo magna, luctus vehicula lacus arcu ut dui. Quisque sed nisl nec purus vehicula elementum [@fig:md].


![Nunc neque commodo magna, luctus vehicula lacus arcu ut dui.](./assets/fig1.jpeg){#fig:md width=50%}

### Aenean finibus turpis purus.
Vitae sollicitudin metus sodales vitae. Vestibulum tempus porta velit. In eu lacus nisi. Donec cursus scelerisque nisl, vel tempus erat posuere vitae. Nunc vestibulum lacus posuere pretium ultrices. Morbi pharetra libero erat, a malesuada lectus mollis et. Suspendisse efficitur, mauris sit amet sollicitudin vehicula, sem libero sagittis nisi, vel tincidunt diam lacus ac nibh. Morbi maximus, magna non egestas rutrum, libero mauris scelerisque nunc, in elementum libero tortor sit amet libero. Morbi id facilisis neque, non pellentesque nisl [@fig:latex]. 

\begin{figure}
    \centering
    \includegraphics[width=0.5\textwidth]{assets/fig2}
    \caption{Imperdiet ligula.}
    \label{fig:latex}
\end{figure}


### Mauris porta felis tincidunt
Semper sapien eu, volutpat eros. Vestibulum facilisis libero eu lacus volutpat bibendum sed imperdiet ligula. Aenean finibus turpis purus, vitae sollicitudin metus sodales vitae. Vestibulum tempus porta velit. In eu lacus nisi. Donec cursus scelerisque nisl, vel tempus erat posuere vitae. Nunc vestibulum lacus posuere pretium ultrices. Morbi pharetra libero erat, a malesuada lectus mollis et. Suspendisse efficitur, mauris sit amet sollicitudin vehicula, sem libero sagittis nisi, vel tincidunt diam lacus ac nibh. Morbi maximus, magna non egestas rutrum, libero mauris scelerisque nunc, in elementum libero tortor sit amet libero. Morbi id facilisis neque, non pellentesque nisl. Cras blandit, nibh ac pulvinar suscipit, nunc neque commodo magna, luctus vehicula lacus arcu ut dui. Quisque sed nisl nec purus vehicula elementum [@fig:tikz].

\begin{figure}
    \centering
    \begin{tikzpicture}[every node/.style={font=\Large}]
        \node[node, fill=yellow] (a)   {a}; 
        \node[node] (b) [right = of a] {b}; 
        \node[node] (c) [right = of b] {c}; 
        \node[node] (d) [below = of a] {d}; 
        \node[node] (e) [right = of d] {e}; 
        \node[node] (f) [right = of e] {f}; 
        \node[node] (g) [below = of d] {g}; 
        \node[node] (h) [right = of g] {h}; 
        \node[node] (i) [right = of h] {i}; 
        \draw[edge] (a) -- (b); 
        \draw[edge] (a) -- (d); 
        \draw[edge] (b) -- (c); 
        \draw[edge] (c) -- (f); 
        \draw[edge] (d) -- (e); 
        \draw[edge] (d) -- (h); 
        \draw[edge] (e) -- (b); 
        \draw[edge] (e) -- (g); 
        \draw[edge] (f) -- (i); 
        \draw[edge] (g) -- (h); 
        \draw[edge] (h) -- (f); 
        \draw[edge] (e) -- (i); 
    \end{tikzpicture}
    \caption{In eu lacus nisi. Donec cursus scelerisque nisl}
    \label{fig:tikz}
\end{figure}


# Code Listings


#### Finibus dictum lacus
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed egestas facilisis mauris vel vestibulum. Mauris purus augue, bibendum vel felis quis, finibus rhoncus quam. Nulla sed ipsum nisl. Morbi tristique ac quam eu consectetur. Nulla nisl enim, rutrum non justo in, egestas porttitor felis. Cras ut vulputate orci. Mauris nisl urna, blandit eu pellentesque in, aliquam eu diam. Suspendisse in diam quis orci commodo vulputate. Etiam neque nibh, efficitur vitae lacus vel, auctor sollicitudin ante [@lst:md].


```python
Greedy-Balance:
    Start with no jobs assigned
    Ti=0 
    Ai={} for all machines Mi 
    For j=1,...,n
        Let Mi be a machine that achieves the minimum Tk 
        Assign job j to machine Mi
        Set Ai += {j}
        Set Ti += tj
    EndFor
```
: In eu lacus nisi. Donec cursus scelerisque nisl, vel tempus erat posuere vitae.
{#lst:md}

#### Nam dignissim purus ut mauris porta, a porta ipsum tristique. 
Maecenas lacinia pharetra quam, in imperdiet enim cursus quis. Suspendisse nec tortor a mi tincidunt tristique a nec tellus.Praesent viverra nunc sed nisl aliquet, vel malesuada lorem sagittis. Nunc blandit vulputate nisl eu vehicula. In pellentesque mauris eu est varius, sit amet congue mi lacinia. Phasellus at diam eu nulla porttitor vehicula vitae non arcu. 

Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Cras et ornare nulla. Vestibulum scelerisque tellus eu risus tempor, eu sagittis nibh condimentum. Aenean molestie turpis feugiat cursus placerat. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Praesent fermentum nisl ut est ornare, et convallis eros cursus. Integer et orci ultrices, molestie enim ac, molestie nunc. Integer tortor erat, bibendum sit amet turpis pharetra, faucibus molestie augue [@lst:latex].

\begin{codelisting}
    \caption{In eu lacus nisi. Donec cursus scelerisque nisl, vel tempus erat posuere vitae.}
    \begin{lstlisting}[language=python, label=lst:latex]
    Greedy-Balance:
        Start with no jobs assigned
        Ti=0 
        Ai={} for all machines Mi 
        For j=1,...,n
            Let Mi be a machine that achieves the minimum Tk 
            Assign job j to machine Mi
            Set Ai += {j}
            Set Ti += tj
        EndFor
    \end{lstlisting}
\end{codelisting}
