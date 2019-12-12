# Example #1: Basic Flow Chart

<img height=480 src="https://markdown-engineering.herokuapp.com/
%    graph TD
%    A[Choose a number] --> B{Is it 14}
%    B --> A
%    B --> C(Awesome)
"/>



Using markdown syntax in github.com

Also can use Markdown syntax including a image tag and then the url content include DOT, PlantUML or UMLGraph syntax. Don't forget to close the image tag.

![Alt text](https://g.gravizo.com/svg?
  digraph G {
    aize ="4,4";
    main [shape=box];
    main -> parse [weight=8];
    parse -> execute;
    main -> init [style=dotted];
    main -> cleanup;
    execute -> { make_string; printf}
    init -> make_string;
    edge [color=red];
    main -> printf [style=bold,label="100 times"];
    make_string [label="make a string"];
    node [shape=box,style=filled,color=".7 .3 1.0"];
    execute -> compare;
  }
)

