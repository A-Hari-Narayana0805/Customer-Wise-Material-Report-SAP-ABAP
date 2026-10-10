# Customer-Wise Material Report – SAP ABAP

## Project Overview
This project is developed using SAP ABAP to display customer-wise material and sales order information. It retrieves data from standard SAP tables using Open SQL joins and displays the results in an ALV report.

## Technologies Used
- SAP ABAP
- Open SQL
- SAP SD (Sales and Distribution)
- SALV ALV

## Key Features
- Sales organization selection
- Creation date range selection
- Customer number filtering
- Material number filtering
- Input validation
- Customer and material data retrieval
- ALV output with optimized column widths
- No-data-found message handling

## SAP Tables Used
| Table | Description |
|---|---|
| VBAK | Sales Document Header |
| VBAP | Sales Document Item |
| KNA1 | Customer Master |
| MARA | General Material Data |
| MAKT | Material Descriptions |

## Project Structure
1. `ZCL_CUST_MAT1748.abap` – Class definition and implementation for input validation, data retrieval, and ALV display.
2. `ZRMM_CUST_MAT1748.abap` – Main report program.
3. `ZRMM_CUST_MAT1748_TOP.abap` – Global data declarations.
4. `ZRMM_CUST_MAT1748_SEL.abap` – Selection-screen definitions.
5. `ZRMM_CUST_MAT1748_F01.abap` – Initialization, input validation, and report execution.

## Selection Criteria
- Sales Organization (VKORG)
- Creation Date (ERDAT)
- Customer Number (KUNNR)
- Material Number (MATNR)

## Output
The report displays customer number, customer name, material number, material description, material type, order quantity, unit of measure, and plant in an ALV table.

## Learning Outcomes
- Working with SAP standard tables
- Implementing ABAP Objects
- Writing Open SQL queries with joins
- Creating selection screens and include programs
- Displaying data using SALV ALV

## Author
Ayitha Hari Narayana
