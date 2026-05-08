# Plex to Odoo field mapping - wade_real_estate

## Source datasets found

| Plex file | Data rows |
|---|---:|
| `01_mdm_v1_parts_full_history.csv` | 0 |
| `02_mdm_v1_customers_full_history.csv` | 2 |
| `03_mdm_v1_contacts_full_history.csv` | 0 |
| `04_mdm_v1_suppliers_full_history.csv` | 23 |
| `05_mdm_v1_operations_full_history.csv` | 8 |
| `06_mdm_v1_employees_full_history.csv` | 0 |
| `07_mdm_v1_buildings_full_history.csv` | 1 |
| `08_mdm_v1_supply_items_full_history.csv` | 0 |
| `09_inventory_v1_inventory_definitions_locations_full_history.csv` | 0 |
| `10_inventory_v1_inventory_tracking_containers_full_history.csv` | 0 |
| `11_inventory_v1_inventory_tracking_lots_full_history.csv` | 0 |
| `12_purchasing_v1_item_suppliers_full_history.csv` | 0 |
| `13_purchasing_v1_approved_suppliers_full_history.csv` | 0 |
| `14_sales_v1_price_adjustments_full_history.csv` | 0 |
| `15_sales_v1_orders_full_history.csv` | 0 |
| `16_purchasing_v1_purchase_orders_full_history.csv` | 0 |
| `17_purchasing_v1_receipts_full_history.csv` | 0 |
| `18_accounting_v1_journal_entries_full_history.csv` | 215 |
| `19_accounting_v1_ap_invoices_full_history.csv` | 623 |
| `20_accounting_v1_ar_invoices_full_history.csv` | 129 |
| `21_shipping_v1_beta1_transfer_orders_full_history.csv` | 0 |
| `22_inventory_v1_inventory_history_container_adjustments_full_history.csv` | 0 |
| `23_engineering_v1_boms_components_full_history.csv` | 0 |

## Mapping by template

Rules used:
- Direct = same/close field name found in Plex file header.
- Derived/Lookup = needs transform, external id mapping, or relation lookup.
- Empty rows must be removed before import (no blank data rows).

### `01_Bill_of_Materials`

Source file(s): `23_engineering_v1_boms_components_full_history.csv`, `05_mdm_v1_operations_full_history.csv`, `01_mdm_v1_parts_full_history.csv`

#### Sheet `mrp_bom`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `product_tmpl_id` |  | Derived/Lookup |
| `product_id` | `id` | Direct |
| `product_qty` |  | Derived/Lookup |
| `product_uom_id` |  | Derived/Lookup |
| `code` | `code` | Direct |
| `type` | `type` | Direct |
| `company_id` |  | Derived/Lookup |
| `sequence` |  | Derived/Lookup |
| `active` |  | Derived/Lookup |
| `ready_to_produce` |  | Derived/Lookup |
| `consumption` |  | Derived/Lookup |
| `allow_operation_dependencies` |  | Derived/Lookup |
| `picking_type_id` |  | Derived/Lookup |
| `produce_delay` |  | Derived/Lookup |
| `days_to_prepare_mo` |  | Derived/Lookup |
| `enable_batch_size` |  | Derived/Lookup |
| `batch_size` |  | Derived/Lookup |

#### Sheet `mrp_bom_line`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `bom_id` |  | Derived/Lookup |
| `sequence` |  | Derived/Lookup |
| `product_id` | `id` | Direct |
| `product_qty` |  | Derived/Lookup |
| `product_uom_id` |  | Derived/Lookup |
| `bom_product_template_attribute_value_ids` |  | Derived/Lookup |
| `operation_id` |  | Derived/Lookup |

