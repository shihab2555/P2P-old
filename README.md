It's a rough application using P2P platform. To run the first client use the command "go run main_old.go -l 10000 -secio". If it runs successfully it will provide the command how to run the next peer. A sample command is following. "go run main_old.go -l 10001 -d /ip4/127.0.0.1/tcp/10001/ipfs/Qmco8oyCJASAwKNgthDtkjBZtEZTbhvuW6oWeLurtAJLJK -secio".


When you run two or more client, in the transaction record put an integer value. In the nonce value also put an integer value. For another peer put a different integer vlaue for both nonce and transaction.


It's very important that the transaction record and nonce should be different for different peer in each epoch.
