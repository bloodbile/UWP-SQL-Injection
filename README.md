# 🎀 UWP 3.0 SQL Injection 🎀
## Overview
An SQL injection vulnerability has been identified in UWP 3.0, specifically within a POST request to the /engine/stateandparameters.php endpoint. The vulnerability arises from the id parameter, which has been shown to accept malicious payloads, such as 38203170 or 5411=05411 and 77432384 or 4779=4783. The distinct responses generated from these inputs suggest that the application is improperly handling user input, directly incorporating it into SQL queries without adequate sanitization or parameterization.
## Impact
This flaw could potentially allow an attacker to manipulate the backend database, leading to unauthorized data access, data modification, or other severe impacts on application integrity and confidentiality. This exploit is most effective when combined with the discovered default login credentials of user:user.
