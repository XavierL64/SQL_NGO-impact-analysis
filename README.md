# SQL_NGO-impact-analysis

Query a PostgreSQL database containing records of assignments, funding, impacts and donor activities for a NGO focusing on education, healthcare, and sustainable development. The data covers the period 2010 to 2023. The database includes three tables: 

**assignments**

Details about each project, including its name, duration (start and end dates), budget, geographical region, and the impact score.

assignment_id (integer)
assignment_name (varchar)
start_date (varchar)
end_date (varchar)
budget (decimal)
region (varchar)
impact_score (decimal)

**donations**

Records of financial contributions, linked to specific donors and assignments, highlighting how financial support is allocated and utilized.

donation_id (integer)
donor_id (integer)
amount (decimal)
donation_date (text)
assignment_id (integer)
status (varchar)
created_at (timestamp)

**donors**

Information on individuals and organizations that fund GoodThought’s projects, including donor types.

donor_id (integer)
donor_name (varchar)
donor_type (varchar)
