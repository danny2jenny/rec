# 简介

该服务与NVR、DVR进行通信，主要实现前端摄像机的预置位的调用，在告警时，可以控制摄像头的转动。
# 注册码

CNEKJPQZEX-eyJsaWNlbnNlSWQiOiJDTkVLSlBRWkVYIiwibGljZW5zZWVOYW1lIjoibGFuIHl1IiwiYXNzaWduZWVOYW1lIjoiIiwiYXNzaWduZWVFbWFpbCI6IiIsImxpY2Vuc2VSZXN0cmljdGlvbiI6IkZvciBlZHVjYXRpb25hbCB1c2Ugb25seSIsImNoZWNrQ29uY3VycmVudFVzZSI6ZmFsc2UsInByb2R1Y3RzIjpbeyJjb2RlIjoiQUMiLCJwYWlkVXBUbyI6IjIwMTgtMDEtMzAifSx7ImNvZGUiOiJETSIsInBhaWRVcFRvIjoiMjAxOC0wMS0zMCJ9LHsiY29kZSI6IklJIiwicGFpZFVwVG8iOiIyMDE4LTAxLTMwIn0seyJjb2RlIjoiUlMwIiwicGFpZFVwVG8iOiIyMDE4LTAxLTMwIn0seyJjb2RlIjoiV1MiLCJwYWlkVXBUbyI6IjIwMTgtMDEtMzAifSx7ImNvZGUiOiJEUE4iLCJwYWlkVXBUbyI6IjIwMTgtMDEtMzAifSx7ImNvZGUiOiJSQyIsInBhaWRVcFRvIjoiMjAxOC0wMS0zMCJ9LHsiY29kZSI6IlBTIiwicGFpZFVwVG8iOiIyMDE4LTAxLTMwIn0seyJjb2RlIjoiREMiLCJwYWlkVXBUbyI6IjIwMTgtMDEtMzAifSx7ImNvZGUiOiJEQiIsInBhaWRVcFRvIjoiMjAxOC0wMS0zMCJ9LHsiY29kZSI6IlJNIiwicGFpZFVwVG8iOiIyMDE4LTAxLTMwIn0seyJjb2RlIjoiUEMiLCJwYWlkVXBUbyI6IjIwMTgtMDEtMzAifSx7ImNvZGUiOiJDTCIsInBhaWRVcFRvIjoiMjAxOC0wMS0zMCJ9XSwiaGFzaCI6IjUxOTU1OTMvMCIsImdyYWNlUGVyaW9kRGF5cyI6MCwiYXV0b1Byb2xvbmdhdGVkIjpmYWxzZSwiaXNBdXRvUHJvbG9uZ2F0ZWQiOmZhbHNlfQ==-QOxwjWvRwJz6vo6J6adC3CJ4ukQHosbPYZ94URUVFna/Rbew8xK/M5gP3kAaPh6ZDveFdtMR1UBoumq3eCwXtXM3U3ls5noB4LIr+QplVlCj2pK5uNq7g/feyNyQcHpSXtvhIOnXDBLOecB05DOsxzm0p7ulGGJoAInmHeb9mc0eYjqc4RPpUQfh6HSYBnvEnKMlLF5bz4KEtzmsvvgA55CwzwQ3gRitm5Q/wUT7AQCBdjmBfNUjKVQL6TSjSDPp56FUdEs4Aab8LqstA2DIMbxocO64rvytmcUeIwu8Mi5uq87KQP5AQMSMYb59Inbd+dmVfx5cJo3fRS4/5s3/Hg==-MIIEPjCCAiagAwIBAgIBBTANBgkqhkiG9w0BAQsFADAYMRYwFAYDVQQDDA1KZXRQcm9maWxlIENBMB4XDTE1MTEwMjA4MjE0OFoXDTE4MTEwMTA4MjE0OFowETEPMA0GA1UEAwwGcHJvZDN5MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAxcQkq+zdxlR2mmRYBPzGbUNdMN6OaXiXzxIWtMEkrJMO/5oUfQJbLLuMSMK0QHFmaI37WShyxZcfRCidwXjot4zmNBKnlyHodDij/78TmVqFl8nOeD5+07B8VEaIu7c3E1N+e1doC6wht4I4+IEmtsPAdoaj5WCQVQbrI8KeT8M9VcBIWX7fD0fhexfg3ZRt0xqwMcXGNp3DdJHiO0rCdU+Itv7EmtnSVq9jBG1usMSFvMowR25mju2JcPFp1+I4ZI+FqgR8gyG8oiNDyNEoAbsR3lOpI7grUYSvkB/xVy/VoklPCK2h0f0GJxFjnye8NT1PAywoyl7RmiAVRE/EKwIDAQABo4GZMIGWMAkGA1UdEwQCMAAwHQYDVR0OBBYEFGEpG9oZGcfLMGNBkY7SgHiMGgTcMEgGA1UdIwRBMD+AFKOetkhnQhI2Qb1t4Lm0oFKLl/GzoRykGjAYMRYwFAYDVQQDDA1KZXRQcm9maWxlIENBggkA0myxg7KDeeEwEwYDVR0lBAwwCgYIKwYBBQUHAwEwCwYDVR0PBAQDAgWgMA0GCSqGSIb3DQEBCwUAA4ICAQC9WZuYgQedSuOc5TOUSrRigMw4/+wuC5EtZBfvdl4HT/8vzMW/oUlIP4YCvA0XKyBaCJ2iX+ZCDKoPfiYXiaSiH+HxAPV6J79vvouxKrWg2XV6ShFtPLP+0gPdGq3x9R3+kJbmAm8w+FOdlWqAfJrLvpzMGNeDU14YGXiZ9bVzmIQbwrBA+c/F4tlK/DV07dsNExihqFoibnqDiVNTGombaU2dDup2gwKdL81ua8EIcGNExHe82kjF4zwfadHk3bQVvbfdAwxcDy4xBjs3L4raPLU3yenSzr/OEur1+jfOxnQSmEcMXKXgrAQ9U55gwjcOFKrgOxEdek/Sk1VfOjvS+nuM4eyEruFMfaZHzoQiuw4IqgGc45ohFH0UUyjYcuFxxDSU9lMCv8qdHKm+wnPRb0l9l5vXsCBDuhAGYD6ss+Ga+aDY6f/qXZuUCEUOH3QUNbbCUlviSz6+GiRnt1kA9N2Qachl+2yBfaqUqr8h7Z2gsx5LcIf5kYNsqJ0GavXTVyWh7PYiKX4bs354ZQLUwwa/cG++2+wNWP+HtBhVxMRNTdVhSm38AknZlD+PTAsWGu9GyLmhti2EnVwGybSD2Dxmhxk3IPCkhKAK+pl0eWYGZWG3tJ9mZ7SowcXLWDFAk0lRJnKGFMTggrWjV8GYpw5bq23VmIqqDLgkNzuoog==

