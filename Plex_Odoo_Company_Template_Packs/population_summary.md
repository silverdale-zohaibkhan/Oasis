# Population Summary

## Overall

- Companies processed: 4
- Templates processed: 132
- Source rows seen: 384114
- Rows written: 326546
- Removed empty rows: 0
- Removed missing-required rows: 57568
- Overall success rate: 85.01%

## oasis_car_wash_systems

- company_id: `1`
- templates: 33
- source rows seen: 336355
- rows written: 290537
- removed empty rows: 0
- removed missing-required rows: 45818
- success rate: 86.38%

| Template | Source file | Source rows | Written | Empty removed | Missing required removed | Success % |
|---|---|---:|---:|---:|---:|---:|
| `01_Bill_of_Materials__mrp_bom.csv` | `23_engineering_v1_boms_components_full_history.csv` | 14959 | 14959 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_bom_byproduct.csv` | `23_engineering_v1_boms_components_full_history.csv` | 14959 | 14959 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_bom_line.csv` | `23_engineering_v1_boms_components_full_history.csv` | 14959 | 14959 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_routing_workcenter.csv` | `23_engineering_v1_boms_components_full_history.csv` | 14959 | 14959 | 0 | 0 | 100.00 |
| `02_Chart_of_Accounts__account_account.csv` | `18_accounting_v1_journal_entries_full_history.csv` | 2167 | 2167 | 0 | 0 | 100.00 |
| `03_Taxes__account_tax.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__account_tax_group.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__repartition_invoice.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__repartition_refund.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `04_Fiscal_Positions__account_fiscal_position.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `04_Fiscal_Positions__account_fiscal_position_account.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `05_Journals_and_Bank_Accounts__account_journal.csv` | `19_accounting_v1_ap_invoices_full_history.csv` | 39177 | 39177 | 0 | 0 | 100.00 |
| `05_Journals_and_Bank_Accounts__res_partner_bank.csv` | `19_accounting_v1_ap_invoices_full_history.csv` | 39177 | 39177 | 0 | 0 | 100.00 |
| `06_Analytic_Accounts__account_analytic_account.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `06_Analytic_Accounts__account_analytic_plan.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `07_Customers_and_Contacts__customer_children.csv` | `03_mdm_v1_contacts_full_history.csv` | 6995 | 6268 | 0 | 727 | 89.61 |
| `07_Customers_and_Contacts__customer_company.csv` | `03_mdm_v1_contacts_full_history.csv` | 6995 | 6984 | 0 | 11 | 99.84 |
| `08_Customer_Accounting_and_Pricelist__res_partner_properties.csv` | `20_accounting_v1_ar_invoices_full_history.csv` | 21036 | 21036 | 0 | 0 | 100.00 |
| `09_Vendors__vendor_company.csv` | `19_accounting_v1_ap_invoices_full_history.csv` | 39177 | 0 | 0 | 39177 | 0.00 |
| `10_Product_Category_and_UoM__product_category.csv` | `01_mdm_v1_parts_full_history.csv` | 14360 | 14348 | 0 | 12 | 99.92 |
| `10_Product_Category_and_UoM__uom_uom.csv` | `01_mdm_v1_parts_full_history.csv` | 14360 | 14348 | 0 | 12 | 99.92 |
| `11_Products__product_product.csv` | `01_mdm_v1_parts_full_history.csv` | 14360 | 14360 | 0 | 0 | 100.00 |
| `11_Products__product_template.csv` | `01_mdm_v1_parts_full_history.csv` | 14360 | 14348 | 0 | 12 | 99.92 |
| `12_Sales_Pricelists__product_pricelist.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 47 | 47 | 0 | 0 | 100.00 |
| `12_Sales_Pricelists__product_pricelist_item.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 47 | 47 | 0 | 0 | 100.00 |
| `13_Work_Centers__mrp_workcenter.csv` | `05_mdm_v1_operations_full_history.csv` | 22 | 0 | 0 | 22 | 0.00 |
| `15_Warehouses_and_Locations__stock_location.csv` | `09_inventory_v1_inventory_definitions_locations_full_history.csv` | 880 | 0 | 0 | 880 | 0.00 |
| `15_Warehouses_and_Locations__stock_warehouse.csv` | `09_inventory_v1_inventory_definitions_locations_full_history.csv` | 880 | 0 | 0 | 880 | 0.00 |
| `16_Lots_and_Inventory_Quant__stock_lot.csv` | `10_inventory_v1_inventory_tracking_containers_full_history.csv` | 4085 | 0 | 0 | 4085 | 0.00 |
| `16_Lots_and_Inventory_Quant__stock_quant.csv` | `10_inventory_v1_inventory_tracking_containers_full_history.csv` | 4085 | 4085 | 0 | 0 | 100.00 |
| `17_Reordering_Rules__stock_warehouse_orderpoint.csv` | `08_mdm_v1_supply_items_full_history.csv` | 320 | 320 | 0 | 0 | 100.00 |
| `18_Delivery_Carriers__delivery_carrier.csv` | `17_purchasing_v1_receipts_full_history.csv` | 53942 | 53942 | 0 | 0 | 100.00 |
| `Purchase_pricelist__product_supplierinfo.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 47 | 47 | 0 | 0 | 100.00 |

## wade_management

- company_id: `2`
- templates: 33
- source rows seen: 29985
- rows written: 21081
- removed empty rows: 0
- removed missing-required rows: 8904
- success rate: 70.31%

| Template | Source file | Source rows | Written | Empty removed | Missing required removed | Success % |
|---|---|---:|---:|---:|---:|---:|
| `01_Bill_of_Materials__mrp_bom.csv` | `05_mdm_v1_operations_full_history.csv` | 8 | 8 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_bom_byproduct.csv` | `05_mdm_v1_operations_full_history.csv` | 8 | 8 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_bom_line.csv` | `05_mdm_v1_operations_full_history.csv` | 8 | 8 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_routing_workcenter.csv` | `05_mdm_v1_operations_full_history.csv` | 8 | 8 | 0 | 0 | 100.00 |
| `02_Chart_of_Accounts__account_account.csv` | `18_accounting_v1_journal_entries_full_history.csv` | 2250 | 2250 | 0 | 0 | 100.00 |
| `03_Taxes__account_tax.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__account_tax_group.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__repartition_invoice.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__repartition_refund.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `04_Fiscal_Positions__account_fiscal_position.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `04_Fiscal_Positions__account_fiscal_position_account.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `05_Journals_and_Bank_Accounts__account_journal.csv` | `19_accounting_v1_ap_invoices_full_history.csv` | 8422 | 8422 | 0 | 0 | 100.00 |
| `05_Journals_and_Bank_Accounts__res_partner_bank.csv` | `19_accounting_v1_ap_invoices_full_history.csv` | 8422 | 8422 | 0 | 0 | 100.00 |
| `06_Analytic_Accounts__account_analytic_account.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `06_Analytic_Accounts__account_analytic_plan.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `07_Customers_and_Contacts__customer_children.csv` | `03_mdm_v1_contacts_full_history.csv` | 48 | 15 | 0 | 33 | 31.25 |
| `07_Customers_and_Contacts__customer_company.csv` | `03_mdm_v1_contacts_full_history.csv` | 48 | 48 | 0 | 0 | 100.00 |
| `08_Customer_Accounting_and_Pricelist__res_partner_properties.csv` | `20_accounting_v1_ar_invoices_full_history.csv` | 534 | 534 | 0 | 0 | 100.00 |
| `09_Vendors__vendor_company.csv` | `19_accounting_v1_ap_invoices_full_history.csv` | 8422 | 0 | 0 | 8422 | 0.00 |
| `10_Product_Category_and_UoM__product_category.csv` | `08_mdm_v1_supply_items_full_history.csv` | 147 | 0 | 0 | 147 | 0.00 |
| `10_Product_Category_and_UoM__uom_uom.csv` | `08_mdm_v1_supply_items_full_history.csv` | 147 | 0 | 0 | 147 | 0.00 |
| `11_Products__product_product.csv` | `08_mdm_v1_supply_items_full_history.csv` | 147 | 147 | 0 | 0 | 100.00 |
| `11_Products__product_template.csv` | `08_mdm_v1_supply_items_full_history.csv` | 147 | 0 | 0 | 147 | 0.00 |
| `12_Sales_Pricelists__product_pricelist.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `12_Sales_Pricelists__product_pricelist_item.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `13_Work_Centers__mrp_workcenter.csv` | `05_mdm_v1_operations_full_history.csv` | 8 | 0 | 0 | 8 | 0.00 |
| `15_Warehouses_and_Locations__stock_location.csv` | `07_mdm_v1_buildings_full_history.csv` | 1 | 1 | 0 | 0 | 100.00 |
| `15_Warehouses_and_Locations__stock_warehouse.csv` | `07_mdm_v1_buildings_full_history.csv` | 1 | 1 | 0 | 0 | 100.00 |
| `16_Lots_and_Inventory_Quant__stock_lot.csv` | `10_inventory_v1_inventory_tracking_containers_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `16_Lots_and_Inventory_Quant__stock_quant.csv` | `10_inventory_v1_inventory_tracking_containers_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `17_Reordering_Rules__stock_warehouse_orderpoint.csv` | `08_mdm_v1_supply_items_full_history.csv` | 147 | 147 | 0 | 0 | 100.00 |
| `18_Delivery_Carriers__delivery_carrier.csv` | `17_purchasing_v1_receipts_full_history.csv` | 1062 | 1062 | 0 | 0 | 100.00 |
| `Purchase_pricelist__product_supplierinfo.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |

