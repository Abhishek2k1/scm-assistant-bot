# SCM Assistant – Flowise RAG Chatbot

## Public Chatbot URL
https://cloud.flowiseai.com/chatbot/90ff334a-4978-405d-861d-d7af2075a92a

#LLM Used
###Google Gemini 2.5 Flash (for conversational question answering and reasoning).

#Embedding Model Used
###Google Gemini Embedding (gemini-embedding-001) with the RETRIEVAL_DOCUMENT task type for generating vector embeddings of the CSV and PDF documents.

#Two Chunk Configurations Tried
### PDF: One Document per Page
 Each PDF page was treated as a separate chunk to improve retrieval of specific policy sections and reduce irrelevant context.
### CSV: Row-wise Document Chunking
 Each supplier record (CSV row) was indexed as an individual document, enabling retrieval of supplier-specific performance and procurement information.



# Validation Questions

## Q1

### Question

Which Tier-3 suppliers have an active disruption flag, and what response level applies per policy?

### Answer

I do not have enough information to identify which Tier-3 suppliers have an active disruption flag. The provided context defines what constitutes an "active disruption flag" (e.g., geopolitical tension, seasonal disruption risk, active labour dispute) and how it contributes to a supplier's risk level (Medium or High Risk), but it does not list specific suppliers or their current risk status.

However, if a supplier is flagged as High Risk for two consecutive quarters (which could be due to active disruption flags), the policy states that it must be escalated to the Chief Procurement Officer (CPO) for strategic review.

The CPO review determines one of three outcomes:

(a) Supplier Remediation Plan

(b) Parallel Sourcing Activation (see Section 10)

(c) Supplier Exit Programme initiation with 90-day wind-down period.


## Q2

### Question

Which suppliers qualify for the annual Volume Rebate Program and how many are there?

### Answer

To qualify for the annual Volume Rebate Program, suppliers must meet the following criteria:

Be a Tier-1 supplier.

Maintain an On-Time Delivery (OTD) rate at or above 93.0%.

Have a Defect Rate below 0.5%.

Achieve a Sustainability Score at or above 85.

Meet these criteria for a full calendar year.

Rebate eligibility is assessed in January of the following year.

The provided context describes the criteria for qualification but does not contain the specific performance data (OTD rate, Defect Rate, Sustainability Score) for individual suppliers. This data is stated to be in the "Supplier Performance Data register (CSV format)." Therefore, I do not have enough information to identify which specific suppliers qualify or how many there are.
---

## Q3

### Question

 Which region has the highest total PO value, and does it breach the concentration limit?

### Answer

I do not have enough information. The provided context defines the concentration limit for regions (no single region may account for more than 45% of total annual procurement spend), but it does not provide any data on the total PO value or annual procurement spend for each region (APAC, EMEA, LATAM, NA).
---

## Q4

### Question

Which suppliers are on Supplier Watch List (SWL) status and what does it restrict?

### Answer
I do not have enough information to identify which specific suppliers are currently on Supplier Watch List (SWL) status, as the context only describes the condition for being placed on it (Compliance Score below 60).

However, the context does state what SWL status restricts: it limits new Purchase Order (PO) issuance to 20% of prior quarter volume.
---

## Q5

### Question

Which product category has the highest average defect rate and does it exceed the Tier-2 limit?

### Answer
The product category with the highest average defect rate is Specialty Alloys at 2.93%.

Yes, this average defect rate of 2.93% exceeds the Tier-2 maximum permissible defect rate of 2.50%.


---

# Future Improvements

-Integrate Hybrid RAG with structured CSV analytics for complex calculations.

-Improve retrieval using hybrid search and re-ranking techniques.
---

