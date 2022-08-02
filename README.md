# Module_18
PREMISE: "You’re a fintech engineer who’s working at one of the five largest banks in the world. You were recently promoted to act as the lead developer on their decentralized finance team. Your task is to build a blockchain-based ledger system, complete with a user-friendly web interface. This ledger should allow partner banks to conduct financial transactions (that is, to transfer money between senders and receivers) and to verify the integrity of the data in the ledger."

---

## Technologies & Imports

Required programs, libraries, systems, and overall dependencies:

Python (version 3.0 or later)
<br>
`streamlit`
<br>
`dataclass`
<br>
`typing`
<br>
`pandas`
<br>
`hashlib`

---

## Usage

### Setting up dataclasses:

```python
@dataclass
class Record:

    sender: str
    receiver: str
    amount: float = 0
```
### Methods:

```python
    def hash_block(self):
        sha = hashlib.sha256()

        record = str(self.record).encode()
        sha.update(record)

        creator_id = str(self.creator_id).encode()
        sha.update(creator_id)

        timestamp = str(self.timestamp).encode()
        sha.update(timestamp)

        prev_hash = str(self.prev_hash).encode()
        sha.update(prev_hash)

        nonce = str(self.nonce).encode()
        sha.update(nonce)

        return sha.hexdigest()
```
## Screenshots

![Screenshot of Plot](https://github.com/hyppolite314/Module_18/blob/main/Screen%20Shot%202022-08-01%20at%2010.50.39%20PM.png)
![Screenshot of Plot](https://github.com/hyppolite314/Module_18/blob/main/Screen%20Shot%202022-08-01%20at%2010.50.47%20PM.png)
![Screenshot of Plot](https://github.com/hyppolite314/Module_18/blob/main/Screen%20Shot%202022-08-01%20at%2010.53.04%20PM.png)

---

## Contributors

Reginald Hyppolite
https://www.linkedin.com/in/reginald-hyppolite-nyc/

BIG THANKS to all the great TAs and Professor Vinicio DeSola

---

## License
MIT
Free open.ware for a better world.