#### Sheet `mrp_routing_workcenter`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `bom_id` |  | Derived/Lookup |
| `sequence` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `workcenter_id` |  | Derived/Lookup |
| `bom_product_template_attribute_value_ids` |  | Derived/Lookup |
| `cost_mode` |  | Derived/Lookup |
| `time_mode` |  | Derived/Lookup |
| `time_cycle_manual` |  | Derived/Lookup |
| `time_mode_batch` |  | Derived/Lookup |
| `blocked_by_operation_ids` |  | Derived/Lookup |
| `active` |  | Derived/Lookup |
| `company_id` |  | Derived/Lookup |

#### Sheet `mrp_bom_byproduct`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `bom_id` |  | Derived/Lookup |
| `sequence` |  | Derived/Lookup |
| `product_id` | `id` | Direct |
| `product_qty` |  | Derived/Lookup |
| `product_uom_id` |  | Derived/Lookup |
| `cost_share` |  | Derived/Lookup |
| `operation_id` |  | Derived/Lookup |
| `bom_product_template_attribute_value_ids` |  | Derived/Lookup |

### `02_Chart_of_Accounts`

Source file(s): `18_accounting_v1_journal_entries_full_history.csv`

#### Sheet `account_account`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `name` | `description` | Direct |
| `code` |  | Derived/Lookup |
| `account_type` |  | Derived/Lookup |
| `reconcile` |  | Derived/Lookup |
| `company_ids` |  | Derived/Lookup |
| `currency_id` | `currency` | Direct |
| `tag_ids` |  | Derived/Lookup |
| `tax_ids` |  | Derived/Lookup |
| `active` |  | Derived/Lookup |
| `non_trade` |  | Derived/Lookup |
| `description` | `description` | Direct |

### `03_Taxes`

Source file(s): _No direct Plex source file matched in this company folder._

#### Sheet `account_tax_group`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `sequence` |  | Derived/Lookup |
| `country_id` |  | Derived/Lookup |

#### Sheet `account_tax`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `amount_type` |  | Derived/Lookup |
| `active` |  | Derived/Lookup |
| `type_tax_use` |  | Derived/Lookup |
| `tax_scope` |  | Derived/Lookup |
| `amount` |  | Derived/Lookup |
| `fiscal_position_ids` |  | Derived/Lookup |
| `original_tax_ids` |  | Derived/Lookup |
| `invoice_label` |  | Derived/Lookup |
| `description` |  | Derived/Lookup |
| `tax_group_id` |  | Derived/Lookup |
| `analytic` |  | Derived/Lookup |
| `company_id` |  | Derived/Lookup |
| `country_id` |  | Derived/Lookup |
| `invoice_legal_notes` |  | Derived/Lookup |
| `price_include_override` |  | Derived/Lookup |
| `include_base_amount` |  | Derived/Lookup |
| `tax_exigibility` |  | Derived/Lookup |
| `cash_basis_transition_account_id` |  | Derived/Lookup |
| `children_tax_ids` |  | Derived/Lookup |

#### Sheet `repartition_invoice`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `tax_id` |  | Derived/Lookup |
| `document_type` |  | Derived/Lookup |
| `sequence` |  | Derived/Lookup |
| `factor_percent` |  | Derived/Lookup |
| `repartition_type` |  | Derived/Lookup |
| `account_id` |  | Derived/Lookup |
| `tag_ids` |  | Derived/Lookup |
| `use_in_tax_closing` |  | Derived/Lookup |

#### Sheet `repartition_refund`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `tax_id` |  | Derived/Lookup |
| `document_type` |  | Derived/Lookup |
| `sequence` |  | Derived/Lookup |
| `factor_percent` |  | Derived/Lookup |
| `repartition_type` |  | Derived/Lookup |
| `account_id` |  | Derived/Lookup |
| `tag_ids` |  | Derived/Lookup |
| `use_in_tax_closing` |  | Derived/Lookup |

### `04_Fiscal_Positions`

Source file(s): _No direct Plex source file matched in this company folder._