# 设计

* 可以兼容不同的NVR、DVR
* 独立服务，与REC通过HTTP服务器进行交互

可以采用libuv进行简单的TCP连接，和服务器进行通信

# 过程

* 通过 HTTP 接收 REC 发来的NVR、DVR配置
* 为每个NVR维护一个对象，实现与NVR的通信
* 接收 REC 发来的预置位调用，并通过与相应NVR的连接，实现对前端摄像机的控制

# 相关工具

libuv 电子书
http://luohaha.github.io/Chinese-uvbook/source/introduction.html

HttpServer libmicrohttpd

HttpRequrest libcurl

HashTable https://github.com/troydhanson/uthash   https://troydhanson.github.io/uthash/

#使用 MQTT 作为传输协议

服务器：https://mosquitto.org/
mosquitto_sub -v -t sensor 
mosquitto_pub -t sensor -m 13 

# 对比
https://www.predic8.com/activemq-hornetq-rabbitmq-apollo-qpid-comparison.htm

# MQTT 相关的资源

Spring 集成 http://docs.spring.io/spring-integration/reference/html/mqtt.html

相关的软件：https://github.com/mqtt/mqtt.github.io/wiki/software?id=software

一个嵌入式的服务：https://github.com/andsel/moquette

# MQTT 测试服务

iot.eclipse.org 1883

# Linux 服务

[Unit]
Description=MQTT Service
After=network.target

[Service]
User=rytec
Restart=always
Type=forking
ExecStart=/home/rytec/data/moquette/bin/moquette.sh

[Install]
WantedBy=multi-user.targe

连接到 /etc/systemd/system/multi-user.target.wants


