# JSON 2 JSX

A JSON to JSX converter. 

![preview](https://raw.githubusercontent.com/appcraft/ac-json2jsx/master/doc/sample.png)

## Why ?

We needed to push React component code dynamically to React Native users. Sending raw code and using eval could probably work but would lead to memory leaks. So this is plain JSON, re-interpreted client-side.

Think of it like a JSX templating engine

## How ?

Babel is used to generate an AST of the JSX code. A simple AST interpreter is then used to evaluate that code and create React/React Native components

## FAQ

### This sounds like a terrible idea

Yeah, it probably is. Still not sure if it's a good idea or a crazy one. I'll beb testing and benchmarking it in our product and see how it well it works. Obviously I'm open to other solutions.

## License

MIT
