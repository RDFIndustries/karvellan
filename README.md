# Karvellan Manufacturing Protocol

Karvellan is an open, federated manufacturing protocol in development by RDF Industries, Inc. It gives consumers, businesses, design tools, and AI agents a common way to find manufacturers, ask whether a part can be made, request quotes, and place orders.

## Direct relationships between buyers and manufacturers

A buyer can work directly with the shop that will make the part. The shop can explain its process limits, suggest a design change, and quote its own price and lead time. The buyer can ask questions and compare offers before choosing a supplier.

Karvellan is designed to make a marketplace or broker optional. When buyers and shops choose to work directly, they can avoid intermediary fees that increase the buyer's price or reduce what the shop earns. A shop can describe its capabilities in a common format that multiple buyer tools can use.

## Federation and communication

- **Public and private federations.** A public federation can help shops reach new buyers. A private federation can serve an approved supplier network. Shops choose which capabilities to advertise and who can see them.
- **Peer-to-peer discovery.** Discovery peers share eligible capability information so a buyer's tool can find shops by criteria such as process, material, or part size.
- **Direct, point-to-point communication.** Once a buyer selects a shop to contact, the buyer and that shop are the parties to the exchange. Requests for quotes, drawings, feedback, and orders are addressed to the chosen counterpart. A relay can carry a message when needed without becoming a party to the transaction.

## Example workflow

1. A buyer's design tool discovers shops that can laser-cut a small batch of aluminum mounting plates.
2. The buyer sends a request for quote (RFQ) to selected shops, referencing a specific drawing revision and sharing the drawing with those shops.
3. One shop quotes the requested revision. Another suggests enlarging a slot to improve manufacturability. If the buyer revises the drawing, the original quote still refers to the earlier revision.
4. The buyer chooses a shop and places the order directly against the agreed quote and drawing revision.

## Project status

The specification is in development. The first reference implementation is planned to demonstrate a buyer discovering a shop, sending a revision-specific RFQ, and receiving a quote or a request for a design change.

## Get involved

RDF Industries, Inc. is developing Karvellan with independent implementations in mind. Feedback from manufacturers, buyers, and developers of CAD, procurement, or agent tools is welcome. If you have a workflow the protocol should account for, [open an issue](https://github.com/rdfindustries/karvellan/issues) and describe what each party needs to know or do.
