The Graph is a decentralized query protocol and indexing service for the blockchain. It allows developers to easily track events being emitted from smart contracts on various networks, and write custom data transformation scripts, which are run in real time. The data is also made available through a simple GraphQL API which developers can then use to display things on their frontends.

How it Works

1) A dApp sends a transaction and some data gets stored in the smart contract. 2/ This smart contract then emits one or more events.
2) Graph's node keeps scanning Ethereum for new blocks and the data for your subgraph that these blocks may contain.
3) If the node finds an event you were looking for and defined in your subgraph, it runs the data transformation scripts (mappings) you defined. The mapping is a WASM (Web assembly) module that creates or updates data Entities on the Graph Nodes in response to the event.
4) We can query the Graph's node for this data using the GraphQL Endpoint
(Referenced From The Graph’s website)

This is a Next.js project bootstrapped with create-next-app.

Getting Started

First, run the development server:

npm run dev
# or
yarn dev


Open http://localhost:3000 with your browser to see the result.

You can start editing the page by modifying pages/index.js. The page auto-updates as you edit the file.

API routes can be accessed on http://localhost:3000/api/hello. This endpoint can be edited in pages/api/hello.js.

The pages/api directory is mapped to /api/*. Files in this directory are treated as API routes instead of React pages.
