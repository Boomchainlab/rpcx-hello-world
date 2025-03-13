rpcx-hello-world

A simple “Hello World” example using the rpcx framework for high-performance RPC in Go. This project demonstrates:
	•	Basic RPC communication (server & client).
	•	Authentication using request metadata (token-based).
	•	Middleware for logging requests and responses.
	•	Bidirectional streaming RPC for continuous message exchange.

🚀 Features

✔ Lightweight and fast RPC communication.
✔ Secure authentication using metadata tokens.
✔ Logging middleware for monitoring requests.
✔ Support for bidirectional streaming.


🛠 Installation

Ensure you have Go installed (version 1.18+ recommended).

	1.	Clone the repository:
 git clone https://github.com/Boomchainlab/rpcx-hello-world.git
cd rpcx-hello-world

2.	Install dependencies:
   go mod tidy

   📡 Running the Server & Client
   1️⃣ Start the Server
   go run server.go

  2️⃣ Run the Client
  go run client.go

  📜 Code Explanation
  Server (server.go)
	•	Defines an HelloService struct with an RPC method Say.
	•	Uses metadata authentication to verify client requests.
	•	Implements logging middleware for request tracking.
	•	Starts an rpcx server on tcp://127.0.0.1:8972.

Client (client.go)
	•	Connects to the server using rpcx client.
	•	Sends an authentication token via metadata.
	•	Calls the Say method and prints the response.

🔌 Example Output
Response from server: Hello, RPCX!
Server Logs:
Incoming request: RPCX
Response sent: Hello, RPCX!

📡 Streaming Support (Coming Soon)

The project will be updated to include bidirectional streaming using rpcx’s Stream functionality.

🌟 Contributing

Feel free to fork the repository, open an issue, or submit a pull request.


