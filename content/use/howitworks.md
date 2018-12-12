+++
title = "How it works"
weight = 100
+++

kubefwd allows applications with connection strings like http://elasticsearch:9200/ or tcp://db:3306 to communicate into the remote cluster. It does this by adding 127.x IP addresses to your local loopback network interface, this way kubefwd can attach listeners on the same port as the Kubernetes service.