#### Sheet `account_fiscal_position`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `company_id` |  | Derived/Lookup |
| `auto_apply` |  | Derived/Lookup |
| `vat_required` |  | Derived/Lookup |
| `foreign_vat` |  | Derived/Lookup |
| `country_group_id` |  | Derived/Lookup |
| `country_id` |  | Derived/Lookup |
| `state_ids` |  | Derived/Lookup |
| `zip_from` |  | Derived/Lookup |
| `zip_to` |  | Derived/Lookup |
| `tax_ids` |  | Derived/Lookup |
| `note` |  | Derived/Lookup |
| `active` |  | Derived/Lookup |

#### Sheet `account_fiscal_position_account`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `position_id` |  | Derived/Lookup |
| `account_src_id` |  | Derived/Lookup |
| `account_dest_id` |  | Derived/Lookup |

### `05_Journals_and_Bank_Accounts`

Source file(s): `18_accounting_v1_journal_entries_full_history.csv`, `19_accounting_v1_ap_invoices_full_history.csv`, `20_accounting_v1_ar_invoices_full_history.csv`

#### Sheet `res_partner_bank`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `partner_id` | `supplierId` | Direct |
| `acc_number` |  | Derived/Lookup |
| `bank_id` |  | Derived/Lookup |
| `acc_holder_name` |  | Derived/Lookup |
| `currency_id` | `currencyAmount` | Direct |

#### Sheet `account_journal`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `name` | `description` | Direct |
| `type` | `type` | Direct |
| `code` | `externalReferenceCode` | Direct |
| `company_id` | `intercompany` | Direct |
| `default_account_id` |  | Derived/Lookup |
| `suspense_account_id` |  | Derived/Lookup |
| `bank_account_id` |  | Derived/Lookup |
| `currency_id` | `currencyAmount` | Direct |
| `sequence` |  | Derived/Lookup |
| `active` |  | Derived/Lookup |

### `06_Analytic_Accounts`

Source file(s): _No direct Plex source file matched in this company folder._

#### Sheet `account_analytic_plan`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `parent_id` |  | Derived/Lookup |

#### Sheet `account_analytic_account`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `code` |  | Derived/Lookup |
| `plan_id` |  | Derived/Lookup |
| `company_id` |  | Derived/Lookup |
| `partner_id` |  | Derived/Lookup |

### `07_Customers_and_Contacts`

Source file(s): `02_mdm_v1_customers_full_history.csv`, `03_mdm_v1_contacts_full_history.csv`

#### Sheet `customer_company`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `name` | `name` | Direct |
| `is_company` |  | Derived/Lookup |
| `vat` |  | Derived/Lookup |
| `email` | `email` | Direct |
| `phone` | `phone` | Direct |
| `mobile` |  | Derived/Lookup |
| `street` |  | Derived/Lookup |
| `street2` |  | Derived/Lookup |
| `city` |  | Derived/Lookup |
| `zip` |  | Derived/Lookup |
| `country_id` |  | Derived/Lookup |
| `state_id` |  | Derived/Lookup |
| `lang` |  | Derived/Lookup |
| `company_id` |  | Derived/Lookup |
| `ref` | `code` | Direct |

#### Sheet `customer_children`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `parent_id` |  | Derived/Lookup |
| `type` | `type` | Direct |
| `name` | `name` | Direct |
| `email` | `email` | Direct |
| `phone` | `phone` | Direct |
| `street` |  | Derived/Lookup |
| `street2` |  | Derived/Lookup |
| `city` |  | Derived/Lookup |
| `zip` |  | Derived/Lookup |
| `country_id` |  | Derived/Lookup |
| `state_id` |  | Derived/Lookup |
| `company_id` |  | Derived/Lookup |

### `08_Customer_Accounting_and_Pricelist`

Source file(s): `20_accounting_v1_ar_invoices_full_history.csv`, `15_sales_v1_orders_full_history.csv`

#### Sheet `res_partner_properties`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `property_account_receivable_id` |  | Derived/Lookup |
| `property_account_payable_id` |  | Derived/Lookup |
| `property_account_position_id` |  | Derived/Lookup |
| `property_payment_term_id` |  | Derived/Lookup |
| `property_supplier_payment_term_id` |  | Derived/Lookup |
| `property_product_pricelist` |  | Derived/Lookup |

