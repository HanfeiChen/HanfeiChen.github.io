---
layout: post
title:  "HTTP Proxy"
author: Hanfei Chen
subtitle: Python
categories: [ Travel ]
image: assets/images/internet.jpg
---

The HTTP proxy works at the TCP level by modifying the traffic sent from the user’s browser and forwarding it onto the remote server.

For unencrypted HTTP requests, the proxy simply forwards the HTTP request to the web server, and sends back the HTTP response it gets back from the web server. However, some modifications to the request must be made sometimes, because the HTTP protocols (1.0 and 1.1) require different structures in certain parts of the request depending on whether a proxy is used.

For HTTPS websites, the browser will first send a CONNECT request to the server to set up an SSL tunnel. The proxy will then set up a tunnel with the browser and another tunnel with the server, and just keep forwarding the encrypted traffic. It is actually interesting to see that the browsers send additional requests to OCSP servers to verify the validity of the server’s certificate.

In the end, my proxy was able to stream HD YouTube videos, and concurrently load huge websites like CNN.com, etc.
