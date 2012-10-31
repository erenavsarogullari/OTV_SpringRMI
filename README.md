Spring Remoting Support and Developing RMI Service

The development of remote-enabled services is eased by Spring remoting support. Currently, Spring supports the following remoting technologies: Remote Method Invocation (RMI), HTTP Invoker, Hessian, Burlap, JAX-RPC, JAX-WS and JMS.

Remote Method Invocation (RMI) : Spring supports RMI via RmiProxyFactoryBean and RmiServiceExporter. RmiServiceExporter exports any Spring-managed bean as an RMI service and registers. RmiProxyFactoryBean is a factory bean creating a proxy for an RMI service. This proxy object talks with remote RMI services on behalf of the client.

Spring’s HTTP invoker : Spring HTTP invokers use the standard Java serialization mechanism to expose services through HTTP. Spring supports HTTP invoker infrastructure via HttpInvokerProxyFactoryBean and HttpInvokerServiceExporter. HttpInvokerServiceExporter that exports the specified service bean as HTTP invoker service endpoint, accessible via an HTTP invoker proxy. HttpInvokerProxyFactoryBean is a factory bean for HTTP invoker proxies.

Hessian : Hessian offers a binary HTTP-based remoting protocol. Spring supports Hessian via HessianProxyFactoryBean and the HessianServiceExporter.

Burlap : Burlap is Caucho’s XML-based alternative to Hessian. Spring provides support classes such as BurlapProxyFactoryBean and BurlapServiceExporter.

JAX-RPC : Spring provides remoting support for web services via JAX-RPC (J2EE 1.4's web service API).

JAX-WS : Spring provides remoting support for web services via JAX-WS (the successor of JAX-RPC, as introduced in Java EE 5 and Java 6).

JMS : The JMS remoting support in the Spring is provided by the JmsInvokerServiceExporter and JmsInvokerProxyFactoryBean classes.

This project shows how to develop Spring RMI Service & Client.

Used Technologies :

JDK 1.6.0_31
Spring 3.1.1
Maven 3.0.2