### `09_Vendors`

Source file(s): `04_mdm_v1_suppliers_full_history.csv`, `19_accounting_v1_ap_invoices_full_history.csv`

#### Sheet `vendor_company`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `name` | `name` | Direct |
| `is_company` |  | Derived/Lookup |
| `supplier_rank` |  | Derived/Lookup |
| `vat` | `taxId` | Direct |
| `email` |  | Derived/Lookup |
| `phone` |  | Derived/Lookup |
| `street` |  | Derived/Lookup |
| `street2` |  | Derived/Lookup |
| `city` |  | Derived/Lookup |
| `zip` |  | Derived/Lookup |
| `country_id` |  | Derived/Lookup |
| `state_id` |  | Derived/Lookup |
| `company_id` | `intercompany` | Direct |
| `ref` | `code` | Direct |

### `10_Product_Category_and_UoM`

Source file(s): `01_mdm_v1_parts_full_history.csv`, `08_mdm_v1_supply_items_full_history.csv`

#### Sheet `product_category`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `parent_id` |  | Derived/Lookup |

#### Sheet `uom_uom`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `relative_uom_id` |  | Derived/Lookup |
| `relative_factor` |  | Derived/Lookup |
| `active` |  | Derived/Lookup |

### `11_Products`

Source file(s): `01_mdm_v1_parts_full_history.csv`, `08_mdm_v1_supply_items_full_history.csv`

#### Sheet `product_template`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `type` |  | Derived/Lookup |
| `is_storable` |  | Derived/Lookup |
| `tracking` |  | Derived/Lookup |
| `categ_id` |  | Derived/Lookup |
| `uom_id` |  | Derived/Lookup |
| `uom_po_id` |  | Derived/Lookup |
| `sale_ok` |  | Derived/Lookup |
| `purchase_ok` |  | Derived/Lookup |
| `list_price` |  | Derived/Lookup |
| `taxes_id` |  | Derived/Lookup |
| `supplier_taxes_id` |  | Derived/Lookup |
| `default_code` |  | Derived/Lookup |
| `barcode` |  | Derived/Lookup |
| `route_ids` |  | Derived/Lookup |

#### Sheet `product_product`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `product_tmpl_id` |  | Derived/Lookup |
| `default_code` |  | Derived/Lookup |
| `barcode` |  | Derived/Lookup |
| `standard_price` |  | Derived/Lookup |

### `12_Sales_Pricelists`

Source file(s): `14_sales_v1_price_adjustments_full_history.csv`

#### Sheet `product_pricelist`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `currency_id` |  | Derived/Lookup |
| `company_id` |  | Derived/Lookup |
| `active` |  | Derived/Lookup |
| `sequence` |  | Derived/Lookup |

#### Sheet `product_pricelist_item`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `pricelist_id` |  | Derived/Lookup |
| `applied_on` |  | Derived/Lookup |
| `compute_price` |  | Derived/Lookup |
| `fixed_price` |  | Derived/Lookup |
| `percent_price` |  | Derived/Lookup |
| `min_quantity` |  | Derived/Lookup |
| `product_id` |  | Derived/Lookup |
| `product_tmpl_id` |  | Derived/Lookup |
| `categ_id` |  | Derived/Lookup |
| `date_start` |  | Derived/Lookup |
| `date_end` |  | Derived/Lookup |

### `13_Work_Centers`

Source file(s): `05_mdm_v1_operations_full_history.csv`

#### Sheet `mrp_workcenter`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `name` |  | Derived/Lookup |
| `code` | `code` | Direct |
| `company_id` |  | Derived/Lookup |
| `sequence` |  | Derived/Lookup |
| `active` |  | Derived/Lookup |
| `costs_hour` |  | Derived/Lookup |
| `time_start` |  | Derived/Lookup |
| `time_stop` |  | Derived/Lookup |
| `time_efficiency` |  | Derived/Lookup |

