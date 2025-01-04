# Smith-School-Rankings-Scrutiny

## Project Overview

The Smith School Rankings Scrutiny project, aims to model a database for ranking various UMD Smith School programs. The goal is to provide a comprehensive data structure that enables multi-year ranking analysis for graduate programs, facilitating data-driven decision-making for the Smith School.

## Key Objectives

1. Identify the top 5 ranked programs over the last 3 years
2. Find the top 5 improved/declined programs over the last 3 years
3. Determine the top 5 programs with consistent ranking across all ranking sources
4. Identify the top 3 performing degrees based on program rankings
5. Calculate the proportion of programs that improved/declined over the last year

## Database Design

### Conceptual Model: ER Diagram

The ER diagram represents the relationships between Program, ProgramCategory, ProgramType, RankingSource, and Rank entities.

### Logical Model: Relational Schema

- Program (programId, programName, prgCtgryId, prgTypeId)
- ProgramCategory (prgCtgryId, prgCtgryName)
- ProgramType (prgTypeId, prgTypeName)
- RankingSource (rnkngSrcId, rnkngSrcName)
- Rank (programId, rnkngSrcId, rankingYear, rankingPosition, rankingPositionPrevYear)

### Physical Model

The database was implemented using SQL Server, with appropriate table creation statements, primary and foreign key constraints, and data insertion queries.

## Key Findings

The project includes SQL queries to answer the following questions:

1. Top 5 ranked programs over the last 3 years
2. Programs with the most significant improvement or decline in rankings
3. Programs maintaining consistent rankings across all ranking sources
4. Top 3 performing degrees based on program rankings
5. Proportion of programs that improved or declined in rankings over the last year

## Technologies Used

- Lucidchart
- SQL Server

## How to Run the Project

1. Execute the SQL scripts in the following order:
   - Table creation scripts
   - Data insertion scripts
   - View creation and query scripts for each business question

2. Analyze the results of each query to gain insights into the program rankings

## Conclusion

This project provides a comprehensive database solution for analyzing UMD Smith School program rankings. By implementing the designed database and executing the provided queries, the Smith School can gain valuable insights into their program performance, track improvements, and make data-driven decisions to enhance their academic offerings.
