Oracle.ManagedDataAccess.Core NuGet Package 3.21.50 README
==========================================================
Release Notes: Oracle Data Provider for .NET Core

December 2021

This provider supports .NET Core 3.1, .NET 5, and .NET 6.

This README supplements the main ODP.NET 21c documentation.
https://docs.oracle.com/en/database/oracle/oracle-database/21/odpnt/


New Features
============
Oracle Identity and Access Management
ODP.NET supports Oracle Identity and Access Management (IAM) cloud service for 
unified identity across Oracle cloud services, including Oracle Cloud Database 
Services, with the core and managed drivers. ODP.NET can use the same Oracle IAM 
credentials for authentication and authorization to the Oracle Cloud and Oracle 
cloud databases, including Autonomous Database. This capability allows single 
sign-on and for identity to be propagated to all services Oracle IAM supports 
including federated users via Azure Active Directory and Microsoft Active 
Directory (on-premises). A unified identity makes user management and account 
management easier for administrators and end users.


Bug Fixes since Oracle.ManagedDataAccess.Core NuGet Package 3.21.41
===================================================================
Bug 33576541 - BULK COPY CANNOT INSERT MORE THAN 255 COLUMNS 


Known Issues and Limitations
============================
1) BindToDirectory throws NullReferenceException on Linux when LdapConnection AuthType is Anonymous

https://github.com/dotnet/runtime/issues/61683

This issue is observed when using System.DirectoryServices.Protocols, version 6.0.0.
To workaround the issue, use System.DirectoryServices.Protocols, version 5.0.1.

 Copyright (c) 2021, 2022, Oracle and/or its affiliates.
