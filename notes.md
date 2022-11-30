Youtube: Exploring Chainlink VRF v2

- Source: https://youtu.be/rdJ5d8j1RCg
- Main difference between v1 and v2:
    - V1: fund contract w/ link
    - V2: fund subscription -> allow you to maintain a balance for multiple contracts

# Chainlink Docs
===

- Source: https://docs.chain.link/vrf/v2/subscription/ -> this plus the sub-articles
- Request & Receive data -> end to end diagram:
    - user subscription mgmt:
        - EOA -> subscription mgr
        - sub mgr send (LINK + gas) to VRF Coordinator
        - VRF Coordinator, add consumer -> now have funded VRF subscription and registered consumer SC
    - EOA interacts w/ Consuming Contract
        - EOA send gas to consuming contract -> consuming contract request random words from VRF Coordinator
