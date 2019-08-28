@RestController
标记在类上,表示该类处理http请求,并且返回json数据
RestController = ResponseBody +@Controller的组合注解

@Service
一般用于修饰service层的组件

@PathVariable
获取参数,通过 @PathVariable 可以将 URL 中占位符参数绑定到控制器处理方法的入参中：URL 中的 {xxx} 占位符可以通过@PathVariable(“xxx“) 绑定到操作方法的入参中。

@ PostMapping
@RequestMapping(method = RequestMethod.POST)的简写
用于处理请求方法的POST类型，向服务器提交添加/新增信息请求

@PutMapping
向服务器提交更新信息

@Autowired
自动导入依赖的bean,将其他的类，接口引入，类似于之前的类的初始化等，用这个注解，类或接口的方法就可以直接调用了

@RequestMapping
提供路由信息，负责URL到Controller中的具体函数的映射。即当前台界面调用Controller处理数据时候告诉控制器怎么操作

@GetMapping
@RequestMapping(method = RequestMethod.GET)的简写
用于处理请求方法的GET类型

@RequestParam
用在方法的参数前面，用来接收后台参数。其有三个配置参数：（1）required 表示是否必须，默认为 true。（2）defaultValue 可设置请求参数的默认值。（3）value 为接收url的参数名（相当于key值）。

@RequestBody
@RequestBody接收的参数是来自requestBody中，即请求体。主要用来处理Content-Type是application/json，application/xml的Json字符串。多用在Post类型请求中。

@DeleteMapping
用于将HTTP DELETE请求映射到特定处理程序方法的注释。具体来说，@DeleteMapping是一个作为快捷方式的组合注释@RequestMapping(method = RequestMethod.DELETE)。





