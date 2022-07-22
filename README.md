- 👋 Hi, I’m @fetaeib
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
fetaeib/fetaeib is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

graph TD
    A[SI-ALL] --> |Portfolio owner bank accounts| B(SI-OWN)
    A --> |Counterparty bank accounts| C(SI-CPTY)
    C --->|cash| D[SI-CPTY-NOSTRO]
    C --->|custody| E[SI-CPTY-CUST]

    B --> |Securities Depo| G(SI-OWN-ICSD)
    B --> |Central Banks| H(SI-OWN-CENTRAL)
    B --> |Correspondent Bank| I(SI-OWN-CCB)
    B --> |T&B partner| J(SI-OWN-TB-PARTNER)
    B --> |In-house bank| K(SI-OWN-INH)

    I --> |custody|L(SI-OWN-CCB-CUST)
    I --> |cash| M(SI-OWN-CCB-NOST)
    I --> |Admin/Fees/Payments/Transfers| N(SI-OWN-CCB-OTH)
