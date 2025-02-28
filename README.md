# aleo_learn_earn_workshop1
My first Aleo zkworkshop was building an auction program where user place bid on an amount greater than 5000

# DEPLOYMENT
Deployment ID: at1nwkjvdnwefx4hcm3k95v342mcwnspt9wxlc573pafypd9mpg2cxquw24h8
Program Deployment URL: https://testnet.aleo.info/program/auction_bidding01.aleo

![Screenshot from 2025-02-28 23-26-09](https://github.com/user-attachments/assets/9b325299-ad96-47b8-bcbd-0de8ea525e26)


# EXECUTION 
transaction ID: at1are5upxvwzhqv8qczgek4m99q3nuefgnsmcjjt7gfam48gwr55fqwyguws
![Screenshot from 2025-02-28 23-36-01](https://github.com/user-attachments/assets/f2997c81-5291-41a6-9124-3e07c140b7b7)


# Overall Flow of the Auction
1. Users Place Bids

- A user calls place_bid(bidder, amount), ensuring that they meet the minimum bid amount.
- The bid is stored as a Bid record with the auctioneer as the owner.

2. Auctioneer Resolves the Auction

- Calls resolve(first, second), selecting the higher bid.
- If tied, the first bid is chosen.

3. Finalizing and Transferring Ownership

- The auctioneer calls finish(bid), marking the winning bid.
- Ownership of the bid record transfers to the winning bidder.
