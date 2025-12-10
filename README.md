# base118
Tracking Live Base Block Height in Python &amp; Java  I’m experimenting with cross-language monitoring tools for Base. To start, here’s a minimal script that fetches the latest block using both Python and Java.  Python
from web3 import Web3

w3 = Web3(Web3.HTTPProvider("https://mainnet.base.org"))
print("Base block:", w3.eth.block_number)
Java
Web3j web3 = Web3j.build(new HttpService("https://mainnet.base.org"));
System.out.println("Base block: " + web3.ethBlockNumber().send().getBlockNumber());
