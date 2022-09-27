# Diagrams

It is often much easier to explain how a script works or should be used by using a diagram. GitHub includes functionality for easily generating diagrams from a simple `mermaid` syntax.

For example,

````
```mermaid
graph LR;
    A[Create branch]-->B[Modify code];
    B-->C[Create pull request];
    C-->D{Accepted?};
    D-->|Yes|E[End];
		D-->|No|B;
```
````

is rendered:

```mermaid
%%{ init: { 'flowchart': { 'curve': 'linearOpen' } } }%%
graph LR;
    A[Create branch]-->B[Modify code];
    B-->C[Create pull request];
    C-->D{Accepted?};
    D-->|Yes|E[End];
		D-->|No|B;
```
