# MySpringMVC

Spring MVC 的实现原理如下:

- **前端控制器 (DispatcherServlet)**: DispatcherServlet 是 Spring MVC 的核心组件,它负责接收和分发来自客户端的请求。DispatcherServlet 会将请求转发给合适的 Controller 处理。
- **处理器映射 (HandlerMapping)**: HandlerMapping 负责根据请求查找对应的 Controller。DispatcherServlet 会通过 HandlerMapping 找到合适的 Controller 来处理请求。
- **控制器 (Controller)**: Controller 负责处理具体的业务逻辑,并返回一个 ModelAndView 对象,该对象包含了视图名称和模型数据。
- **视图解析器 (ViewResolver)**: ViewResolver 负责根据视图名称解析出具体的视图实现,如 JSP、Thymeleaf 等。
- **IOC 容器**: IOC 容器负责管理 Spring MVC 应用程序中的各个组件,包括 Controller、Service、Repository 等。这些组件都被定义为 bean,由 IOC 容器负责创建和管理它们的生命周期。