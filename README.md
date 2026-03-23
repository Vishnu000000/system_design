# system_design

BackStory, You have a acode that is very good and useful for some reason. So You thought to sell that for soem money so else can use it's services.
Bu turrns out you have only 1 desktop, how you cans ell to many people.

It's simple, You should contact AWS(Amazon Web Services) and tell them, I need more desktop or computer to run my code. this will be viable.

Now If Computers are limited, might not fulfilll your whole goal criteria.

If You choose computer that are bigger and can finish requests very quickly, This is called **Vertical Scaling**

If You choose computer that are more, So that you can handle more no of requests in big picture, This is called **Horizontal Scaling**

You can see key differences between horizontal and vertical scaling

<img width="1580" height="928" alt="image" src="https://github.com/user-attachments/assets/0815a26d-d483-4f43-bf8f-42c25f3578c7" />

In real life, We use the combination of both as both have advantages, as we underlines. We make best out of it.

Money wise, we try to avoid single point of failure. Choosing more machines(which is horizental scaling), also make machines bigger(Vertical Scaling)

Load Balancing is lie the consistent hashing, We have n servers and make it as equal no of request as possible

A server is taking load of some k requests, Mostly keeping the no of requests at same level as better as possible.

when a server fails, what it happen is k requests and it already got will moved to clockwise nearest server and given to it, In this way, the no of requests per server might change for certain and load becomes high. It is alright

The efficency won't go away for the reason.

There is some servers/some pizzashop chain, namedly have 5 pizza shop. Now there one load balancer like a central point, that takes the a api call to other 5 shops liek knwing whetther they are alive or nott. It is kind of working or not rrequest.


No wto have persistent non corrupted database that s not specifc to any server, we introduce a database, which store the orders and seer and all the info like whether a order is done or not delivered yet.

Now, each server/pizzashop got some many orders, some of offlien bases and another is delivery type.

when a server or pizza shop closes, You can make the offline orders null, But deliveries can be split across and send to othe pizza shops, in this customer experince won't be affected much, this middle balancer is very importnat ffor this to function.
