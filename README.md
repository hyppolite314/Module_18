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

Setting up dataclasses:

```python
@dataclass
class Record:

    sender: str
    receiver: str
    amount: float = 0
```
![Screenshot of Plot](https://github.com/hyppolite314/geo_analysis_realty/blob/main/inter_plot.png?raw=true)

GeoViews via `hvplot.points`

```python
all_neighborhoods_plot = all_neighborhoods_df.hvplot.points(
    'Lon',
    'Lat',
    geo=True,
    size='sale_price_sqr_foot',
    scale=1,
    color='gross_rent',
    tiles='OSM',
    frame_width=700,
    frame_height=500,
    title = "Average Sales Price per SqFt (2010-2016)"
    )

all_neighborhoods_plot
```
![Screenshot of Plot](https://github.com/hyppolite314/geo_analysis_realty/blob/main/geo_view.png?raw=true)

---

## Contributors

Reginald Hyppolite
https://www.linkedin.com/in/reginald-hyppolite-nyc/

BIG THANKS to all the great TAs and Professor Vinicio DeSola

---

## License
MIT
Free open.ware for a better world.