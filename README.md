## Environmental Setup:

1. go get github.com/davecgh/go-spew/spew

2. go get github.com/gorilla/mux

3. go get github.com/joho/godotenv

## Peer to peer environmental setup:

1. go get -d github.com/libp2p/go-libp2p/...

2. navigate to the cloned directory from above

3. make

4. make deps (If it shows error use sudo and/or add the path to environmental variable "Directory to go where library is installed"\go\bin)

5. create a directory under examples called p2p with

mkdir ./examples/p2p.

We are gonna keep the code in that directory. That means the code directory should be go/github.com/libp2p/go-libp2p/examples/p2p/main_old.go 


## Build and Run:

Before running the code go to the root directory of go-libp2p and run make deps again

1. It's a rough application using P2P platform. To run the first client use the command "go run main_old.go -l 10000 -secio". If it runs successfully it will provide the command how to run the next peer. A sample command is following. "go run main_old.go -l 10001 -d /ip4/127.0.0.1/tcp/10001/ipfs/Qmco8oyCJASAwKNgthDtkjBZtEZTbhvuW6oWeLurtAJLJK -secio".

2. When you run two or more client, in the transaction record put an integer value. In the nonce value also put an integer value. For another peer put a different integer vlaue for both nonce and transaction.

3. It's very important that the transaction record and nonce should be different for different peer in each epoch.
