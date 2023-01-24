# Library-Managment-SQL

##Documentation for Library Management System SQL Code:

This SQL code is for a library management system that includes three tables: Book, Member, and Loan.

Book Table:
The Book table contains information about each book in the library's collection.
The primary key for this table is the BookID column, which is an integer and is used to uniquely identify each book.
Other columns in the table include Title, Author, ISBN, PublicationDate, NumberOfPages, and Genre.
The table has a 1:1 relationship with the Loan table, meaning that for each book in the collection, there can be only one loan associated with it.
Member Table:
The Member table contains information about each library member.
The primary key for this table is the MemberID column, which is an integer and is used to uniquely identify each member.
Other columns in the table include FirstName, LastName, Email, PhoneNumber, Address, MembershipStartDate, MembershipEndDate, and MembershipType.
The table has a 1:1 relationship with the Loan table, meaning that for each member, there can be only one loan associated with them.
Loan Table:
The Loan table contains information about each book loan.
The primary key for this table is the LoanID column, which is an integer and is used to uniquely identify each loan.
Other columns in the table include BookID, MemberID, LoanDate, DueDate, ReturnDate, Fine, and IsOverdue.
The BookID and MemberID columns are foreign keys, linking to the primary keys of the Book and Member tables, respectively. This ensures that each loan is associated with the correct book and member.
Note:

The Fine column is used to store the fine amount when the loan is overdue and the IsOverdue column is used to indicate whether the loan is overdue or not.

The data types used in the table are INT, VARCHAR, DATE and DECIMAL.

This SQL code is for logical design only and it can be used as a reference for creating physical schema in the database.
