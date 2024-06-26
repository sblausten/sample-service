# This doc is for testing styling problems from a subdirectory

Here is a markdown table:

TEST LINK - [index-page](https://github.com/sblausten/sample-service/blob/main/docs/folder/index.md)

| Hello       | there     | Tilte  |   |   |
|-------------|-----------|--------|---|---|
| Value one   | Value two | `code` |   |   |
| Empty cells |           |        |   |   |
|             |           |        |   |   |

Code block

```js
const person = 'one';

const func = () => {
  return 'this is a func';
};
```

```mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```

Headings

# Heading one

## Heading 2

### heading three

Version number: 2

### heading 4

Embedded images

![expedia group](./the-power-of-platform-logos-updated.png)

# Graphviz

This should render a small diagram as long as `graphviz` is available in the environment
where the docs are generated. [MkDocs will use it automatically](https://github.com/backstage/mkdocs-techdocs-core/blob/main/src/core.py#L106).

{% dot attack_plan.svg
    digraph G {
        rankdir=LR
        Earth [peripheries=2]
        Mars
        Earth -> Mars
    }
%}

[comment]: <> (# PlantUML)

[comment]: <> (```plantuml format="png" classes="uml myDiagram" alt="My super diagram placeholder" title="My super diagram" width="300px" height="300px")

[comment]: <> (  Goofy ->  MickeyMouse: calls)

[comment]: <> (  Goofy <-- MickeyMouse: responds)

[comment]: <> (```)

[comment]: <> (::uml:: format="png" classes="uml myDiagram" alt="My super diagram placeholder" title="My super diagram" width="300px" height="300px")

[comment]: <> (  Goofy ->  MickeyMouse: calls)

[comment]: <> (  Goofy <-- MickeyMouse: responds)

[comment]: <> (::end-uml::)


# Mermaid 
This project contains a few lambdas to handle managing installations, github webhook handlers and dishing out tokens to backstage backends.

```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'primaryColor': '#ff0000'}}}%%
        graph TD
          A[Christmas] -->|Get money| B(Go shopping)
          B --> C{Let me think}
          B --> G[/Another/]
          C ==>|One| D[Laptop]
          C -->|Two| E[iPhone]
          C -->|Three| F[fa:fa-car Car]
          subgraph section
            C
            D
            E
            F
            G
          end
```

# Images

<details>
  <summary>Example Diagram</summary>
## LOCAL PNG
![png](../assets/headline.png)
</details><br>

## LOCAL SVG
<details>
![svg](../assets/coverage.svg)
</details>


