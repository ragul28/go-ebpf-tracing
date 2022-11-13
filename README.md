# Go eBPF tracing

Sample getting started project of eBPF tracing basics 

## Prerequisites

* Golang 1.19+
* bcc

## Running

* Build server & eBPF tracer   
    ```sh
    make build_srv
    make build_trace
    ```

* Run webserver on first terminal
    ```sh
    ./server
    ```

* Run webserver on 2nd terminal
    ```sh
    ./trace ./server
    ```

* Curl server running on localhost, trace the call
    ```
    curl localhost:8080
    ```