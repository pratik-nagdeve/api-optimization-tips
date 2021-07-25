# api-optimization-cheatsheet

##optimization of api:
---------------------------
    
1. representation of payload (xml, json eg:serializer- deserialization may cost most)
2. try preheating connections eg tcp connection(handshake and connection may cost )
3. consider h2 ie http2 if you are sending lot of requests in parallel
4. beware tcp connection , cost of retransmission(tcp meltdown problem), tcp headofline walking
5. check your proxies (eg. reverse proxy, cashing layers or load balancers)
6. avoid large payloads (serializer, xml, json)
7. watchout for the client side proccessing