## wade_real_estate

- company_id: `3`
- templates: 33
- source rows seen: 2259
- rows written: 1626
- removed empty rows: 0
- removed missing-required rows: 633
- success rate: 71.98%

| Template | Source file | Source rows | Written | Empty removed | Missing required removed | Success % |
|---|---|---:|---:|---:|---:|---:|
| `01_Bill_of_Materials__mrp_bom.csv` | `05_mdm_v1_operations_full_history.csv` | 8 | 8 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_bom_byproduct.csv` | `05_mdm_v1_operations_full_history.csv` | 8 | 8 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_bom_line.csv` | `05_mdm_v1_operations_full_history.csv` | 8 | 8 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_routing_workcenter.csv` | `05_mdm_v1_operations_full_history.csv` | 8 | 8 | 0 | 0 | 100.00 |
| `02_Chart_of_Accounts__account_account.csv` | `18_accounting_v1_journal_entries_full_history.csv` | 215 | 215 | 0 | 0 | 100.00 |
| `03_Taxes__account_tax.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__account_tax_group.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__repartition_invoice.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__repartition_refund.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `04_Fiscal_Positions__account_fiscal_position.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `04_Fiscal_Positions__account_fiscal_position_account.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `05_Journals_and_Bank_Accounts__account_journal.csv` | `19_accounting_v1_ap_invoices_full_history.csv` | 623 | 623 | 0 | 0 | 100.00 |
| `05_Journals_and_Bank_Accounts__res_partner_bank.csv` | `19_accounting_v1_ap_invoices_full_history.csv` | 623 | 623 | 0 | 0 | 100.00 |
| `06_Analytic_Accounts__account_analytic_account.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `06_Analytic_Accounts__account_analytic_plan.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `07_Customers_and_Contacts__customer_children.csv` | `02_mdm_v1_customers_full_history.csv` | 2 | 0 | 0 | 2 | 0.00 |
| `07_Customers_and_Contacts__customer_company.csv` | `02_mdm_v1_customers_full_history.csv` | 2 | 2 | 0 | 0 | 100.00 |
| `08_Customer_Accounting_and_Pricelist__res_partner_properties.csv` | `20_accounting_v1_ar_invoices_full_history.csv` | 129 | 129 | 0 | 0 | 100.00 |
| `09_Vendors__vendor_company.csv` | `19_accounting_v1_ap_invoices_full_history.csv` | 623 | 0 | 0 | 623 | 0.00 |
| `10_Product_Category_and_UoM__product_category.csv` | `01_mdm_v1_parts_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `10_Product_Category_and_UoM__uom_uom.csv` | `01_mdm_v1_parts_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `11_Products__product_product.csv` | `01_mdm_v1_parts_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `11_Products__product_template.csv` | `01_mdm_v1_parts_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `12_Sales_Pricelists__product_pricelist.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `12_Sales_Pricelists__product_pricelist_item.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `13_Work_Centers__mrp_workcenter.csv` | `05_mdm_v1_operations_full_history.csv` | 8 | 0 | 0 | 8 | 0.00 |
| `15_Warehouses_and_Locations__stock_location.csv` | `07_mdm_v1_buildings_full_history.csv` | 1 | 1 | 0 | 0 | 100.00 |
| `15_Warehouses_and_Locations__stock_warehouse.csv` | `07_mdm_v1_buildings_full_history.csv` | 1 | 1 | 0 | 0 | 100.00 |
| `16_Lots_and_Inventory_Quant__stock_lot.csv` | `10_inventory_v1_inventory_tracking_containers_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `16_Lots_and_Inventory_Quant__stock_quant.csv` | `10_inventory_v1_inventory_tracking_containers_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `17_Reordering_Rules__stock_warehouse_orderpoint.csv` | `08_mdm_v1_supply_items_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `18_Delivery_Carriers__delivery_carrier.csv` | `15_sales_v1_orders_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |
| `Purchase_pricelist__product_supplierinfo.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 0 | 0 | 0 | 0 | 100.00 |

## wadler_manufacturing

- company_id: `4`
- templates: 33
- source rows seen: 15515
- rows written: 13302
- removed empty rows: 0
- removed missing-required rows: 2213
- success rate: 85.74%

| Template | Source file | Source rows | Written | Empty removed | Missing required removed | Success % |
|---|---|---:|---:|---:|---:|---:|
| `01_Bill_of_Materials__mrp_bom.csv` | `23_engineering_v1_boms_components_full_history.csv` | 175 | 175 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_bom_byproduct.csv` | `23_engineering_v1_boms_components_full_history.csv` | 175 | 175 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_bom_line.csv` | `23_engineering_v1_boms_components_full_history.csv` | 175 | 175 | 0 | 0 | 100.00 |
| `01_Bill_of_Materials__mrp_routing_workcenter.csv` | `23_engineering_v1_boms_components_full_history.csv` | 175 | 175 | 0 | 0 | 100.00 |
| `02_Chart_of_Accounts__account_account.csv` | `18_accounting_v1_journal_entries_full_history.csv` | 1790 | 1790 | 0 | 0 | 100.00 |
| `03_Taxes__account_tax.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__account_tax_group.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__repartition_invoice.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `03_Taxes__repartition_refund.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `04_Fiscal_Positions__account_fiscal_position.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `04_Fiscal_Positions__account_fiscal_position_account.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `05_Journals_and_Bank_Accounts__account_journal.csv` | `20_accounting_v1_ar_invoices_full_history.csv` | 2347 | 2347 | 0 | 0 | 100.00 |
| `05_Journals_and_Bank_Accounts__res_partner_bank.csv` | `20_accounting_v1_ar_invoices_full_history.csv` | 2347 | 2347 | 0 | 0 | 100.00 |
| `06_Analytic_Accounts__account_analytic_account.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `06_Analytic_Accounts__account_analytic_plan.csv` | `` | 0 | 0 | 0 | 0 | 100.00 |
| `07_Customers_and_Contacts__customer_children.csv` | `03_mdm_v1_contacts_full_history.csv` | 485 | 388 | 0 | 97 | 80.00 |
| `07_Customers_and_Contacts__customer_company.csv` | `03_mdm_v1_contacts_full_history.csv` | 485 | 485 | 0 | 0 | 100.00 |
| `08_Customer_Accounting_and_Pricelist__res_partner_properties.csv` | `20_accounting_v1_ar_invoices_full_history.csv` | 2347 | 2347 | 0 | 0 | 100.00 |
| `09_Vendors__vendor_company.csv` | `19_accounting_v1_ap_invoices_full_history.csv` | 1892 | 0 | 0 | 1892 | 0.00 |
| `10_Product_Category_and_UoM__product_category.csv` | `01_mdm_v1_parts_full_history.csv` | 101 | 101 | 0 | 0 | 100.00 |
| `10_Product_Category_and_UoM__uom_uom.csv` | `01_mdm_v1_parts_full_history.csv` | 101 | 101 | 0 | 0 | 100.00 |
| `11_Products__product_product.csv` | `01_mdm_v1_parts_full_history.csv` | 101 | 101 | 0 | 0 | 100.00 |
| `11_Products__product_template.csv` | `01_mdm_v1_parts_full_history.csv` | 101 | 101 | 0 | 0 | 100.00 |
| `12_Sales_Pricelists__product_pricelist.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 4 | 4 | 0 | 0 | 100.00 |
| `12_Sales_Pricelists__product_pricelist_item.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 4 | 4 | 0 | 0 | 100.00 |
| `13_Work_Centers__mrp_workcenter.csv` | `05_mdm_v1_operations_full_history.csv` | 4 | 0 | 0 | 4 | 0.00 |
| `15_Warehouses_and_Locations__stock_location.csv` | `09_inventory_v1_inventory_definitions_locations_full_history.csv` | 7 | 0 | 0 | 7 | 0.00 |
| `15_Warehouses_and_Locations__stock_warehouse.csv` | `09_inventory_v1_inventory_definitions_locations_full_history.csv` | 7 | 0 | 0 | 7 | 0.00 |
| `16_Lots_and_Inventory_Quant__stock_lot.csv` | `10_inventory_v1_inventory_tracking_containers_full_history.csv` | 206 | 0 | 0 | 206 | 0.00 |
| `16_Lots_and_Inventory_Quant__stock_quant.csv` | `10_inventory_v1_inventory_tracking_containers_full_history.csv` | 206 | 206 | 0 | 0 | 100.00 |
| `17_Reordering_Rules__stock_warehouse_orderpoint.csv` | `08_mdm_v1_supply_items_full_history.csv` | 18 | 18 | 0 | 0 | 100.00 |
| `18_Delivery_Carriers__delivery_carrier.csv` | `15_sales_v1_orders_full_history.csv` | 2258 | 2258 | 0 | 0 | 100.00 |
| `Purchase_pricelist__product_supplierinfo.csv` | `14_sales_v1_price_adjustments_full_history.csv` | 4 | 4 | 0 | 0 | 100.00 |

