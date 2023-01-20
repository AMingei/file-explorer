# file-explorer

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


```js
// TemplateClass 作为既定的模板类
CLASS TemplateClass
	// 为子类提供了既定的模板方法 templateMethod()
	+ templateMethod() { if(...) { this.realizableFunctionA(); } else ... }
	# realizableFunctionA() { / }
	- realizableFunctionB() { / }
	- realizableFunctionC() { / }

// 子类继承 TemplateClass，选择性实现父类提供的抽象函数
CLASS ConcreteClassA => TemplateClass
	- realizableFunctionA()
	- realizableFunctionB()

CLASS ConcreteClassB => TemplateClass
	- realizableFunctionB()
	- realizableFunctionC()

INTER ISasd
```
