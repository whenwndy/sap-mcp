# SAP ERP Mock MCP (synthetic demo)
A read-only SAP-style ERP MCP server for a fictional premium appliance distributor. **Not affiliated with SAP. No real ERP connection or customer data.**

## Run
```bash
npm install
npm start
```
HTTP MCP endpoint: `POST /mcp` (Streamable HTTP); health: `GET /health`. Set `PORT` for hosting.

## Tools
`search_products`, `get_inventory_levels`, `search_sales_orders`, `get_sales_order`, `search_purchase_orders`, `get_purchase_order`, `get_project_financials`, `get_project_appliances`, `get_supplier_performance`, `get_sales_summary`, `get_inventory_risks`.

## Example prompts
- How many Induction Pro 920 cooktops are available by warehouse?
- What orders and deliveries are associated with Marina Heights?
- Which suppliers have the longest lead times?
- Show open purchase orders.
- Which SKUs have low available inventory?

## Important
All data is synthetic and fictional. This is a small seed dataset, not a production SAP API emulator. The server has **no authentication**: do not deploy it publicly without adding access controls, rate limiting, and an appropriate authorization layer. The MCP tools are read-only.
