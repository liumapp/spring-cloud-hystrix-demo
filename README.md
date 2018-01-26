# spring-cloud-hystrix-demo
Simple demo for Spring Cloud Hystrix

## how to use
* start hystrix-demo-eureka first

    * then view http://localhost:1234

    * you can find the eureka pannel in this page

* start client A and client B , they are named hystrix-demo-client-a and hystrix-demo-clint-b

    * then you can find they are registed in eureka pannel

    * client A is listening on 8081 and client B is listening on 8082

* start customer , it was named hystrix-demo-customer

* view http://localhost:8083

    * keep refresh the page , you can find client A and client B is offering their server .
    
    * now , cancel client B's server (just simple kill it )
    
    * keep refresh the page , you can find hystrix can find that client B have error until eureka remove B from the server's list . 