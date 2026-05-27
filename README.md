# lastmile-route-optimiser
CVRP-based last-mile delivery route optimiser using OR-Tools and OSMnx — models radius-cost-SLA tradeoffs for dark-store catchment zones.
# Last-Mile Delivery Route Optimiser

Formulates last-mile delivery scheduling as a Capacitated Vehicle Routing 
Problem (CVRP) to optimise dispatch sequences and minimise delivery cost 
without compromising SLA.

## Tech Stack
Python, OR-Tools, OSMnx, NetworkX, Folium

## Key Results
- 26% reduction in average simulated delivery time vs nearest-neighbour heuristic
- Radius-cost-SLA trade-off curve identifying optimal dark-store serviceable zone
- Interactive Folium heatmap surfacing peak-hour dispatch inefficiencies

## Approach
- Formulated CVRP using Google OR-Tools for batches of 8-12 concurrent orders
- Integrated real road-network data via OSMnx for peak and off-peak travel-time matrices
- Modelled delivery radius impact on SLA adherence and cost-per-order
- Overlaid order density and idle-rider positions on heatmap for dispatch analysis