### `15_Warehouses_and_Locations`

Source file(s): `07_mdm_v1_buildings_full_history.csv`, `09_inventory_v1_inventory_definitions_locations_full_history.csv`

#### Sheet `stock_warehouse`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `name` | `name` | Direct |
| `code` | `oldBuildingCode` | Direct |
| `company_id` |  | Derived/Lookup |

#### Sheet `stock_location`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` | `id` | Direct |
| `name` | `name` | Direct |
| `location_id` |  | Derived/Lookup |
| `usage` |  | Derived/Lookup |
| `company_id` |  | Derived/Lookup |

### `16_Lots_and_Inventory_Quant`

Source file(s): `10_inventory_v1_inventory_tracking_containers_full_history.csv`, `11_inventory_v1_inventory_tracking_lots_full_history.csv`

#### Sheet `stock_lot`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `product_id` |  | Derived/Lookup |
| `company_id` |  | Derived/Lookup |
| `ref` |  | Derived/Lookup |

#### Sheet `stock_quant`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `product_id` |  | Derived/Lookup |
| `location_id` |  | Derived/Lookup |
| `lot_id` |  | Derived/Lookup |
| `inventory_quantity` |  | Derived/Lookup |

### `17_Reordering_Rules`

Source file(s): `08_mdm_v1_supply_items_full_history.csv`

#### Sheet `stock_warehouse_orderpoint`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `active` |  | Derived/Lookup |
| `trigger` |  | Derived/Lookup |
| `product_id` |  | Derived/Lookup |
| `warehouse_id` |  | Derived/Lookup |
| `location_id` |  | Derived/Lookup |
| `product_min_qty` |  | Derived/Lookup |
| `product_max_qty` |  | Derived/Lookup |
| `replenishment_uom_id` |  | Derived/Lookup |
| `company_id` |  | Derived/Lookup |
| `route_id` |  | Derived/Lookup |

### `18_Delivery_Carriers`

Source file(s): `15_sales_v1_orders_full_history.csv`, `17_purchasing_v1_receipts_full_history.csv`

#### Sheet `delivery_carrier`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `name` |  | Derived/Lookup |
| `delivery_type` |  | Derived/Lookup |
| `product_id` |  | Derived/Lookup |
| `company_id` |  | Derived/Lookup |
| `sequence` |  | Derived/Lookup |
| `active` |  | Derived/Lookup |
| `fixed_price` |  | Derived/Lookup |
| `margin` |  | Derived/Lookup |
| `fixed_margin` |  | Derived/Lookup |
| `free_over` |  | Derived/Lookup |
| `amount` |  | Derived/Lookup |
| `country_ids` |  | Derived/Lookup |
| `state_ids` |  | Derived/Lookup |
| `max_weight` |  | Derived/Lookup |
| `max_volume` |  | Derived/Lookup |
| `must_have_tag_ids` |  | Derived/Lookup |
| `excluded_tag_ids` |  | Derived/Lookup |
| `integration_level` |  | Derived/Lookup |
| `allow_cash_on_delivery` |  | Derived/Lookup |
| `tracking_url` |  | Derived/Lookup |

### `Purchase pricelist`

Source file(s): `14_sales_v1_price_adjustments_full_history.csv`

#### Sheet `product_supplierinfo`

| Odoo field | Suggested Plex column | Mapping rule |
|---|---|---|
| `id` |  | Derived/Lookup |
| `partner_id` |  | Derived/Lookup |
| `product_tmpl_id` |  | Derived/Lookup |
| `product_id` |  | Derived/Lookup |
| `min_qty` |  | Derived/Lookup |
| `price` |  | Derived/Lookup |
| `currency_id` |  | Derived/Lookup |
| `product_uom_id` |  | Derived/Lookup |
| `delay` |  | Derived/Lookup |
| `product_code` |  | Derived/Lookup |
| `product_name` |  | Derived/Lookup |

