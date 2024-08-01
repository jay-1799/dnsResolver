# DNS Resolver

This project is a custom DNS resolver implemented in Go. It listens for DNS queries on UDP port 53 and resolves them by querying the root DNS servers.

## Table of Contents

- [Description](#description)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Testing](#testing)

## Description

This DNS resolver project is designed to handle DNS queries and resolve them by recursively querying root DNS servers. It demonstrates the basics of DNS query handling, packet parsing, and network communication in Go.

## Features

- Listens for DNS queries on UDP port 53
- Parses and handles DNS queries
- Recursively queries root DNS servers to resolve domain names
- Supports caching of DNS responses

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/yourusername/dns-resolver.git
   cd dns-resolver
   ```

2. Install the necessary Go packages:

   ```sh
   go mod tidy
   ```

## Usage

1. Start the DNS resolver:

   ```sh
   go run main.go
   ```

2. The resolver will start listening on UDP port 53.

3. To test the resolver, you can use tools like `dig` or `nslookup` to query the resolver for domain names.

   - Using `dig`:

     ```sh
     dig @localhost google.com
     ```

   - Using `nslookup`:

     ```sh
     nslookup google.com localhost
     ```

## Testing

To test the DNS resolver with a query for `google.com`:

1. Ensure DNS resolver is running by executing the `main.go` file.
2. Open a new terminal and use `dig` or `nslookup`:

   - Using `dig`:

     ```sh
     dig @localhost google.com
     ```

   - Using `nslookup`:

     ```sh
     nslookup google.com localhost
     ```
