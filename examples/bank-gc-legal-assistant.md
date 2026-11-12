# Legal Assistant for a Bank General Counsel

A version of the Legal Assistant built for the Office of the General Counsel at a community bank. It reads vendor contracts, NDAs, leases and employment documents from the bank's side and gives the GC a two-minute view: what the document says, what's wrong with it, and what needs a decision. It runs inside the tools a bank already approves (for example, Microsoft Copilot), from one instruction file attached to the chat.

It is not a lawyer. The GC decides.

## What it checks beyond a standard review

- **Regulators' access.** Audit and access rights for the bank, its examiners and its auditors.
- **Incident notice.** Vendor notice early enough for the bank to meet the FDIC 36-hour and NYDFS 72-hour reporting windows.
- **Bank data.** The bank owns it. No vendor use or AI training, and certified destruction at exit.
- **Mergers.** Assignment to a successor bank without consent or fees; termination and deconversion costs.
- **Supervisory information.** No clause may force disclosure of confidential supervisory information, and regulators can always be told.
- **Insiders.** Transactions with directors or affiliates are flagged for Board approval.

Anything it isn't sure of is marked "verify". It never invents citations.

## Sample review (fictional bank, fictional contract)

*PRIVILEGED & CONFIDENTIAL. Prepared at the direction of the General Counsel. Draft for attorney review. Not a legal opinion.*

**Side:** Reviewed from the Bank's side as customer.

**Summary:** Master SaaS agreement between Harbor Community Bank and LedgerCloud Inc. for online-banking analytics, 3-year term. The main risk is data: the vendor may use bank data to train its models. 5 items are worth raising before signing. Overall: **HIGH**.

### Risks

| # | Section | Short quote | What can go wrong | Who bears it | Severity | LAW? |
|---|---|---|---|---|---|---|
| 1 | 6.4 | "aggregated and de-identified Customer Data to improve the Services" | Vendor can train its AI on bank customer data | Bank | HIGH | Verify |
| 2 | 9.2 | "notify Customer within five (5) business days" | Too late for the bank's 36-hour FDIC and 72-hour NYDFS notices | Bank | HIGH | Yes |
| 3 | 14.1 | "may not assign... including by merger" | A merger would need vendor consent | Bank | MEDIUM | |
| 4 | 11.3 | liability cap of "fees paid in the prior 3 months" | Cap covers data breach too; roughly $30K against a breach | Bank | HIGH | |
| 5 | 3.2 | "renews automatically... unless 180 days' notice" | Easy to miss the exit window | Bank | LOW | |

### Drafting errors

- Section 9.2 refers to "the Security Exhibit (Exhibit D)". The agreement has Exhibits A to C only.
- "Customer Data" is defined in 1.4, but Section 6.4 uses "Client Data".

### Better wording

| Section | Current text | Proposed text | Why |
|---|---|---|---|
| 9.2 | "within five (5) business days" | "without undue delay and in any event within twenty-four (24) hours of discovery" | Leaves time for the bank's regulatory notices |
| 14.1 | "including by merger" | "except that Customer may assign this Agreement without consent to a successor by merger, acquisition or sale of substantially all assets" | Keeps the contract intact through a deal |

### Questions for the GC

1. Is analytics on de-identified data acceptable at all, or should 6.4 be struck?
2. Should data breach sit outside the liability cap?

### Missing documents

Exhibit D (Security), referenced in 9.2.

*Reviewed: LedgerCloud MSA (sample).docx. This review does not say whether to sign, does not predict the outcome of any dispute and does not replace attorney review.*
