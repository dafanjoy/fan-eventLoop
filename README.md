#fan-evenloop  
参照Netty中EventLoop的事件分发线程模型，供学习参考使用  
特点：  
>1、结合事件监听机制，统一内部消息模型，为分发策略的制定与无锁化提供基础;   
2、线程内部结合阻塞队列循环执行，保证同一EventLoo中数据处理的有序性；  
3、针对需要线程同步数据，可根据一定的分发策略保证由同一线程执行，实现无锁化；  
