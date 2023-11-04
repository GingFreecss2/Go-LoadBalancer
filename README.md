# Simple Go Load Balancer

This is a simple load balancer implemented in Go, designed to distribute incoming HTTP requests among multiple backend servers. The load balancer uses a round-robin algorithm to evenly distribute requests to the available backend servers.

## Table of Contents
- [Simple Go Load Balancer](#simple-go-load-balancer)
  - [Table of Contents](#table-of-contents)
  - [Architecture](#architecture)
  - [Getting Started](#getting-started)
  - [Usage](#usage)
  - [Contributing](#contributing)

## Architecture

![Load Balancer Architecture](/architecture.PNG)

The architecture of the load balancer is straightforward. It includes the following components:

- **Load Balancer**: The main application responsible for accepting incoming HTTP requests and distributing them to backend servers.

- **Backend Servers**: Multiple backend servers that host the actual services. In the example, three backend servers are defined, serving content from Facebook, Bing, and DuckDuckGo.

- **Round-Robin Algorithm**: The load balancer employs a round-robin algorithm to evenly distribute incoming requests among the available backend servers. This algorithm cycles through the servers in a circular fashion, ensuring that each server receives its fair share of traffic.

## Getting Started

To get started with this load balancer, make sure you have Go installed on your system. You can follow these steps:

1. Clone this repository to your local machine.

```bash
git clone https://github.com/GingFreecss2/Go-LoadBalancer.git
cd Go-LoadBalancer
```

2. Build and run the load balancer.
``` bash
Copy code
go run main.go
```

The load balancer will start serving requests on localhost:8000. You can configure the backend servers and the port in the source code.

## Usage
The load balancer will listen for incoming HTTP requests and distribute them to the backend servers using the round-robin algorithm. To use the load balancer, send HTTP requests to the load balancer's address, and it will forward them to the backend servers.

## Contributing
If you want to contribute to this project, please follow these steps:

1. Fork the repository.

2. Create a new branch for your feature or bug fix.

3. Make your changes and commit them.

4. Push the changes to your fork.

5. Create a pull request, describing the changes you made and why they are necessary.
